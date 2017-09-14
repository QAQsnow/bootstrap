BOOTSTRAP DAY02:
 * 按钮
   * HTML元素
     * <button>
     * <input type="button">
     * <a>
   * CSS样式
     * 基类 - .btn
     * 修饰类 - .btn-*
       * default
       * info
       * warning
       * ...
     * 尺寸类 - .btn-*
       * btn-lg - 大按钮
       * btn-sm - 小按钮
       * btn-xs - 最小按钮
     * 块级元素 - .btn-block
 * 图片 - 图片的显示宽度(px->%)
   * 响应式图片 - .img-responsive
   * 图片形状
     * 方形
       * .img-rounded - 圆角矩形
       * .img-thumbnail - 带边框
     * 圆形 - .img-circle
 * 文本
   * 颜色设置 - .text-*
     * info
     * warning
     * danger
     * ...
   * 对齐
     * .text-left - 左对齐
     * .text-center - 居中对齐
     * .text-right - 右对齐
     * .text-justify - 两端对齐(自动换行)
     * .text-nowrap - 两端对齐(不会换行)
 * 列表(自定义列表)
   * 默认样式
   * 水平排列
     .dl-horizontal 被添加在<dl>元素
 * 表格
   <table>
     <thead>
       <tr>
         <th></th>
       </tr>
     </thead>
     <tbody>
       <tr>
         <td><td>
       </tr>
     </tbody>
     <tfoot>
       <tr>
         <td><td>
       </tr>
     </tfoot>
   </table>
 * 表单
   * HTML
     <form id="" name="myForm" enctype="application/x-www-form-urlencoded" action="url" method="get|post">
       <input type="submit">
     </form>
   * JS逻辑
     * 如何获取表单?
       * formId - document.getElementById()
       * formName
         document.getElementsByName()
	 document.formName
       * document.forms[i]
     * 阻止表单的自动提交
       submit.onclick = function(event){
          event.preventDefault();
	  return false;
       }
   * 
* 组件
  * 字体图标库
    * 基类 - .glyphicon
    * 图标类 - .glyphicon-*
  * 下拉菜单
    * 
    * 交互效果(动态JS)
      * (不建议)通过 JavaScript 代码实现
        * 类似于 jQuery UI 的组件
      * 通过 data-* 属性实现
  * 按钮组
    * 
* 总结
  * Bootstrap
    * HTML 页面的布局和样式
      * 直接使用 Bootstrap 提供预定义 class
    * 开发的 Web应用 或 网站
      * 使用统一一套 CSS 内容,样式相似
  * 
* 扩展内容
  * 自调函数
    (function(win){
      // 私有变量或内部函数
      var jQuery = {}
      // 将私有变量开放给全局域
      window.jQuery = window.$ = jQuery;
    })(window);
    +function(win){}(window);
  * SVG的使用场景
    * 网站页面所使用的各类图标
    * 地图类
  * HTML5新特性
    * 应用类
      * 地图类
        * SVG
	* LocalStorage
	* 拖放
      * 博客网站 - 离线应用
        * 文件系统 File
	* 在线与离线事件
    * 游戏类
      * Canvas - 2D效果
      * WebGL - 3D效果