## Яндекс
[Задача1(Яндекс-js-06-05-25)](#задача1яндекс-js-06-05-25)


## Задачи на js
[Задача1(Яндекс-js-06-05-25)](#Задача1(яндекс-js-06-05-25))



## Задача1(Яндекс-js-06-05-25)
Реализовать метод times для числового объекта (числа). Метод должен принимать функцию-колбэк (callback) 
и вызывать её столько раз, каково значение числа.
Каждый раз в колбэк должен передаваться индекс текущей итерации (начиная с 0).

<details>
<summary><strong>Разбор(своими словами) </strong></summary>
 
1.  Добавление метода в прототип Number:
    - `Number.prototype.times = ...` — добавляет новый метод times ко всем числовым значениям в JavaScript.
    - Это позволяет вызывать (3).times(...), (5).times(...) и т. д.

2. Цикл for:
    - for (let i = 0; i < this; i++) — цикл выполняется от 0 до this - 1 (где this — числовое значение, у которого вызван метод).
    - Например, для (3).times(...) цикл выполнится 3 раза (i = 0, i = 1, i = 2).
3. Вызов колбэка:
    - callback(i) — на каждой итерации вызывается переданная функция (console.log в примере), куда передаётся текущий индекс i.

</details>

<details>
<summary><strong>Решение</strong></summary>
 
```js
Number.prototype.times = function(callback) {
  for (let i = 0; i < this; i++) {
    callback(i);
  }
};
```
</details>


 <details>
<summary><strong> Решение с пояснениями</strong></summary>

```js
Number.prototype.times = function(callback) {
  // Цикл for выполняется от 0 до this-1 (this — числовое значение, на котором вызван метод)
  for (let i = 0; i < this; i++) {
    // Вызываем переданный callback, передавая текущий индекс i
    callback(i);
  }
};
```
</details>

## Задача2(Яндекс-js-06-05-25)
Реализовать функцию sumPromises, которая принимает в качестве аргументов промисы и возвращает сумму результатов их выполнения.
Функция может принимать любое количество аргументов.Можно использовать любые API промисов.
```
// Пример использования
const promise1 = Promise.resolve(1);
const promise2 = Promise.resolve(2);

sumPromises(promise1, promise2).then(console.log); // 3
```
<details>
<summary><strong>Разбор(своими словами) </strong></summary>
 
1.  Добавление метода в прототип Number:
    - `Number.prototype.times = ...` — добавляет новый метод times ко всем числовым значениям в JavaScript.
    - Это позволяет вызывать (3).times(...), (5).times(...) и т. д.

2. Цикл for:
    - for (let i = 0; i < this; i++) — цикл выполняется от 0 до this - 1 (где this — числовое значение, у которого вызван метод).
    - Например, для (3).times(...) цикл выполнится 3 раза (i = 0, i = 1, i = 2).
3. Вызов колбэка:
    - callback(i) — на каждой итерации вызывается переданная функция (console.log в примере), куда передаётся текущий индекс i.

</details>

<details>
<summary><strong>Решение</strong></summary>
 
```js
Number.prototype.times = function(callback) {
  for (let i = 0; i < this; i++) {
    callback(i);
  }
};
```
</details>


 <details>
<summary><strong> Решение с пояснениями</strong></summary>

```js
Number.prototype.times = function(callback) {
  // Цикл for выполняется от 0 до this-1 (this — числовое значение, на котором вызван метод)
  for (let i = 0; i < this; i++) {
    // Вызываем переданный callback, передавая текущий индекс i
    callback(i);
  }
};
```
</details>



