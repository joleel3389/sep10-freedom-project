# Entry 5
##### 4/11/25

### Learning my tool for my freedom project

---

For entry 5, my task was to further learn more about the freedom project tool I chose (which was flexbox), to be able to use it/incorporate it in my actual freedom project later. For my tool, I got to learn all of the properties used with it, with some honorable mentions being `flex-flow`, `flex`, and `align-items` for instance. In the process of learning all the properties of flexbox, I used [W3Schools](https://www.w3schools.com/css/css3_flexbox.asp) to learn the properties, and [jsbin](https://jsbin.com) to tinker with and understand these properties.

For example, with the `flex-flow` property, this property has two values. One value belongs to `flex-wrap`, and the other to `flex-direction`. The purpose of the `flex-flow` property is to have both of the properties `flex-wrap` and `flex-direction` be used under one property; `flex-flow`. When writing the values for `flex-flow`, the direction goes first, and then if the item should wrap or not. I tinkered with it as shown in my code snippet and image output below.
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

This image & code snippet are meant to show how when I set the values to row and wrap-reverse, my flex items did indeed change to a row formation. If wrapping is needed they'll wrap in the reverse order, starting from numbers 4 through 6 instead of 1 through 3 on the first row.

Next is the `flex` property, which combines the following 3 flex properties; `flex-grow`, `flex-shrink`, and `flex-basis`. When adding values for `flex`, they'll go in the order of grow, shrink, then basis.

The following code snippets and image show how I tinkered with the `flex` property below.
```html
<div class="flex-container">
  <div style="flex: 2 0 0px">1</div>
  <div style="flex: 0 0 10px;">2</div>
  <div style="flex: 0 0 20px;">3</div>
</div>
```

![Screenshot 2025-03-27 2 05 43 PM](https://github.com/user-attachments/assets/600f74c8-d795-44c5-ab2c-99b3ef25ce76)

The code snippet and image both support the idea that div 1 will grow 2 times greater than the other two divs which have a set width of 10px (div 2) and 20px (div 3). However, none of the divs are shrinkable, due to all of them having a value of 0 for shrink. Additionally, divs 2 & 3 are not growable, and div 1 does not have a set width as shown.

The last honorable property I learned for flexbox is the `align-items` property which aligns flex items if there's space vertically. It's similar to the property `align-content`, but they align different things.

Here's an image to show how I tinkered with the `align-items` property.

![Screenshot 2025-04-09 2 17 00 PM](https://github.com/user-attachments/assets/6cff69bf-426d-4d5f-81ee-33c1539e6501)

In this particular case, the flex items in my flex container would be aligned to the baseline. The baseline has to do with the font sizes of my flex items, so my flex items would all be aligned no matter how big the font for each individual flex item was.

### Skills

---

Here are the following skills I learned from writing my 5th blog.

* Problem decomposition
    * My freedom project tool of flexbox did not have that many properties, but it still could have been hard to process all at once in one go. So in order to effectively learn my tool, I split this task into bits where I would learn 1-2 properties at a time. I also considered learning similar properties at the same time, which helped me recognize the difference in such similar properties easier than if I were to go back and analyze the difference.
* Time management
    * Assignments such as our learning log were made to help keep us on track and learn our freedom project tool in an effective amount of time. Learning logs were not posted on Google Classroom to remind us when to turn it in/push our changes, so I had to set reminders on my phone to ensure I didn't forget to push my changes to my learning log and to allow me to save time to do it. Managing my time to ensure I got my weekly learning logs done has helped me understand my tool better, and so time management was a skill I continued to master throughout my freedom project tool learning.

### Next steps

---

After learning my freedom project tool, I will create a wireframe for my freedom project (or create a prototype).

[Previous](entry04.md) | [Next](entry06.md)

[Home](../README.md)
