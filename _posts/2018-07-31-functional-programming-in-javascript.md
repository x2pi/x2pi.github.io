---
title: Functional programming in Javascript
date: 2018-07-31 00:00:00 +0000
layout: post
creationdate: ''
tags:
- JS
- Functional Programing

---
#### Item 1: Thay vì sử dụng trực tiếp có thể thay thế bằng hàm
<i class="far fa-thumbs-down"></i>
```javascript
document.querySelector('#msg').innerHTML = '<h1>Hello World</h1>';
```
<i class="far fa-thumbs-up"></i>
```javascript
function printMessage(elementId, format, message) {
document.querySelector(`#${elementId}`).innerHTML =
`<${format}>${message}</${format}>`;
}
printMessage('msg', 'h1','Hello World');
```

