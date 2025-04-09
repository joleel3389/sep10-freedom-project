
# Tool Learning Log

## Tool: **Flexbox**

---

### 3/3/25:
* I learned how to use the `justify-content` property.
    * Variables I can use with this property are `center`, `flex-start`, `flex-end`, `space-around`, `space-between`, and `space-evenly`.
        * I used the value `space-evenly`, so my elements under my **buttons** class would be equidistant from each other.
* I learned how to use the `flex-direction` property.
    * Variables used with this property are `row`, `column`, `row-reverse`, and `column-reverse`.
        * I used the `row` value to have my elements displayed horizontally, but not in reversed order.

This is my CSS that shows my tinkering.
```css
.buttons {
    display: flex;
    flex-direction: row;
    justify-content: space-evenly;
    margin: auto;
    width: 80%;
    padding-top: 7px;
}
```

### 3/10/25:
* I learned how to use the `flex-grow` property.
    * Flex grow has a value, where you can input a number value.
    * The default value for `flex-grow` is set to 0.

This is my HTML with inline CSS that shows my tinkering.
```html
  <div class="container">
    <div class="mini" style="flex-grow: 1;">1</div>
    <div class="mini" style="flex-grow: 5">2</div>
    <div class="mini" style="flex-grow: 1">3</div>
  </div>
```

The second div will come out to be 5 times bigger than the others, since the value of flex grow is 5, while the rest is 1. The following outcome image shows that div 2 is clearly 5 times bigger.

![Screenshot 2025-03-10 2 21 36 PM](https://github.com/user-attachments/assets/fe3e596a-40fd-4823-82e2-4733b4d505af)

### 3/17/25:
* I learned how to use the `flex-shrink` property.
  * Flex shrink is like `flex-grow` and needs a number value
    * Unlike flex grow, flex items will shrink with this property.
  * The default value for `flex-shrink` is set to 1.

The following HTML with inline CSS code shows my tinkering.
```html
  <div class="flex-container">
    <div class="mini">1</div>
    <div class="mini" style="flex-shrink: 2">2</div>
    <div class="mini">3</div>
    <div class="mini">4</div>
    <div class="mini">5</div>
    <div class="mini">6</div>
    <div class="mini">7</div>
    <div class="mini">8</div>
    <div class="mini">9<div>
  </div>
```

The second div will shrink compared to the rest by 2, like shown in the image below.

![2025-03-21 16_07_47-Window](https://github.com/user-attachments/assets/7ea32164-6754-43bd-8ad7-b867adc16393)

### 3/24/25:
* I learned how to use the `flex-basis` property.
  * Flex basis allows you to set a length for your flex item.
    * For instance, if you want your flex item to have a length of 100px, set the value of `flex-basis` to 100px.

The following HTML shows how I tinkered with the `flex-basis` property.
```html
<div class="flex-container">
  <div>1</div>
  <div style="flex-basis: 100px;">2</div>
  <div>3</div>
</div>
```

Compared to the other divs, div #2 will be set to have a width of 100 pixels, while the others are set to the default like shown below.

![Screenshot 2025-03-27 1 50 16 PM](https://github.com/user-attachments/assets/096650c9-8240-424c-8265-5d6f19a1e310)

* I learned about the `flex` property.
  * The flex property combines the previous 3 flex properties, which are `flex-grow`, `flex-shrink`, and `flex-basis`.
    * The values when using the `flex` property will go in the corresponding order as well (grow, shrink, then basis).

The following HTML shows how I tinkered with the `flex` property.
```html
<div class="flex-container">
  <div style="flex: 2 0 0px">1</div>
  <div style="flex: 0 0 10px;">2</div>
  <div style="flex: 0 0 20px;">3</div>
</div>
```
Div #1 will grow 2 times greater than the other two divs which have a set width of 10px (div #2) and 20px (div #3). However, none of the divs are shrinkable, divs #2 and #3 are not growable, and div #1 does not have a set width as shown.

![Screenshot 2025-03-27 2 05 43 PM](https://github.com/user-attachments/assets/600f74c8-d795-44c5-ab2c-99b3ef25ce76)

### 4/1/25:
* I learned about the `align-self` property.
  * The `align-self` allows you to change the alignment of one particular flex-item
  * The value set for the `align-self` property will be prioritized over the value you have set for the `align-items` property.
  * Possible values include center, flex-start, and flex-end for instance.

The following HTML shows how I tinkered with the `align-self` property.
```html
<div class="flex-container">
  <div style="align-self: center">1</div>
  <div style="align-self: flex-start">2</div>
  <div style="align-self: flex-end">3</div>
</div>
```

The first div will be positioned to the center, the second div to the top, and the third div to the bottom of the container shown in the image below.

![2025-04-06 16_18_43-Window](https://github.com/user-attachments/assets/0634755e-731f-4b29-82bb-567533eb7d21)

### 4/7/25:
* I learned the `order` property that's used with flex items.
  * The `order` property is used to reorder any existing flex items.
  * The value you use for the `order` property must be a number value, with the default being 0, the most prioritized.
    * If you don't use any values that are less than the default ones, your order will stay the same, with first flex-item prioritized to be first.

For instance, the following code will still prioritize div #1 to be shown first, as a value of 1 in div #3 will not override that value for being greater.
```html
<div class="flex-container">
  <div>1</div>
  <div style="order: 2">2</div>
  <div style="order: 1">3</div>
</div>
```

![Screenshot 2025-04-07 2 24 13 PM](https://github.com/user-attachments/assets/049471a4-894e-42ed-94a0-a5f25cbdd05d)

Whileas in this code, the divs will be in the opposite order due to the value priority (lower values are prioritized first).
```html
<div class="flex-container">
  <div style="order: 3">1</div>
  <div style="order: 2">2</div>
  <div style="order: 1">3</div>
</div>
```

![2025-04-07 19_25_34-Window](https://github.com/user-attachments/assets/7884a534-764c-492c-a39a-f711c539e714)

### 4/8/25:
* I learned how to use the `flex-wrap` property.
  * Flex wrap has 3 values, `nowrap`, `wrap`, and `wrap-reverse`.
    * The value `nowrap` is meant to prevent your flex items from wrapping. This is also the default set value.
    * The `wrap` value allows your flex items to wrap if there is no more space on the screen.
    * The `wrap-reverse` will wrap your flex items, but in the reverse order.
* I learned how to use the `flex-flow` property.
  * The `flex-flow` property allows you to put the values for `flex-wrap` and `flex-direction` onto one line of code.

The following code and image shows the use of the `wrap-reverse` value belonging to `flex-wrap` and `row` value belonging to `flex-direction` in the `flex-flow` property.
```css
.flex-container {
  display: flex;
  border: 0px;
  background-color: transparent;
  height: 200px;
}
div {
  border: 2px blue solid;
  background-color: white;
  margin: auto;
  padding: 0px 40px 0px 40px;
  text-align: center;
  margin: 10px;
  align-self: center;
  flex-flow: row wrap-reverse;
}
```

![Screenshot 2025-04-08 1 58 00 PM](https://github.com/user-attachments/assets/94be6d11-bf48-4fbe-8cc3-4e40d2f27821)

The flex items will be in a row formation, but if wrapping is needed they'll wrap in the reverse order, starting from numbers 4 through 6 instead of 1 through 3 on the first row.

### 4/9/25:
* I learned the `align-content` property.
  * This property aligns along an invisible flex line.
  * Values used with this property are `center`, `stretch`, `flex-start`, `flex-end`, `space-around`, `space-between`, and `space-evenly`.
    * Works better when `flex-wrap` is set to wrap.

For instance, in this code the `flex-wrap` property is set to `wrap` in order to see and complement the `flex-end` value of `align-content`, which allows the container to be aligned to the bottom of the screen.
```css
.flex-container {
  display: flex;
  border: 0px;
  background-color: transparent;
 height: 600px;
  padding: 0px;

  align-content: flex-end;
  flex-wrap: wrap;
}
div {
  border: 2px blue solid;
  background-color: white;
  padding: 0px 40px 0px 40px;
  align-self: center;
  margin: 10px;
  text-align: center;
}
```

image

* I learned the `align-items` property.
  * The purpose of this property is similar to the `align-content` property except it's for aligning th flex items if there is space available still.
  * Values of this property are `center`, `flex-start`, `flex-end`, `stretch`, `baseline`, and `normal`.

The following screenshot shows that the`baseline` value aligns all flex items to the text baseline, no matter how big the font is.

image

### X/X/XX:
* Text
