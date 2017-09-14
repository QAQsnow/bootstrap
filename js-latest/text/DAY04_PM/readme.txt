BOOTSTRAP DAY04:
 * 插件
   * 下拉菜单
   * 标签页
   * 警告框
   * 工具提示
     * 工具提示的属性 - title
     * data-*属性
       * data-toggle="tooltip" - 实现动态效果
       * data-placement属性 - 设置显示的方向
         * left
	 * top
	 * right
	 * bottom
     * JavaScript代码
       * 调用 tooltip() 方法
   * 弹出框
     * 弹出框的属性
       * title - 设置弹出框的标题
       * data-content - 设置弹出框的内容
     * data-*属性
       * data-toggle="popover" - 实现动态效果
       * data-placement属性 - 设置显示的方向
         * left
	 * top
	 * right
	 * bottom
     * JavaScript代码
       * 调用 popover() 方法
   * 模态框
     * HTML结构
       模态框容器元素
       <div class="modal">
         对话框的容器元素
         <div class="modal-dialog">
	   模态框内容的容器元素
	   <div class="modal-content">
	     模态框的头部
	     <div class="modal-header"></div>
	     模态框的主体
	     <div class="modal-body"></div>
	     模态框的注脚
	     <div class="modal-footer"></div>
	   </div>
	 </div>
       </div>
     * 动态效果
       * data-toggle="modal" - 打开模态框
       * data-dismiss="modal" - 关闭模态框
     * 与jQuery UI的模态框的区别
       * jQuery UI模态框(正常关闭)
       * Bootstrap模态框(非正常关闭)
   * 轮播图
     * HTML结构
       轮播图的容器元素
       <div 
            id=""
	    class="carousel">
         轮播图使用图片的容器元素
	 <div class="carousel-inner">
	   每个使用图片的容器元素
	   <div class="item">
	     引入图片
	     <img src="" />
	     定义说明文字
	     <div class="carousel-caption">
	       说明文字
	     </div>
	   </div>
	 </div>
	 定义手动控制轮播效果的按钮
	 <a 
	    class="left carousel-control"
	    href="#轮播图的容器ID"
	    data-slide="prev">
	   <span 
	     class="glyphicon 
	        glyphicon-chevron-left">
	   </span>
	 </a>
	 <a 
	    class="right carousel-control"
	    href="#轮播图的容器ID"
	    data-slide="next">
	   <span 
	     class="glyphicon 
	        glyphicon-chevron-right">
	   </span>
	 </a>
	 轮播图的图片定位器
	 <ol class="carousel-indicators">
	   数量与引入的图片数量相同
	   <li></li>
	   * data-target="#轮播图的容器ID"
	   * data-slide-to="对应图片的编号"
	 </ol>
       </div>
     * 动态效果
       以下属性必须设置在轮播图的容器元素上
       * data-ride="carousel"
       * 添加class="slide"
       * data-interval="毫秒级" - 设置切换时间
 * 定制(bootstrap.css文件)
   * Bootstrap包
     * 用于开发生产环境 - CSS\FONTS\JS
       * 直接使用即可
     * Bootstrap的源码
 * Less - CSS的预处理器(css具有编程性)
   * 两种使用方式
     * 在客户端(浏览器) - less.js文件
       * style.less文件 - 样式的编程
       * 引入 less.js 文件 - 负责转换
     * 在服务器端(Node.js)
       * 验证 Node.js 环境是否有效
         在命令行中输入:node -v
       * 验证 npm 命令是否可用
         在命令行中输入:npm -v
       * 利用npm在线安装Less
         npm install less -g
	 * 导致失效
	   * 在线安装
	     * 可能缺少"-g"参数
	     * 可能安装失败的
	   * 离线安装
	     * 全局命令不能使用
       * 使用 less 命令 - lessc
         * 将 lessc 命令添加系统环境变量中
	 * 进入到 lessc 安装目录
       * lessc 配置到 WebStorm 中
         * 压缩包拷贝(没有中文和空格)的目录
	 * 点击"File"->"Setting"菜单,打开配置窗口
	 * 选中"Tools"->"File Watchers"菜单
	 * 点击"+"号->选择"Less"选项
	 * 配置"Program"选项,选择 lessc.cmd 文件的目录
       * 注意
         lessc命令只对当前工程有效
   * Less的语法
     * 注释
       * CSS中的注释 - 转换为CSS时,保留
         /* 注释 */
       * Less中的注释 - 转换为CSS时,去掉
         // 注释
     * 变量(更像JS中的常量)
       @变量名 : 变量值;
     * 
   * 定制 - bootstrap.less

// 核心的变量和混合
@import "variables.less";
@import "mixins.less";

// CSS重置、打印机和字体图标
@import "normalize.less";
@import "print.less";
@import "glyphicons.less";

// 核心的CSS - CSS样式
@import "scaffolding.less";
@import "type.less";
@import "code.less";
@import "grid.less";
@import "tables.less";
@import "forms.less";
@import "buttons.less";

// 组件
@import "component-animations.less";
@import "dropdowns.less";
@import "button-groups.less";
@import "input-groups.less";
@import "navs.less";
@import "navbar.less";
@import "breadcrumbs.less";
@import "pagination.less";
@import "pager.less";
@import "labels.less";
@import "badges.less";
@import "jumbotron.less";
@import "thumbnails.less";
@import "alerts.less";
@import "progress-bars.less";
@import "media.less";
@import "list-group.less";
@import "panels.less";
@import "responsive-embed.less";
@import "wells.less";
@import "close.less";

// 插件
@import "modals.less";
@import "tooltip.less";
@import "popovers.less";
@import "carousel.less";

// 工具类
@import "utilities.less";
@import "responsive-utilities.less";

 * 扩展内容
   * 开发中到底是否使用第三方JS库或框架
     * 支持使用第三方库(国内)
       * 简便或降低难度
     * 不赞同使用第三方库(国外)
       * 依赖性不高 - 得不偿失
       * 任何第三方库或框架具有局限性
   * 预处理器 - 可编程性
     * CSS样式表
       * Less
       * Sass
       * postCSS
     * HTML(模板引擎)
       * ejs
       * jade
       * haml