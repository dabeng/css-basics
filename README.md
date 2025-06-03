# CSS
## Layout
### 多个块状元素的水平垂直居中
```css
#container{
  display: flex;
  justify-content: center; /* This defines the alignment along the main axis */
  align-items: center; /* This defines the alignment along the cross axis */
 }
```
equivalent tailwindwcss utility classes
```html
<div class="flex justify-center items-center">
  <div>01</div>
  <div>02</div>
  <div>03</div>
</div>
```
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

### nth-child selelctor
比如我们有一个列表，包含10个以上的item：
```html
<ol>
  <li>e4rt</li>
  <li>66ert</li>
  <li>i9etr</li>
  <li>fsdg</li>
  <li>gh</li>
  <li>gh</li>
  <li>fwr</li>
  <li>ue56</li>
  <li>34s</li>
</ol>
```
为开头的前2个item和结尾的后2个item加红色
```css
li:nth-child(-n+2),li:nth-last-child(-n+2) {
    color: red;
}
```
为中间的第4个～6个item加蓝色
```css
li:nth-child(n+4):nth-child(-n+6) {
  color: blue;
}
```
## Resopnsive Design
### 举例说明响应式设计
```html
<div class="left">
  <p>Left</p>
</div>

<div class="main">
  <p>Main Content</p>
</div>

<div class="right">
  <p>Right</p>
</div>
```
```css
.left {
  background-color:#2196F3;
  padding:20px;
  float:left;
  width:20%; /* The width is 20%, by default */
}

.main {
  background-color:#f1f1f1;
  padding:20px;
  float:left;
  width:60%; /* The width is 60%, by default */
}

.right {
  background-color:#4CAF50;
  padding:20px;
  float:left;
  width:20%; /* The width is 20%, by default */
}

/* Use a media query to add a break point at 800px: */
@media screen and (max-width:800px) {
 .left  , .main, .right {width:100%;}
}
```

## Flexbox
### CSS Grid vs Flexbox
1. CSS Grid Layout is a two-dimensional system, meaning it can handle both columns and rows, unlike flexbox which is largely a one-dimensional system (either in a column or a row).
2. A core difference between CSS Grid and Flexbox is that — CSS Grid’s approach is layout-first while Flexbox’ approach is content-first.If you are well aware of your content before making layout, then blindly opt for Flexbox and if not, opt for CSS Grid.
3. Flexbox layout is most appropriate to the components of an application (as most of them are fundamentally linear), and small-scale layouts, while the Grid layout is intended for larger scale layouts which aren’t linear in their design.
4. If you only need to define a layout as a row or a column, then you probably need flexbox. If you want to define a grid and fit content into it in two dimensions — you need the grid.

## Preprocessor
### Sass
### Less
### Stylus
