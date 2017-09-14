讲师简介：
 * 金云龙
前三个阶段:
 * 一阶段 - HTML5 + CSS3 基础
 * 二阶段 - JAVASCRIPT(ECMA+BOM+DOM)
 * 三阶段 - JQUERY + SERVER + AJAX + HTML5核心(新特性)
 基础内容
 * 四阶段 - BOOTSTRAP + ANGULARJS + JQUERY MOBILE(WEB APP) + 微信 + ...
 应用场景
WEBSTORM的配置:
 * 功能:
   * 代码提示功能
   * 多行编辑 - alt+鼠标左键
   * 编辑器文本大小 - ctrl+鼠标滚轮
 * 配置: File -> Setting
   * Keymap - Eclipse(快捷键方式)
   * 编辑器主题 Editor->Colors&Fonts->Font
BOOTSTRAP DAY01:
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
   * CSS3提供的 媒体查询
 * 
扩展内容:
 * 库(JQUERY)与框架(ANGULARJS)的区别
   * JS库 - 工具(没有思想)
   * JS框架 - 解决方案(具有思想)
 * 集成开发工具
   * WebStorm - Web前端人员称为 神器
   * HBuilder - 国内(免费)