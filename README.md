___
# МИНИСТЕРСТВО НАУКИ И ВЫСШЕГО ОБРАЗОВАНИЯ РОССИЙСКОЙ ФЕДЕРАЦИИ ФЕДЕРАЛЬНОЕ ГОСУДАРСТВЕННОЕ БЮДЖЕТНОЕ ОБРАЗОВАТЕЛЬНОЕ УЧРЕЖДЕНИЕ ВЫСШЕГО ПРОФЕСИОНАЛЬНОГО ОБРАЗОВАНИЯ «САХАЛИНСКИЙ ГОСУДАРСТВЕННЫЙ УНИВЕРСИТЕТ»
### <p align="center">Лабораторная работа №5 “JS”</p> 
#### <br><p align="right">Подготовил студент направления подготовки 01.03.02 «Прикладная математика и информатика»<br> Института естественных наук и техносферной безопасности<br> Зураев Дмитрий Бакенович.</p><br><p align="right">Научный руководитель:<br> Соболев Евгений Игоревич.</p><br> <p align="center">Южно-Сахалинск 2023 г.</p>
___
### <p align="center">Введение</p>
<p align="justify">JavaScript (JS) - это высокоуровневый язык программирования, который используется для создания интерактивных и динамических веб-страниц. JS является одним из трех основных языков, используемых веб-браузерами (наряду с HTML и CSS), и позволяет добавлять функциональность и взаимодействие на веб-страницах.
Лабораторная работа по JavaScript (JS) предоставляет возможность познакомиться с одним из самых популярных языков программирования, используемых для разработки веб-приложений.</p>

### <p align="center">Цели</p>
<p align="justify">Ознакомиться с основными концепциями и возможностями JavaScript. Изучить синтаксис языка, работу с переменными, операторами, условиями, циклами и функциями. Также поработать с форматом типа Date.</p>

### <p align="center">Задачи</p>
<p align="justify">Применить технологию JS.</p>

____________________
## <p align="center">_Решение_</p>
1.
```javascript
var str = 'hdfgv';
alert(str[0]);
alert(str[1]);
alert(str[4]);
```
2.
```javascript
var secondsInHour = 60*60;
alert(`2) Количество секунд в часе: ${secondsInHour}`);
```
3.
```javascript
var num = 1;
num += 12;
num -= 14;
num *= 5;
num /= 7;
num++;
num--;
alert(num);
```
4.
```javascript
var num = 3;
alert("4) " + num);
```
5.
```javascript
var a = 10;
var b = 2;
alert(`5) Числа ${a} и ${b}.\nСумма: ${a+b}; Разность: ${a-b}; Произведение: ${a*b}; Частное: ${a/b}`);
```
6.
```javascript
var c = 15;
var d = 2;
var result = c + d;
alert("6) " + result);
```
7.
```javascript
var a = 10, b = 2, c = 5;
alert(`7) Сумма a+b+c = ${a+b+c}`);
```
8.
```javascript
var a = 17;
var b = 10;
var c = a - b;
var d = 7;
var result = c + d;
alert("8) " + result);
```
9.
```javascript
var secondsInDay = secondsInHour*24;
var secondsInMonth = secondsInDay*30;
alert(`9) Количество секунд в часе: ${secondsInHour}\nКоличество секунд в сутках: ${secondsInDay}\nКоличество секунд в месяце: ${secondsInMonth}\n`);
```
10.
```javascript
var hour = 13;
var minute = 40;
var second = 55;
alert(`10) ${hour}:${minute}:${second}`);
```
11.
```javascript
var number = 12;
var square = 12*12;
alert("11) " + square);
```
12.
```javascript
alert("12) " +
    // Входной массив
    [4,9,144]
      // Оставляем только чётные числа
      .filter(element => !(element % 2))
      // Считаем квадратный корень и записываем в аккумулятор
      .reduceRight((accumulator, element) => accumulator + Math.sqrt(element), 0)
   );
```
13.
```javascript
var applePrice = 1.15;
var orangePrice = 2.30;
alert("13) В JavaScript, при выполнении операции сложения чисел с плавающей точкой,может возникнуть проблема с точностью. Это связано с тем, что числа с плавающей точкой представлены в двоичной системе, и некоторые числа не могут быть точно представлены в этой системе. \nНаш результат будет немного неточным = " + (applePrice + orangePrice));
```
14.
```javascript
//fourteen тк сначала вывел икс потом увелич.
alert("14) let x = 5; alert(x++); - Получится 5");
```
15.
```javascript
//fifteen при преобраз. типов
alert(`15) [ ] + false - null + true - будет ${[] + false - null + true} Not a Number, то есть не число`);
```
16.
```javascript
//sixteen справа налево
alert(`16) let y = 1; let x = y = 2; console.log(x); - выведет Два`);
```
17.
```javascript
//seventeen пуст. масс. преобр. в пуст. стр.
alert(`17) [ ] + 1 + 2 - будет 12`);
```
18.
```javascript
var a6 = 5 % 3; //остаток от деления 5 на 3 равно 2
var a7 = 3 % 5; //остаток от деления 3 на 5 равно 3
var a8 = 5 + '3'; //будет равно "53"
var a9 = '5' - 3; //строка "5" будет преобразована в число, будет равно 2
var a10 = 75 + 'кг'; //равно "75кг"
```
19.
```javascript
var height = 23;
var width = 10;
var s = height*width;
alert(`19) Площадь прямоугольника = высоту ${height} * ширину ${width} = ${s} см2`);
```
20.
```javascript
var heightC = 10;
var dC = 4;
var v = heightC*Math.PI*(dC*dC/4);
alert(`20) Объем циллиндра = V=h*PI*d2/4 = ${v} см3`);
```
21.
```javascript
var S = 2_000_000;
var p = 10;
var years = 5;
var perepl = S*(p*years/100); //2млн - 10 процентов в год
alert(`21) ${perepl} переплата при сумме в ${S} млн на ${years} лет под ${10} процентов`);
```
22.
```javascript
var str = "Привет";
var num = 123;
var flag = true;
var txt = "true";
alert(`str = \"Привет\" - тип ${typeof(str)}\nnum = 123 - тип ${typeof(num)}\nflag = true - тип ${typeof(flag)}\ntxt = \"true\" - тип ${typeof(txt)}`);
```
23.
```javascript
var num = prompt("Введите число, а я выведу противоположное");
alert(`Противоположное число числу ${num}: ${-num}`);
```
[Kata1](https://www.codewars.com/kata/56530b444e831334c0000020)
```javascript
function chromosomeCheck(sperm) {
if(sperm == "xx" || sperm == "XX" || sperm == "xX" || sperm == "Xx" ){
   return "Congratulations! You're going to have a daughter.";
} else if(sperm == "xy" || sperm == "xY" || sperm == "XY" || sperm == "Xy" ){
   return "Congratulations! You're going to have a son."
} else {
    return "It`s a wrong data";
}
}
```
[Kata2](https://www.codewars.com/kata/583710ccaa6717322c000105)
```javascript
function simpleMultiplication(number) {
if(number % 2 == 0){
   return number * 8;
} else if(number % 2 != 0){
   return number * 9;
} else {
    return "It`s a wrong data";
}
}
```
[Kata3](https://www.codewars.com/kata/5a805d8cafa10f8b930005ba)
```javascript
function nearestSq(n){
  var num = Math.trunc(Math.sqrt(n)); // 10
  var sqNum = num*num; // 100
  var nextSqNum = Math.pow(num+1, 2); // 121 
  var difSqNum = n-sqNum; // 111-100 = 11
  var difSqNextNum = nextSqNum - n; //121-111 = 10
  if(n<0){
      return "Enter a positive number";
  } else if(difSqNum > difSqNextNum){
      return nextSqNum;
  } else if (difSqNum < difSqNextNum){
      return sqNum;
  } else {
      return n;
  }
}
```
[Kata4](https://www.codewars.com/kata/5763bb0af716cad8fb000580)
```javascript
function countSquares(cuts){
  //return cuts == 0 ? 1 : 6 * cuts * cuts + 2;
  if(cuts == 0 || cuts == +0 || cuts == -0)
    return 1;
  else 
    return 6 * cuts * cuts + 2;
}
```
[Kata5](https://www.codewars.com/kata/578a8a01e9fd1549e50001f1)
```javascript
function periodIsLate(last, today, cycleLength) {
  //перевел миллисек в дни
  if(((today - last)/ (24 * 60 * 60 * 1000)) > cycleLength)
    return true;
  return false;
}
```
[Kata6](https://www.codewars.com/kata/57eae20f5500ad98e50002c5)
```javascript
function noSpace(x){
  return x.split(" ").join("").trim();
  //разбить на массив слов по пробелу.объеденить в строку.убрать нач и кон пробелы
}
```
## <center>_Вывод_</center>
Таким образом, я изучил основные понятия и возможности в JavaScript. Ознакомился с синтаксисом языка, работал с переменными, операторами, условиями, циклами и функциями. Также поработал с форматом типа Date.
