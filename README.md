# Лабораторная №2 по теме "Обновляемый список в React"

## Задание 1
Сделать так, чтобы при нажатии на кнопку "Добавить" то, что введено в текстовое поле, добавлялось в список.

## Задание 2
При нажатии на кнопку [x] элемент удаляется.

## Задание 3
Вывод списка организовать в виде компонентов List и ListItem (имена произвольные, можно использовать свои):
```jsx
<List>
  <ListItem/>
  <ListItem/>
  <ListItem/>
  <ListItem/>
</List>
```
Вначале писать тест, потом писать компонент.

## Способ выполнения
* Сделать форк этого репозитория. 
* Разработку вести через TDD: вначале тесты, потом компонент.
* Решение без тестов приниматься не будет.
* Результат оформить в виде pull request.

## Разработка через TDD
Вначале формулируем требования к компонентам:

### ListItem
* Должен отображает на экране то, что передали в параметре title.
* Должен показывать на экране кнопку.
    * При нажатии на кнопку должен вызываться переданный коллбэк handleClick.
    * Коллбэк должен вызываться с параметром id, который мы передаём в компонент.

### List
* Позитивный кейс: отображение непустого списка:
    * Компонент выводит каждый элемент списка.
    * Кнопка в каждом элементе нажимается, при этом вызывается handleClick с параметром id. _[опционально]_
* Негативный кейс: отображение пустого списка: _[опционально]_
    * Выводится надпись "В списке нет элементов".

### Form _[опционально]_
* Отображается поле для ввода и кнопка "Добавить".
* Можно ввести что-то в поле для ввода.
* При нажатии на кнопку вызывается handleSubmit с параметром,
  равным тому, что ввели в поле для ввода.

## Запуск
```
npm i
```

```
npm start
```

## Запуск тестов
```npm run test```
