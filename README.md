# Руководство по оформлению css-кода

Данное руководство содержит основные правила по оформлению кода, сформированные на основе личного опыта.

## Содержание
1. [Последовательность свойств](#1-Последовательность-свойств)

## 1) Последовательность свойств
## Сокращения

1. Директивы и локальные переменные - `@include`, `@extend` (для SCSS/SASS/LESS/Stylus/Postcss)
2. Размеры и отступы - `width`, `height`, `margin`, `padding`
3. Позиционирование и положение - `position`, `top/right/bottom/left`, `display`, `float`, `z-index`
4. Рамка - `border`
5. Оформление - `background`, `border-radius`, `outline`, `opacity`, `list-style-type`, `overflow`
6. Типографика и оформление текста - `font-style`, `font-variant`, `font-weight`, `font-size`, `line-height`, `font-family`, `color`
7. Прочее - `transition`, `animation`

__Пример:__
```css
.sequence {
  [@mixin|@include];

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

  transition: opacity .3s ease;
}
```
