# CSS
## Selector
### Priority
- ID 选择器， 如 #id{}
- 类选择器， 如 .class{}
- 属性选择器， 如 a[href="segmentfault.com"]{}
- 伪类选择器， 如 :hover{}
- 伪元素选择器， 如 ::before{}
- 标签选择器， 如 span{}
- 通配选择器， 如 *{}

内联样式 > ID 选择器 > 类选择器 = 属性选择器 = 伪类选择器 > 标签选择器 = 伪元素选择器
## Resopnsive Design
## Flexbox
### CSS Grid vs Flexbox
1 CSS Grid Layout is a two-dimensional system, meaning it can handle both columns and rows, unlike flexbox which is largely a one-dimensional system (either in a column or a row).
2 A core difference between CSS Grid and Flexbox is that — CSS Grid’s approach is layout-first while Flexbox’ approach is content-first.If you are well aware of your content before making layout, then blindly opt for Flexbox and if not, opt for CSS Grid.
3 Flexbox layout is most appropriate to the components of an application (as most of them are fundamentally linear), and small-scale layouts, while the Grid layout is intended for larger scale layouts which aren’t linear in their design.
4 If you only need to define a layout as a row or a column, then you probably need flexbox. If you want to define a grid and fit content into it in two dimensions — you need the grid.
## Preprocessor
### Sass
### Less
### Stylus
