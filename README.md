# Руководство по оформлению css-кода

Данное руководство содержит основные правила по оформлению кода, сформированные на основе личного опыта.

## Содержание
- [Последовательность свойств](#Последовательность-свойств]

## Последовательность свойств

0) @mixin, @include - если используем SCSS/SASS/LESS/Stylus/Postcss
1) Размеры и отступы - width, height, margin, padding
2) Позиционирование и положение - position, top/right/bottom/left, display, float, z-index
3) Рамка - border
4) Оформление - background, border-radius, outline, opacity, list-style-type, overflow
5) Типографика и оформление текста - font-style, font-variant, font-weight, font-size, line-height, font-family, color
6) Прочее - transition, animation

```css
.sequence {
    [@include|@mixin];

    width: 100px;
	height: 100px;
	margin: 0;
	padding: 10px;

	position: relative;
	top: 2px;
	left: 2px;
	display: block;
	z-index: 10;

	border: 1px solid;

	background-color: #eee;
	border-radius: 3px;
	box-sizing: border-box;
	list-style-type: disc;
	opacity: .9;
	overflow: visible;

    color: #000;
	font-style: italic;
	font-size: 12px;
	line-height: 100px;
	font-family: Arial, sans-serif;
	text-transform: uppercase;
}
```