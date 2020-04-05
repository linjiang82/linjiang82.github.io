---
categories: WebDevelop
---

###How to use CSSTransition with a module css/scss
* import CSSTransition from React-Transition-Group
* Name the CSS selectors in css module using camelCase way as below.Need to mention that if not using module css, the naming is using '-' like '{transitionName}-enter-active'
```css
.enter {
opacity: 0;
}
.enterActive {
opacity: 1;
transition: opacity 1000ms ease-in-out;
}
.exit {
opacity: 1;
}
.exitActive {
opacity: 0;
transition: opacity 1000ms ease-in-out;
}
```
* import arbitrayName from 'Css module'
* use the arbitrayName in CSSTransition like a variable
