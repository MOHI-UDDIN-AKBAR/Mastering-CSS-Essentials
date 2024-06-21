# CSS Documentation

## Introduction to CSS

CSS (Cascading Style Sheets) is a stylesheet language used to describe the presentation of HTML or XML documents. There are three primary ways to apply CSS:

### Inline CSS

- **Definition**: CSS rules within the `style` attribute of an HTML element.
- **Example**: `<p style="color: red;">This is a paragraph.</p>`

### Internal CSS

- **Definition**: CSS rules within `<style>` tags in the `<head>` section of an HTML document.
- **Example**:
  ```html
  <head>
    <style>
      body {
        background-color: lightblue;
      }
    </style>
  </head>
  ```

### External CSS

- **Definition**: CSS rules in a separate `.css` file linked to an HTML document using `<link>` tag.
- **Example**:
  ```html
  <head>
    <link rel="stylesheet" type="text/css" href="styles.css" />
  </head>
  ```

## Using Classes and IDs in CSS

- **Classes**: Defined with a dot (`.`) prefix and applied to multiple elements.
- **IDs**: Defined with a hash (`#`) prefix and unique per page.
- **Examples**:

  ```html
  <div class="container">Content</div>
  <input type="text" id="username" />
  ```

  ```css
  .container {
    color: red;
  }
  #username {
    padding: 0.4rem;
  }
  ```

## Font Styles in CSS

- **Font Family**: `font-family: 'Courier New', Courier, monospace;`
- **Font Size**: `font-size: 16px;`
- **Font Weight**: `font-weight: bold;`
- **Font Style**: `font-style: italic;`

## Color in CSS

There are six ways to specify colors in CSS:

1. By color name: `color: red;`
2. By hexadecimal value: `color: #1f2633;`
3. By RGB value: `color: rgb(23, 39, 51);`
4. By RGBA value: `color: rgba(23, 39, 51, 0.5);`
5. By HSL value: `color: hsl(240, 80%, 15%);`
6. By HSLA value: `color: hsla(240, 80%, 15%, 0.5);`

## Text Style in CSS

- **Text Alignment**: `text-align: left;`, `right;`, `center;`, `justify;`
- **Text Decoration**: `text-decoration: underline;`, `overline;`, `line-through;`, `none;`
- **Text Indent**: `text-indent: -5px;` or `5px;`
- **Text Transform**: `text-transform: uppercase;`, `lowercase;`, `capitalize;`
- **Text Shadow**: `text-shadow: 0px 0px 2px blue;`
- **Line Height**: `line-height: 20px;`
- **Word Spacing**: `word-spacing: 10px;`
- **Letter Spacing**: `letter-spacing: 12px;`
- **Word Wrap**: `word-wrap: normal;`

## Box Model Properties

### Float

- **Float**: `float: left;`, `right;`

### Clear

- **Clear**: `clear: left;`, `right;`, `both;`

### Margin

- **Margin**: `margin-left: 5px;`, `margin-right: 5px;`, `margin-top: 5px;`, `margin-bottom: 5px;`, `margin: 5px;`, `margin: 0px 5px;`

### Padding

- **Padding**: `padding-left: 5px;`, `padding-right: 5px;`, `padding-top: 5px;`, `padding-bottom: 5px;`, `padding: 5px;`, `padding: 0px 5px;`

### Border

- **Border**: `border-width: 5px;`, `border-style: solid;`, `border-color: green;`, `border: 5px solid green;`

### Outline

- **Outline**: `outline-width: 5px;`, `outline-style: solid;`, `outline-color: green;`, `outline: 5px solid green;`

### Outline Offset

- **Outline Offset**: `outline-offset: 10px;`

## Background and Gradients

- **Background**: `background-color: red;`, `background-image: url("image.jpg");`, `background-repeat: repeat;`, `no-repeat;`, `repeat-x;`, `repeat-y;`, `background-position: top;`, `left;`, `right;`, `bottom;`, `center;`, `%`, `px`, `rem;`, `background-size: cover;`, `contain;`, `50% 20%;`, `200px 100px;`, `auto;`, `background-clip: border-box;`, `padding-box;`, `content-box;`, `text;`, `background-attachment: scroll;`, `fixed;`, `local;`

- **Linear Gradient**: `background: linear-gradient(to right, red, blue);`, `background: linear-gradient(45deg, red, blue);`

- **Radial Gradient**: `background: radial-gradient(circle, blue, red);`

- **Conic Gradient**: `background: conic-gradient(red, blue, green);`, `background: conic-gradient(red 90deg, yellow 50deg, blue);`

- **Repeating Gradient**: `background: repeating-gradient(red, blue 10px, gold 50px);`, `background: repeating-gradient(circle 10px, red, blue 50px);`

## Columns and Shadows

- **Columns**: `column-count: 3;`, `column-fill: balance;`, `auto;`, `column-gap: 10px;`, `column-rule: 2px solid red;`, `column-span: all;`, `none;`, `column-width: px;`, `%`, `rem;`

- **Shadows**: `text-shadow: 0px 0px 2px 2px red;`, `box-shadow: 0px 0px 2px 2px red;`, `0px 0px 2px 2px red, 2px 0px 2px 2px red, 0px 2px 2px 2px red;`

## Transforms

- **Transform**: `transform: translate(10px, 20px);`, `translateX(10px);`, `translateY(20px);`, `scale(1.2);`, `scaleX(1.2);`, `scaleY(1.2);`, `rotateX(90deg);`, `rotateY(90deg);`, `rotateZ(90deg);`, `skew(20deg, 20deg);`, `skewX(20deg);`, `skewY(20deg);`, `transform-style: preserve-3d;`, `perspective: 100px;`, `perspective-origin: right;`, `left;`

## Resizing Elements

- **Resize**: `resize: horizontal;`, `vertical;`, `both;`, `none;`

## Transitions and Animations

- **Transition**: `transition-property: width;`, `height;`, `transition-delay: 3s;`, `transition-duration: 2s;`, `transition-timing-function: linear;`, `ease-in;`, `ease-out;`, `ease-in-out;`, `cubic-bezier(0.25, 0.1, 0, 25, 1);`, `transition: width 0.3s linear;`

- **Animation**: `animation-name: slideIn;`, `animation-delay: 3s;`, `animation-duration: 2s;`, `animation-timing-function: linear;`, `ease-in;`, `ease-out;`, `ease-in-out;`, `cubic-bezier(0.25, 0.1, 0, 25, 1);`, `animation-iteration-count: infinite;`, `animation-play-state: paused;`, `running;`, `animation-fill-mode: none;`, `forward;`, `backward;`, `both;`, `animation-direction: normal;`, `reverse;`, `alternate;`, `alternate-reverse;`

## Filters

- **Filter**: `filter: blur(2px);`, `brightness(200%);`, `drop-shadow(0px 0px 2px red);`, `grayscale(100%);`, `opacity(20%);`, `none`

## Display and Visibility

- **Display**: `display: inline;`, `block;`, `inline-block;`, `flex;`, `inline-flex;`, `grid;`, `inline-grid;`, `none;`

- **Visibility**: `visibility: hidden;`, `visible;`

## Flexbox

- **Flex Direction**: `flex-direction: row;`, `row-reverse;`, `column;`, `column-reverse;`

- **Wrap**: `flex-wrap: wrap;`, `nowrap;`, `wrap-reverse;`

- **Grow**: `flex-grow: 1;`, `2;`, `any number;`

- **Basis**: `flex-basis:`, ` %`, `px;`, `rem;`

- **Shrink**: `flex-shrink: 1;`, `2;`, `any number;`

- **Justify Content**: `justify-content: flex-start;`, `center;`, `space-around;`, `space-between;`

- **Align Items**: `align-items: flex-start;`, `center;`, `baseline;`, `stretch;`

- **Align Content**: `align-content: flex-start;`, `center;`, `space-around;`, `space-between;`

## Grid

- **Grid Container**: `display: grid;`, `inline-grid;`

- **Grid Columns**: `grid-template-columns: 1fr 1fr 1fr;`, `2fr 1fr;`, `auto;`, `10% 20%;`, `px;`, `rem;`

- **Grid Rows**: `grid-template-rows: 100px 200px 300px;`, `50% 100%;`, `auto;`, `px;`, `rem;`

- **Grid Gaps**: `grid-column-gap: 10px;`, `grid-row-gap: 10px;`, `gap: 10px;`, `0px 10px;`

- **Grid Lines**: `grid-column-start: 1;`, `grid-column-end: 3;`, `span 3;`, `auto;`, `1;`, `grid-row-start: 1;`, `grid-row-end: 3;`, `span 3;`, `auto;`, `1;`

- **Grid Areas**: `grid-template-areas: "header header header" "content content sidebar" "footer footer footer";`

- **Align Self**: `align-self: flex-start;`, `center;`, `baseline;`, `stretch;`

---

## Pseudo-classes and Pseudo-elements

### Input Pseudo-class

- `:autofill`, `:enabled`, `:disabled`, `:read-only`, `:read-write`, `:placeholder-shown`, `:checked`, `:interminate`, `:valid`, `:invalid`, `:required`, `:optional`, `:in-range`, `:out-of-range`

### Linguistic Pseudo-class

- `:dir(ltr,rtl)`, `:lang(en-us)`

### Location Pseudo-class

- `:link`, `:visited`, `:target`

### Tree Structure Pseudo-class

- `:root`, `:empty`, `:first-child`, `:last-child`, `:nth-child(n)`, `:nth-last-child(n)`, `:only-child`, `:first-of-type`, `:last-of-type`, `:nth-of-type()`, `:nth-last-of-type()`, `:only-of-type`

### User Action Pseudo-class

- `:hover`, `:action`, `:focus`

### Functional Pseudo-class

- `:not()`, `:is()`, `:where()`, `:has()`

### Pseudo-elements

- `::first-line`, `::first-letter`, `::after`, `::before`, `::cue`, `::placeholder`, `::selection`

---

## Positioning

- **Position**: `position: static;`, `relative;`, `absolute;`, `fixed;`, `sticky;`

- **Top**: `top: 50px;`, `px;`, `%;`, `auto;`

- **Right**: `right: 50px;`, `px;`, `%;`, `auto;`

- **Bottom**: `bottom: 50px;`, `px;`, `%;`, `auto;`

- **Left**: `left: 50px;`, `px;`, `%;`, `auto;`

## Responsive Design

- **Media Queries**: `@media (max-width: 768px) { }`, `min-width;`, `max-height;`, `orientation;`

- **Viewport**: `@viewport { width: 360px; height: 640px; }`, `min-width;`, `max-height;`

## Accessibility

- **Tab Index**: `tabindex="1";`, `2;`, `any number;`

- **Keyboard Navigation**: `:focus;`, `active;`, `hover;`

- **Screen Reader**: `aria-labelledby;`, `describedby;`, `hidden;`

## CSS Variables

- **Variable**: `--mycolor: blue;`, `white;`, `border;`

- **Usage**: `color: var(--mycolor);`, `background: var(--mycolor);`

## Conclusion

CSS is a powerful tool for designing web pages, offering numerous properties and techniques for styling elements. Mastering CSS enables developers to create visually appealing and responsive web interfaces.
