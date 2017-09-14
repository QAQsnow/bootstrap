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
     * 动态效果
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
       </div>
     * 动态效果
       以下属性必须设置在轮播图的容器元素上
       * data-ride="carousel"
       * class="slide"
 * 定制(bootstrap.css文件)
   Less - CSS的预处理器(css具有编程性)
 * 扩展内容
   * 开发中到底是否使用第三方JS库或框架
     * 支持使用第三方库(国内)
       * 简便或降低难度
     * 不赞同使用第三方库(国外)
       * 依赖性不高 - 得不偿失
       * 任何第三方库或框架具有局限性
   * 