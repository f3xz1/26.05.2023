Я работал только в style.css и script.js

По какой то причине, при изменении ширины браузера @media работает, но при открытии мобильной версии сайта ничего не меняеться.

Я изменил внешний вид navbar, добавил анимацию добавления рамок у кнопки Search и исправил дописал это в script.js:

```javascript
onresize = function () {
  if (this.window.innerWidth <= 768) {
    burgerMenu.style.rotate = "0deg";
    navSlider.style = ` top: 0px;position: absolute;display: none;`;
    navSlider.querySelector(".nav-slider-inner").style = `display: none;`;
    menuToggler = false;
  }
};
```

Я не разобрался, ставьте кол (T_T)
