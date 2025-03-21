# Tool Learning Log

## Tool: **Flexbox**

---

### 3/6/25:
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

insert image here later

### 3/17/25:
* I learned how to use the `flex-shrink` property.
  * Flex shrink is like `flex-grow` and needs a number value
    * Unlike flex grow, flex items will shrink with this property.
  * The default value for `flex-shrink` is set to 1.




### X/X/XX:
* Text



