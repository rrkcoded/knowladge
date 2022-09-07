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


Work with string
.... //concatenation
a = firstNames + firstNames;
a = firstNames + ' ' + lastNames;
a = 'Im ' + firstNames + firstNames;
a = 'Im' + ' ' + firstNames + ' ' + firstNames;
a = 'Im' + ' ' + age + ' ' + 'years old';


Cycles
//     while,   do while,   for,  for of,   for in

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


let colors = ['Red', 'White', 'Blue', 'Green', 'Black'];
for (let i = 0; i < colors.length; i++) {
    console.log(colors[i])
}


            FOR IN
Перебрати властивості об'єкта для кожної властивості виконати заданий код


const player = {
    name: 'Oleg',
    age: '14',
    city: 'Kyiv'
};
for (let key in player) {
    console.log(key)
    console.log(player[key])
}
console.clear()




            FOR OF
Оператор for...of відноситься до типу оператора for, який циклічно повторює об'єкти, поки не досягне кінця рядка.


for (let value of users) {
    console.log(value)
}








                       FUNCTION 

Функція - це значення, що представляє 'дія'
Звичайні значення, такі як рядки або числа є даними.
Функції, з іншого боку, можна як дії.
Ми можемо передавати їх із змінної до змінної і запускати, коли захочемо.                       


Function Declaration: функция объявляется отдельной конструкцией «function…» в основном потоке кода.
// Function Declaration
function sum(a, b) {
  return a + b;
}



Function Expression: функция, созданная внутри другого выражения или синтаксической конструкции. В данном случае функция создаётся в правой части «выражения присваивания» =:
// Function Expression
let sum = function(a, b) {
  return a + b;
};


Function Declaration может быть вызвана раньше, чем она объявлена.

Другими словами, когда движок JavaScript готовится выполнять скрипт или блок кода, прежде всего он ищет в нём Function Declaration и создаёт все такие функции. Можно считать этот процесс «стадией инициализации».

И только после того, как все объявления Function Declaration будут обработаны, продолжится выполнение.

В результате функции, созданные, как Function Declaration, могут быть вызваны раньше своих определений.



- Если функция объявлена как отдельная инструкция в основном потоке кода, то это “Function Declaration”.
- Если функция была создана как часть выражения, то это “Function Expression”.
- Function Declaration обрабатываются перед выполнением блока кода. Они видны во всём блоке.
- Функции, объявленные при помощи Function Expression, создаются только когда поток выполнения достигает их.






















