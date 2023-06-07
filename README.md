# advanced-css-sass
notes for this course https://www.udemy.com/course/advanced-css-and-sass/learn/lecture

## ``transform``
 
- center element:
```css
.text-box {
  position: absolute;
  top: 50%;
  left: 50%;
  transform: translate(-50%, -50%);
  text-align: center;
}
```

📌[transform specifications](https://drafts.csswg.org/css-transforms/#transform-property):
- No transform on non-replaced inline boxes, table-column boxes, and table-column-group boxes.
 
e.g. [Stackoverflow: transform-not-working-on-css-hover-element](https://stackoverflow.com/questions/48172124/transform-not-working-on-css-hover-element)


## ``@keyframes``

```css
@keyframes slidein {
  from {
    transform: translateX(0%);
  }

  to {
    transform: translateX(100%);
  }
}

from
A starting offset of 0%.

to
An ending offset of 100%.
```

e.g.
```css
@keyframes moveInLeft {
  0% {
    opacity: 0;
    transform: translateX(-100px);
  }
  80% {
    transform: translateX(20px);
  }
  100% {
    opacity: 1;
    transform: translateX(0);
  }
}
```