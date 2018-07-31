---
title: Functional programming in Javascript
date: 2018-07-31 00:00:00 +0000
layout: post
creationdate: ''
tags:
- 'book '
- js
- functional programin

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
	document.querySelector(`#${elementId}`).innerHTML = `<${format}>${message}</${format}>`;
}
printMessage('msg', 'h1','Hello World');
```

### Item 2: Thay vòng lặp qua các phần tử của mảng bằng hàm

<i class="far fa-thumbs-down"></i>

```javascript
var array = [0, 1, 2, 3, 4, 5, 6, 7, 8, 9];
for(let i = 0; i < array.length; i++) {
     array[i] = Math.pow(array[i], 2);
}
array; //-> [0, 1, 4, 9, 16, 25, 36, 49, 64, 81]
```
<i class="far fa-thumbs-up"></i>

```javascript
[0, 1, 2, 3, 4, 5, 6, 7, 8, 9].map(
  function(num) {
    return Math.pow(num, 2);
  });
    //-> [0, 1, 4, 9, 16, 25, 36, 49, 64, 81]
```