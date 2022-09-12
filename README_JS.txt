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
!== Не равно по значенню
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

Другими словами, когда движок JavaScript готовится выполнять скрипт или блок кода, прежде всего он ищет в нём 
Function Declaration и создаёт все такие функции. Можно считать этот процесс «стадией инициализации».

И только после того, как все объявления Function Declaration будут обработаны, продолжится выполнение.

В результате функции, созданные, как Function Declaration, могут быть вызваны раньше своих определений.



- Если функция объявлена как отдельная инструкция в основном потоке кода, то это “Function Declaration”.
- Если функция была создана как часть выражения, то это “Function Expression”.
- Function Declaration обрабатываются перед выполнением блока кода. Они видны во всём блоке.
- Функции, объявленные при помощи Function Expression, создаются только когда поток выполнения достигает их.




let valueV2;
let value;
value = numbers.length
valueV2 = numbers.length
value = Array.isArray(numbers)  // проверка массив ли это
value = numbers[2]
numbers[1] = 77; // заменяем 1 элемент на значение 77
numbers[0] = 11;
value = numbers.indexOf(77); // в value выводим какой по счёту элемент с значением 77

value = numbers.push(200); // добавляет в конец (в value будет количество элементов в масиве)

value = numbers.pop(); // удаляет с конца (в value вернётся элемент который удалило)

value = numbers.unshift(1121); // добавляет в начало (в value будет количество элементов в масиве)

value = numbers.shift(); // удаляет с начала (в value вернётся элемент который удалило)

value = numbers.slice(0, 3); // обрезает часть масива не меняя его исходный масив

value = numbers.splice(1, 3, "GG", 882); // вырезает нужные объкты.  первое число это с какого объкта в масиве начинать, второе это по какое вырезать. Все что идёт после будет добавляться в исходный масив

valueV2 = numbersV2.reverse(); // переворачивает масив

valueV2 = numbersV2.concat(1, 2, 32, 'ff') // конкатенирует (добавляет) в масив

value = numbersV2.join() // делает из масива строку

value = numbersV2.join('') // делает из масива строку

console.log(value, numbers); // делает из масива строку + соеденяет все объекты масива в один объект


let newMass = [];
for (let i = 0; i < mass.length; i++){
    newMass.push(mass[i].length);
}
console.log(newMass); // => [3, 4, 4, 6]
// Вместо имён вписывает количество символов в одном элементе




let newMass2 = [];
for (let i = 0; i < mass.length; i++) {
    newMass2.push(mass[i].toUpperCase());
}
console.log(newMass2); // Все элементы пишет капсом



forEach - просто перебирает массив ничего не возвращая
filter - фильтрует
map - возвращает новый массив на основе callback(a)
reduce - помогает разворачивать массив / формировать структура (напр. из массива в объект)
some/every - some вернёт true, если хотя бы 1 элемент удовлитворяют условия callback ;  every вернёт true, если все элементы удовлитворяют условия callback
sort - сортировать
find - найти


// forEach
users.forEach((user, i, arr) => {
    console.log(users, i, arr);
});










