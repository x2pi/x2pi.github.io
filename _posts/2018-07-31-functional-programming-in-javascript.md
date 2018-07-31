---
title: Functional programming in Javascript
date: 2018-07-31 00:00:00 +0000
layout: post
creationdate: ''
tags:
- JS
- Functional Programing
- 'book '

---
### Item 1: Thay vì sử dụng trực tiếp có thể thay thế bằng hàm

Mua sách ủng hộ tác giả nhé: [Functional Programming in JavaScript](https://www.amazon.com/Functional-Programming-JavaScript-functional-techniques/dp/1617292826)

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