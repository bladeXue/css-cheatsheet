# CSS必知必会

个人向CSS知识点清单。

## 关于布局

## 关于文本

## 关于居中方法

## 关于函数

## 属性列表

[Index of CSS properties](https://www.w3.org/Style/CSS/all-properties.en.html)提供了完整的属性列表。

制作标准：

1. 属性必须来自MDN的有效文档链接。
2. 基于Chrome Group和个人记忆技巧来分组。
3. 折叠重复属性，使得每个属性选项最小化。
4. 有歧义的属性必须添加必要的解释。
5. 当连续几个属性可以用“同一组解释词”的时候，使用`/`将它们并入同一行。

### 1. Layout组

> 布局的任务是：划分页面的画布矩阵，并计算所有元素的应处于的位置和尺寸大小。

- [`display`](https://developer.mozilla.org/en-US/docs/Web/CSS/display)
- [`visibility`](https://developer.mozilla.org/en-US/docs/Web/CSS/visibility)

定位布局相关：

- [`position`](https://developer.mozilla.org/en-US/docs/Web/CSS/position)
- [`top`](https://developer.mozilla.org/en-US/docs/Web/CSS/top)/[`right`](https://developer.mozilla.org/en-US/docs/Web/CSS/right)/[`bottom`](https://developer.mozilla.org/en-US/docs/Web/CSS/bottom)/[`left`](https://developer.mozilla.org/en-US/docs/Web/CSS/left)

浮动布局相关：

- [`float`](https://developer.mozilla.org/en-US/docs/Web/CSS/float)：设置浮动。
- [`clear`](https://developer.mozilla.org/en-US/docs/Web/CSS/clear)：清除浮动。
- [`shape-image-threshold`](https://developer.mozilla.org/en-US/docs/Web/CSS/shape-image-threshold)/[`shape-margin`](https://developer.mozilla.org/en-US/docs/Web/CSS/shape-margin)/[`shape-outside`](https://developer.mozilla.org/en-US/docs/Web/CSS/shape-outside)：设置浮动元素的占位区形状。

列布局相关：

> 这个列布局收录还有缺陷。

- `column-count`
- `column-width`
- `column-gap`
- [`column-rule`](https://developer.mozilla.org/en-US/docs/Web/CSS/column-rule)
- [`columns`](https://developer.mozilla.org/en-US/docs/Web/CSS/columns)

弹性布局相关：

- [`flex-flow`](https://developer.mozilla.org/en-US/docs/Web/CSS/flex-flow)：[`flex-direction`](https://developer.mozilla.org/en-US/docs/Web/CSS/flex-direction)和[`flex-wrap`](https://developer.mozilla.org/en-US/docs/Web/CSS/flex-wrap)2个弹性容器属性的简写。
- [`flex`](https://developer.mozilla.org/en-US/docs/Web/CSS/flex)：[`flex-grow`](https://developer.mozilla.org/en-US/docs/Web/CSS/flex-grow)，[`flex-shrink`](https://developer.mozilla.org/en-US/docs/Web/CSS/flex-shrink)和[`flex-basis`](https://developer.mozilla.org/en-US/docs/Web/CSS/flex-basis)3个弹性项属性的简写。
- [`justify-content`](https://developer.mozilla.org/en-US/docs/Web/CSS/justify-content)/[`justify-items`](https://developer.mozilla.org/en-US/docs/Web/CSS/justify-items)/[`justify-self`](https://developer.mozilla.org/en-US/docs/Web/CSS/justify-self)：主轴对齐方式。
- [`align-content`](https://developer.mozilla.org/en-US/docs/Web/CSS/align-content)/[`align-items`](https://developer.mozilla.org/en-US/docs/Web/CSS/align-items)/[`align-self`](https://developer.mozilla.org/en-US/docs/Web/CSS/align-self)：交叉轴对齐方式。
- [`order`](https://developer.mozilla.org/en-US/docs/Web/CSS/order)：顺序权重。

网格布局相关：

> 这个网格布局收录还有缺陷。

> `justify-items`，`align-items`和`order`属性是Flex和Grid系统通用的。

- [`grid`](https://developer.mozilla.org/en-US/docs/Web/CSS/grid)：[`grid-template-rows`](https://developer.mozilla.org/en-US/docs/Web/CSS/grid-template-rows)，[`grid-template-columns`](https://developer.mozilla.org/en-US/docs/Web/CSS/grid-template-columns)，[`grid-template-areas`](https://developer.mozilla.org/en-US/docs/Web/CSS/grid-template-areas)，[`grid-auto-rows`](https://developer.mozilla.org/en-US/docs/Web/CSS/grid-auto-rows)，[`grid-auto-columns`](https://developer.mozilla.org/en-US/docs/Web/CSS/grid-auto-columns)和[`grid-auto-flow`](https://developer.mozilla.org/en-US/docs/Web/CSS/grid-auto-flow)6个网格容器属性的简写。
- [`grid-area`](https://developer.mozilla.org/en-US/docs/Web/CSS/grid-area)：[`grid-row-start`](https://developer.mozilla.org/en-US/docs/Web/CSS/grid-row-start)，[`grid-column-start`](https://developer.mozilla.org/en-US/docs/Web/CSS/grid-column-start)，[`grid-row-end`](https://developer.mozilla.org/en-US/docs/Web/CSS/grid-row-end)和[`grid-column-end`](https://developer.mozilla.org/en-US/docs/Web/CSS/grid-column-end)4个网格项属性的简写，用于向指定容器区域分配网格项。
- [`grid-gap`](https://developer.mozilla.org/en-US/docs/Web/CSS/grid-gap)：[`grid-row-gap`](https://developer.mozilla.org/en-US/docs/Web/CSS/grid-row-gap)和[`grid-column-gap`](https://developer.mozilla.org/en-US/docs/Web/CSS/grid-column-gap)2个网格间距属性的简写。
- [`place-content`](https://developer.mozilla.org/en-US/docs/Web/CSS/place-content)/[`place-items`](https://developer.mozilla.org/en-US/docs/Web/CSS/place-items)/[`place-self`](https://developer.mozilla.org/en-US/docs/Web/CSS/place-self)：`justify-*`和`align-*`族属性在网格系统中的简写。

### 2. Box组

- [`box-sizing`](https://developer.mozilla.org/en-US/docs/Web/CSS/box-sizing)
- [`box-decoration-break`](https://developer.mozilla.org/en-US/docs/Web/CSS/box-decoration-break)
- [`box-shadow`](https://developer.mozilla.org/en-US/docs/Web/CSS/box-shadow)
- [`margin`](https://developer.mozilla.org/en-US/docs/Web/CSS/margin)：[`margin-top`](https://developer.mozilla.org/en-US/docs/Web/CSS/margin-top)，[`margin-right`](https://developer.mozilla.org/en-US/docs/Web/CSS/margin-right)，[`margin-bottom`](https://developer.mozilla.org/en-US/docs/Web/CSS/margin-bottom)和[`margin-left`](https://developer.mozilla.org/en-US/docs/Web/CSS/margin-left)4个外边距属性的简写。
- [`padding`](https://developer.mozilla.org/en-US/docs/Web/CSS/padding)：[`padding-top`](https://developer.mozilla.org/en-US/docs/Web/CSS/padding-top)，[`padding-right`](https://developer.mozilla.org/en-US/docs/Web/CSS/padding-right)，[`padding-bottom`](https://developer.mozilla.org/en-US/docs/Web/CSS/padding-bottom)和[`padding-left`](https://developer.mozilla.org/en-US/docs/Web/CSS/padding-left)4个内边距属性的简写。
- [`width`](https://developer.mozilla.org/en-US/docs/Web/CSS/width)/[`height`](https://developer.mozilla.org/en-US/docs/Web/CSS/height)
- [`min-width`](https://developer.mozilla.org/en-US/docs/Web/CSS/min-width)/[`min-height`](https://developer.mozilla.org/en-US/docs/Web/CSS/min-height)
- [`max-width`](https://developer.mozilla.org/en-US/docs/Web/CSS/max-width)/[`max-height`](https://developer.mozilla.org/en-US/docs/Web/CSS/max-height)

溢出相关：

- [`overflow`](https://developer.mozilla.org/en-US/docs/Web/CSS/overflow)：[`overflow-x`](https://developer.mozilla.org/en-US/docs/Web/CSS/overflow-x)和[`overflow-y`](https://developer.mozilla.org/en-US/docs/Web/CSS/overflow-y)2个溢出属性的简写。


### 3. Border组

- [`border`](https://developer.mozilla.org/en-US/docs/Web/CSS/border)：[`border-width`](https://developer.mozilla.org/en-US/docs/Web/CSS/border-width)，[`border-style`](https://developer.mozilla.org/en-US/docs/Web/CSS/border-style)和[`border-color`](https://developer.mozilla.org/en-US/docs/Web/CSS/border-color)3个边框属性的简写。
- [`border-radius`](https://developer.mozilla.org/en-US/docs/Web/CSS/border-radius)
- [`border-image`](https://developer.mozilla.org/en-US/docs/Web/CSS/border-image)

### 4. Background组

- [`background`](https://developer.mozilla.org/en-US/docs/Web/CSS/background)：[`background-color`](https://developer.mozilla.org/en-US/docs/Web/CSS/background-color)，[`background-image`](https://developer.mozilla.org/en-US/docs/Web/CSS/background-image)，[`background-position`](https://developer.mozilla.org/en-US/docs/Web/CSS/background-position)，[`background-size`](https://developer.mozilla.org/en-US/docs/Web/CSS/background-size)，[`background-repeat`](https://developer.mozilla.org/en-US/docs/Web/CSS/background-repeat)，[`background-origin`](https://developer.mozilla.org/en-US/docs/Web/CSS/background-origin)，[`background-clip`](https://developer.mozilla.org/en-US/docs/Web/CSS/background-clip)和[`background-attachment`](https://developer.mozilla.org/en-US/docs/Web/CSS/background-attachment)8个背景属性的简写。
- [`background-blend-mode`](https://developer.mozilla.org/en-US/docs/Web/CSS/background-blend-mode)：背景层之间的混合模式。

### 5. Font组

- [`font`](https://developer.mozilla.org/en-US/docs/Web/CSS/font)：[`font-style`](https://developer.mozilla.org/en-US/docs/Web/CSS/font-style)，[`font-variant`](https://developer.mozilla.org/en-US/docs/Web/CSS/font-variant)，[`font-weight`](https://developer.mozilla.org/en-US/docs/Web/CSS/font-weight)，[`font-stretch`](https://developer.mozilla.org/en-US/docs/Web/CSS/font-stretch)，[`font-size`](https://developer.mozilla.org/en-US/docs/Web/CSS/font-size)，[`line-height`](https://developer.mozilla.org/en-US/docs/Web/CSS/line-height)和[`font-family`](https://developer.mozilla.org/en-US/docs/Web/CSS/font-family)7个字体属性的简写。
- [`font-feature-settings`](https://developer.mozilla.org/en-US/docs/Web/CSS/font-feature-settings)
- [`font-kerning`](https://developer.mozilla.org/en-US/docs/Web/CSS/font-kerning)
- [`font-synthesis`](https://developer.mozilla.org/en-US/docs/Web/CSS/font-synthesis)：[`font-synthesis-weight`](https://developer.mozilla.org/en-US/docs/Web/CSS/font-synthesis-weight)，[`font-synthesis-style`](https://developer.mozilla.org/en-US/docs/Web/CSS/font-synthesis-style)，[`font-synthesis-small-caps`](https://developer.mozilla.org/en-US/docs/Web/CSS/font-synthesis-small-caps)和[`font-synthesis-position`](https://developer.mozilla.org/en-US/docs/Web/CSS/font-synthesis-position)4个字体合成属性的简写，当目标字体缺少诸如粗体或者大小写字体时由浏览器合成这些字体。该属性于2022年完成主流浏览器支持。
- [`font-size-adjust`](https://developer.mozilla.org/en-US/docs/Web/CSS/font-size-adjust)：调整大小写字体的尺寸。

> 这里的一些属性其实非常新，可见在新标准中，**文本**依旧是布局的重点。

### 6. Text组

- [`color`](https://developer.mozilla.org/en-US/docs/Web/CSS/color)

文本对齐相关：

- [`text-align`](https://developer.mozilla.org/en-US/docs/Web/CSS/text-align)
- [`text-align-last`](https://developer.mozilla.org/en-US/docs/Web/CSS/text-align-last)
- [`direction`](https://developer.mozilla.org/en-US/docs/Web/CSS/direction)
- [`unicode-bidi`](https://developer.mozilla.org/en-US/docs/Web/CSS/unicode-bidi)
- `text-combine-upright`
- [`text-orientation`](https://developer.mozilla.org/en-US/docs/Web/CSS/text-orientation)
- [`vertical-align`](https://developer.mozilla.org/en-US/docs/Web/CSS/vertical-align)

文本修饰相关：

- [`text-decoration`](https://developer.mozilla.org/en-US/docs/Web/CSS/text-decoration)：`text-decoration-line`，`text-decoration-color`，`text-decoration-style`和`text-decoration-thickness`4个文本修饰属性的简写。

文本转换相关：

- [`text-transform`](https://developer.mozilla.org/en-US/docs/Web/CSS/text-transform)

文本间距相关：

- [`text-indent`](https://developer.mozilla.org/en-US/docs/Web/CSS/text-indent)
- [`letter-spacing`](https://developer.mozilla.org/en-US/docs/Web/CSS/letter-spacing)
- [`word-spacing`](https://developer.mozilla.org/en-US/docs/Web/CSS/word-spacing)
- [`word-break`](https://developer.mozilla.org/en-US/docs/Web/CSS/word-break)
- [`white-space`](https://developer.mozilla.org/en-US/docs/Web/CSS/white-space)

文本阴影相关：

- [`text-shadow`](https://developer.mozilla.org/en-US/docs/Web/CSS/text-shadow)

文本溢出相关：

- `text-overflow`

文本渲染相关：

- [`text-rendering`](https://developer.mozilla.org/en-US/docs/Web/CSS/text-rendering)

文化换行相关：

- [`hyphens`](https://developer.mozilla.org/en-US/docs/Web/CSS/hyphens)：连字符。
- [`line-break`](https://developer.mozilla.org/en-US/docs/Web/CSS/line-break)：换行。
- [`overflow-wrap`](https://developer.mozilla.org/en-US/docs/Web/CSS/overflow-wrap)：控制换行溢出。

制表符长度：

- [`tab-size`](https://developer.mozilla.org/en-US/docs/Web/CSS/tab-size)

### 7. Content组

- [`content`](https://developer.mozilla.org/en-US/docs/Web/CSS/content)
- [`quotes`](https://developer.mozilla.org/en-US/docs/Web/CSS/quotes)
- [`counter-increment`](https://developer.mozilla.org/en-US/docs/Web/CSS/counter-increment)/[`counter-reset`](https://developer.mozilla.org/en-US/docs/Web/CSS/counter-reset)/[`counter-set`](https://developer.mozilla.org/en-US/docs/Web/CSS/counter-set)

### 8. List组

- [`list-style`](https://developer.mozilla.org/en-US/docs/Web/CSS/list-style)：[`list-style-image`](https://developer.mozilla.org/en-US/docs/Web/CSS/list-style-image)，[`list-style-position`](https://developer.mozilla.org/en-US/docs/Web/CSS/list-style-position)和[`list-style-type`](https://developer.mozilla.org/en-US/docs/Web/CSS/list-style-type)3个列表属性的简写。

### 9. Table组

- [`table-layout`](https://developer.mozilla.org/en-US/docs/Web/CSS/table-layout)
- [`caption-side`](https://developer.mozilla.org/en-US/docs/Web/CSS/caption-side)
- [`empty-cells`](https://developer.mozilla.org/en-US/docs/Web/CSS/empty-cells)
- [`border-collapse`](https://developer.mozilla.org/en-US/docs/Web/CSS/border-collapse)
- [`border-spacing`](https://developer.mozilla.org/en-US/docs/Web/CSS/border-spacing)

### 10. Animation组

- [`animation`](https://developer.mozilla.org/en-US/docs/Web/CSS/animation)：[`animation-name`](https://developer.mozilla.org/en-US/docs/Web/CSS/animation-name)，[`animation-duration`](https://developer.mozilla.org/en-US/docs/Web/CSS/animation-duration)，[`animation-timing-function`](https://developer.mozilla.org/en-US/docs/Web/CSS/animation-timing-function)，[`animation-delay`](https://developer.mozilla.org/en-US/docs/Web/CSS/animation-delay)，[`animation-iteration-count`](https://developer.mozilla.org/en-US/docs/Web/CSS/animation-iteration-count)，[`animation-direction`](https://developer.mozilla.org/en-US/docs/Web/CSS/animation-direction)，[`animation-fill-mode`](https://developer.mozilla.org/en-US/docs/Web/CSS/animation-fill-mode)和[`animation-play-state`](https://developer.mozilla.org/en-US/docs/Web/CSS/animation-play-state)8个动画属性的简写，其中`animation-name`是由`@keyframes`指定的关键帧名称，且无视属性值顺序（但习惯上放在首位）。

### 11. Transition组

- [`transition`](https://developer.mozilla.org/en-US/docs/Web/CSS/transition)：[`transition-property`](https://developer.mozilla.org/en-US/docs/Web/CSS/transition-property)，[`transition-duration`](https://developer.mozilla.org/en-US/docs/Web/CSS/transition-duration)，[`transition-timing-function`](https://developer.mozilla.org/en-US/docs/Web/CSS/transition-timing-function)和[`transition-delay`](https://developer.mozilla.org/en-US/docs/Web/CSS/transition-delay)4个过渡属性的简写。

### 12. Transform组

- [`transform`](https://developer.mozilla.org/en-US/docs/Web/CSS/transform)
- [`transform-origin`](https://developer.mozilla.org/en-US/docs/Web/CSS/transform-origin)
- [`transform-style`](https://developer.mozilla.org/en-US/docs/Web/CSS/transform-style)

- [`backface-visibility`](https://developer.mozilla.org/en-US/docs/Web/CSS/backface-visibility)：可变换元素的背面可见性。
- [`perspective`](https://developer.mozilla.org/en-US/docs/Web/CSS/perspective)
- [`perspective-origin`](https://developer.mozilla.org/en-US/docs/Web/CSS/perspective-origin)

### 13. Appearance组

- [`outline`](https://developer.mozilla.org/en-US/docs/Web/CSS/outline)：[`outline-width`](https://developer.mozilla.org/en-US/docs/Web/CSS/outline-width)，[`outline-style`](https://developer.mozilla.org/en-US/docs/Web/CSS/outline-style)和[`outline-color`](https://developer.mozilla.org/en-US/docs/Web/CSS/outline-color)3个轮廓属性的简写。
- [`outline-offset`](https://developer.mozilla.org/en-US/docs/Web/CSS/outline-offset)：设置轮廓偏移距离。

### 14. Page组

- [`widows`](https://developer.mozilla.org/en-US/docs/Web/CSS/widows)
- [`orphans`](https://developer.mozilla.org/en-US/docs/Web/CSS/orphans)：孤行。
- [`page`](https://developer.mozilla.org/en-US/docs/Web/CSS/page)
- [`page-break-after`](https://developer.mozilla.org/en-US/docs/Web/CSS/page-break-after)：[`break-after`](https://developer.mozilla.org/en-US/docs/Web/CSS/break-after)属性的别名。
- [`page-break-before`](https://developer.mozilla.org/en-US/docs/Web/CSS/page-break-before)：[`break-before`](https://developer.mozilla.org/en-US/docs/Web/CSS/break-before)属性的别名。
- [`page-break-inside`](https://developer.mozilla.org/en-US/docs/Web/CSS/page-break-inside)：[`break-inside`](https://developer.mozilla.org/en-US/docs/Web/CSS/break-inside)属性的别名。

### 15. Layer组/SVG组/Shape组/Mask组

- [`shape-rendering`](https://developer.mozilla.org/en-US/docs/Web/CSS/shape-rendering)
- [`clip-path`](https://developer.mozilla.org/en-US/docs/Web/CSS/clip-path)
- [`clip-rule`](https://developer.mozilla.org/en-US/docs/Web/CSS/clip-rule)

- [`filter`](https://developer.mozilla.org/en-US/docs/Web/CSS/filter)

混合模式相关：

- [`mix-blend-mode`](https://developer.mozilla.org/en-US/docs/Web/CSS/mix-blend-mode)

蒙版和遮罩相关：

- [`mask`](https://developer.mozilla.org/en-US/docs/Web/CSS/mask)：[`mask-image`](https://developer.mozilla.org/en-US/docs/Web/CSS/mask-image)，[`mask-position`](https://developer.mozilla.org/en-US/docs/Web/CSS/mask-position)，[`mask-size`](https://developer.mozilla.org/en-US/docs/Web/CSS/mask-size)，[`mask-repeat`](https://developer.mozilla.org/en-US/docs/Web/CSS/mask-repeat)，[`mask-clip`](https://developer.mozilla.org/en-US/docs/Web/CSS/mask-clip)，[`mask-origin`](https://developer.mozilla.org/en-US/docs/Web/CSS/mask-origin)，[`mask-composite`](https://developer.mozilla.org/en-US/docs/Web/CSS/mask-composite)和[`mask-mode`](https://developer.mozilla.org/en-US/docs/Web/CSS/mask-mode)8个遮罩属性的简写。
- [`mask-type`](https://developer.mozilla.org/en-US/docs/Web/CSS/mask-type)

### 16. Stack组

- [`isolation`](https://developer.mozilla.org/en-US/docs/Web/CSS/isolation)

### 17. Others组

- [`z-index`](https://developer.mozilla.org/en-US/docs/Web/CSS/z-index)
- [`opacity`](https://developer.mozilla.org/en-US/docs/Web/CSS/opacity)
- `pointer-events`
- `user-select`
- [`all`](https://developer.mozilla.org/en-US/docs/Web/CSS/all)
- [`cursor`](https://developer.mozilla.org/en-US/docs/Web/CSS/cursor)
- [`resize`](https://developer.mozilla.org/en-US/docs/Web/CSS/resize)
- [`writing-mode`](https://developer.mozilla.org/en-US/docs/Web/CSS/writing-mode)

### 18. Image组

- [`object-fit`](https://developer.mozilla.org/en-US/docs/Web/CSS/object-fit)
- [`object-position`](https://developer.mozilla.org/en-US/docs/Web/CSS/object-position)

