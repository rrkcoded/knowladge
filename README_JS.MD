Data types
Boolean: true/false,
String: "12323", "Andrey", ' '
Number: 22143, 2
Array: [1,2,3,4,5] , [А, B, C]
Null: null
Underfined: underfined


Comparisson
> Больше
< Меньше
<= Меньше, или равно
>= Больше, или равно
== Равно по значенню но не по типу данных
=== Равно и по значенню и по типу данных
!== Не равно по типу данных
!=== Не равно по значенню и по типу данных

Math
value = Math.PI;     число пи
value = Math.random();     рандом 0-1
value = Math.round(2.4);    обычное округление
value = Math.ceil(2.1);   округления в большую пользу
value = Math.floor(2.9);    округления в меньшую пользу
value = Math.min(2, 12, 15, 0, 12);    отбиракет мин значение
value = Math.floor(Math.random() * 10 + 1);    рандом 1-10


Lenght

let name = 'Denis';
if (name.lenght < 3) {       // name.lenght количество значений в строке
alert("Too small") 
}

let colors = ['White', 'Red', 'Green']; // colors.lenght количество объектов в массиве
if (colors.lenght < 4) {
alert("Too small")
}



Переменные Variable
var 
const - нельзя перезаписывать


Условные операторы Conditional Statements

if...else  =
if (a = 0){
   some action
} else {
 some action
}

switch =
switch(color) {
  case 'green':
     console.log('Color is green');
     break;
  case 'red':
     console.log('Color is red');
     break;
  default:
     console.log('Default')
...

Cycles
//     while,   do while,   for,  (soon = for of, for in)

Перерахує від 1 до 10
let i = 0;
while (i++ < 10) {
console.log(i);
}

Cпочатку вибиває в консоль а потім перераховує
do {
console.log('some action');
} while (i < 0)

for (let i = 0; i < 10; i++) {
console.log(i)
}


Work with string
.... //concatenation
a = firstNames + firstNames;
a = firstNames + ' ' + lastNames;
a = 'Im ' + firstNames + firstNames;
a = 'Im' + ' ' + firstNames + ' ' + firstNames;
a = 'Im' + ' ' + age + ' ' + 'years old';

