# Floating Cursore

Interesting animation for cursor on css and some js you can use to decorate your project

## Take note 
- calculating cursor position


```javascript
document.addEventListener("mousemove", (e) => {
document.body.style.cssText = `--move-x: ${e.clientX}px; --move-y: ${e.clientY}px;`;
});
```

- Styling cursor to change the position and initial height

```css
height: 0;
transform: translate3d(var(--move-x), var(--move-y), 0);
transition: transform var(--transition-cursor), height 1s ease;

```

- Styling cursor image 

>Height calculate in index height is calculated from the index variable  `--index: calc(1vw + 1vh)` for adaptation 

```css
transform: var(--cursor-transform) scale(1.5);
height: calc(var(--height) * 2);
```
- For `hover`

```css
.magic-list__item:hover .cursor__image {
  transform: var(--cursor-transform) scale(1);
}
```

## Screenshot

![ezgif com-video-to-gif-3](https://user-images.githubusercontent.com/113831614/223547308-e67206dc-cd6d-4713-b4c0-62e55f7145dc.gif)


 
