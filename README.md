ADF Sample - MultilineOutputText
================================

The Oracle ADF sample application based on the blog post [ADF - Displaying Multi-Line Text with outputText Component](http://rogersuen.blogspot.com/2014/10/adf-displaying-multi-line-text-with-outputext.html) published on [Roger Suen's Blog](http://rogersuen.blogspot.com).

In summary, we can make use of the `white-space` and `word-wrap` CSS properties to display multi-line text with the `outputText` component. To get the expected width of the `outputText` component in a `panelFormLayout` or `panelGridLayout` component, we can wrap the `outputText` component in a fixed-width containing box. For the `panelFormLayout` component particularly, we can also apply `table-layout: fixed` to the content cells of the `panelFormLayout` component in the skin file to enforce the field width.

Chinese Summary: 

利用 `white-space` 和 `word-wrap` CSS 属性，我们可以用 ADF 的 `outputText` 组件显示自动折行的多行文本。将 `outputText` 组件配合 `panelFormLayout` 和 `panelGridLayout` 布局组件使用时，为了保证 `outputText` 输出指定宽度的多行文本，可以将 `outputText` 组件包裹在一个定宽的 `panelGroupLayout` 组件中，然后再置于 `panelFormLayout` 或者 `panelGridLayout` 组件中。对于 `panelFormLayout` 组件，也可以在 ADF 皮肤文件中为 `panelFormLayout` 组件的 `column` 伪元素中对应的 `table` 元素设置 `table-layout: fixed` 属性，以关闭默认的表格自动布局算法，保证表格按照指定的宽度布局。
