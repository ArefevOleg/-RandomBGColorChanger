#  Building a Random Background Color
Создаём программу для случайного изменения цвета фона, находим и исправляем ошибки.

## 1.
```javascript
// На старте проекта была предоставлена разметка HTML и стилизация CSS.
// Нужно было исправить синтаксические ошибки в массиве darkColorsArr.

const darkColorsArr = [
  "#2C3E50",
  "#34495E",
  "#2C2C2C"
  "#616A6B"
  "#4A235A"
  "#2F4F4F",
  "#0E4B5A",
  "#36454F",
  "#2C3E50",
  "#800020",
];
// запятые
```
## 2.
```javascript
// При ссылке на несуществующую переменную выдается ошибка ReferenceError. 
// В данном случае, похоже, что CamperBot пытается использовать math, но в JavaScript нет объекта math.
console.log(darkColorsArr.length * math.random())
// Math.random()
```
## 3.
```javascript
// Обновите инструкцию консоли, чтобы вывести целое число в диапазоне от 0 до 9.
console.log(darkColorsArr.length * math.random())
// Math.floor()
```
## 4.
```javascript
// Исправьте ошибку TypeError, обновив документ.
// В методе queryselector используется правильное имя метода, который выбирает элемент из DOM.
const body = document.queryselector("body");
// document.querySelector
```
## 5.
```javascript
// Исправьте документ.Строка querySelector("bg-hex-code"), 
// чтобы она корректно выбирала элемент с идентификатором bg-hex-code.
const body = document.querySelector("body");
const bgHexCodeSpanElement = document.querySelector("bg-hex-code");

console.log(bgHexCodeSpanElement);
// "#bg-hex-code"
```
## 7.
```javascript
// Исправьте ошибку в документе.Строка querySelector("#click-btn");.
const btn = document.querySelector("#click-btn");
console.log(btn);
// "#btn"
```
## 8.
```javascript
// Исправьте ошибку в строке btn.onclick = изменить цвет фона();.
btn.onclick = changeBackgroundColor();
// btn.onclick = changeBackgroundColor;
```


###### из курса [freecodecamp](https://www.freecodecamp.org/learn/javascript-algorithms-and-data-structures-v8/)