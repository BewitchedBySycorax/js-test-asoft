### Задание №1

Реализовать функцию `myLisp(inputStr)`
Реализовать функцию `myLisp`, которая будет проверять корректность открытиязакрытия скобок в строке `inputStr` и возвращать `true` если строка корректна, в ином функция должна возвращать `false`.
Строка `inputStr` может состоять из любых символов, но все кроме скобок {}, [] и () должно игнорироваться.

**Примеры вызовов:**
```javascript
myLisp('()') //true
myLisp('[)') //false
myLisp('{}[]()') //true
myLisp('([{}])') //true
myLisp('())({}}{()][][') //false
```

### Задание №2

Реализовать функцию `checkQuadsDoubles(num1,num2)`
Реализовать функцию, которая принимает в качестве аргументов числа `num1` и `num2`. Функция должна возвращать `true` если в `num1` есть 4 подряд идущих одинаковых цифры и 2 тех же, подряд идущих, цифры в `num2`, в ином случае функция должна возвратить `false`.

**Примеры вызовов:**
```javascript
checkQuadsDoubles(45568411115, 11223344) //true;
checkQuadsDoubles(11112344445, 442253) //true;
checkQuadsDoubles(12222345, 123452) //false;
checkQuadsDoubles(12345, 12345) //false;
```

### Задание №3

Реализовать метода `Array.groupBy`
Добавить к глобальному объекту `Array` метод `groupBy`, который позволяет сгруппировать элементы массива по результату выполнения функции полученной в качестве аргумента.

**Примеры вызовов:**
```javascript
[1,2,3,2,4,1,5,1,6].groupBy()
{
   1: [1, 1, 1],
   2: [2, 2],
   3: [3],
   4: [4],
   5: [5],
   6: [6]
}
```

```javascript
[1,2,3,2,4,1,5,1,6].groupBy(function(val) { return val % 3;} )
{
   0: [3, 6],
   1: [1, 4, 1, 1],
   2: [2, 2, 5]
}
```

### Задание №4

HTML:
```html
<button id="counter">Click me (0)</button>
```

Задание:
Реализовать подсчет кликов, максимум до 3-х включительно, при достижении заданного количества обработчки должен сниматься
Реализовать на чистом js, с использованием jQuery, с использованием angularjs, с использованием react


### Задание №5

Реализовать метод `fn.delay(ms)`

**Пример вызова:**
```javascript
var myAlert = function (){
    alert("bingo!");
};

myAlert.delay(1000); // Алерт "bingo!" появится через 1с
```


### Задание №6

Реализовать функцию Dummy:

```javascript
function Dummy(){...}
```

так чтобы код ниже работал:
```javascript
// код ниже должен работать
var A = Dummy();
var B = new Dummy();

console.log(A === B); // должно выводить в консоль true
```

### Задание №7

Реализовать методы on и trigger:
```javascript
const eventEmitter = {}; 
eventEmitter.on = function (eventName, handler) {...};
eventEmitter.trigger = function (eventName, data) {...};
```

так, чтобы код ниже работал и в консоль вывелась единица:
```javascript
eventEmitter.on('click', (data) => {
  console.log(data);
});

eventEmitter.trigger('click', 1);
```
