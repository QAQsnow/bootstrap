WEBSTORM的配置:
 * 功能:
   * 代码提示功能
   * 多行编辑 - alt+鼠标左键
   * 编辑器文本大小 - ctrl+鼠标滚轮
 * 配置: File -> Setting
   * Keymap - Eclipse(快捷键方式)
   * 编辑器主题 Editor->Colors&Fonts->Font
BOOTSTRAP :
 * 基础内容
   * 之前的HTML页面与当前真实HTML页面的区别:
     * 之前的HTML页面,运行于桌面电脑浏览器(PC端页面)
     * 当前真实HTML页面
       * 桌面电脑浏览器
       * 移动端(手机+PAD)浏览器
   * 兼容全端显示(HTML页面)
     * 针对不同终端进行开发
     * 在同一页面兼容全端(响应式)
   * 如何实现响应式
     * 手工编写方式
     * 使用已有框架(Bootstrap)
 * 如何测试响应式
   * 使用浏览器(Chrome)的开发者工具
   * 使用移动开发工具提供模拟器
   * 使用真实设备(手机或平板电脑)
 * 手工编写响应式
   * Viewport
     <meta name="viewport" content="width=device-width,initial-scale=1"/>
     viewport属性
     * width宽度
     * height高宽
     * user-scalable - 设置是否允许用户缩放
   * 将绝对单位改为相对单位
     * 宽高 - 像素值(px) -> 百分值(%)
       * 作为容器元素
         根据页面设计进行设置
       * 作为子元素
         公式：当前元素的宽度 / 父元素的宽度 = 百分值
     * 像素值(px) -> 相对值(em)
       * 浏览器对普通字体的默认大小 - 16px
       * 自定义CSS覆盖掉浏览器的默认解析(CSS RESET)
     * 响应式图片
       * width或height - px->%
       * max-width或max-height - px->%
         * 好处 - 避免图片显示时的失真
   * 网格布局 - 解决方案(表格:行和列)
     * 习惯
       * 将HTML页面的宽度分为 12 列
       * 12 列设置为 100%
       CSS代码
       .col-1 { width : 8.33% }
       .col-2 { width : 16.66% }
       .col-3 { width : 25% }
       ...
       .col-12 { width : 100% }
     * 第一种 - 只有一行多列
       * 设置浮动
       CSS代码
       * { float : left; }
     * 第二种 - 具有多行多列
       * 设置行概念
     * CSS的盒子模型(框模型)
       * content-box
         实际宽度 = 边框 + 宽度
       * border-box
   * CSS3提供的 媒体查询
     * 使用方式
       * 类似于HTML引入CSS文件方式
         <link rel="stylesheet" media="媒体类型 操作符 媒体属性" href="">
       * 直接CSS文件中定义
         @media 媒体类型 操作符 媒体属性 {
	     // CSS内容
	 }
     * 媒体查询:
       * 媒体类型
         * all - 所有设备(不常用)
	 * screen - (多用于响应式)
	 * print - 打印机
	 * speech - 屏幕阅读器(盲人)
       * 操作符
         * and - 逻辑与
	 * not - 逻辑非
	 * only - 仅有一个
       * 媒体属性
         * width
	 * max-width
	 * height
	 * max-height
     * 举例
       移动端:
       手机端:<link media="screen and (max-width:576px)">
       平板电脑端:<link media="screen and (max-width:768px)">
       桌面端:
       大桌面端:<link media="screen and (min-width:1200px)">
       普通桌面端:<link media="screen and (min-width:768px)">

       if(width<=576){
         // 手机
       }else if(width<=768){
	 // 平板
       }

       if(width>1200){
         // 大桌面
       }else if(width>768){
         // 普通桌面
       }
 * Bootstrap框架
   * 提供的功能
     * 起步 - 基本使用
     * CSS样式 - 响应式 CSS 使用
     * 组件 - 下拉菜单、导航条等
     * 插件 - 组件的基础上提供交互效果
       * 通过 JavaScript 逻辑完成
       * 是基于 jQuery 实现的
扩展内容:
 * 库(JQUERY)与框架(ANGULARJS)的区别
   * JS库 - 工具(没有思想)
   * JS框架 - 解决方案(具有思想)
 * 集成开发工具
   * WebStorm - Web前端人员称为 神器
   * HBuilder - 国内(免费)
 * CDN 加速服务
   * 本地引入 - 需要文件下载到本地
     * 第三方JS文件 - 存储在自己的服务器
     * 问题
       * 导致HTML页面加载速度变慢
   * CDN加速服务 - 不需要任何下载
     * 第三方JS文件 - 专用服务器(免费)
     * 解决问题
       * 不需要下载任何第三方文件
       * 发布Web应用 - 加速