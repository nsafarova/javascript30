> This is a JavaScript practice with [JavaScript30](https://javascript30.com/) by [Wes Bos](https://github.com/wesbos) without any frameworks, no compilers, no boilerplate, and no libraries.

# 05 - Flex Panels Image Gallery

View Demo here -> [Flex Panels Image Gallery](link)

![](../images/day-05.png)

## How to use
 - click on the each row to open and click back to close

## Learning notes

 - CSS3 `flexbox` layout and nested flexbox
 - `Event handling` used to handle `click` and `transitionend` events
 - use `toggle()` to add or remove a CSS class to the selected element

### includes()

> Safari transitionend event.propertyName === flex */
>
> Chrome + FF transitionend event.propertyName === flex-grow */

`includes()` is used to check for the word "flex" in the `propertyName` property of the `transitionend` event object to ensure cross-browser compatibility.

```
if (e.propertyName.includes('flex')) {
  this.classList.toggle('open-active');
}
```
