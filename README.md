# Markdown cheatsheet

## Вставка HTML
Для создания разметки, которую синтаксис Markdown не обеспечивает, можно просто использовать сам HTML.

Единственное ограничение состоит в том, что блочные элементы HTML должны отделяться пустыми строками от окружающего их текста, причём начальный и конечный тэг не должны отступать от начала строки.

Синтаксис форматирования Markdown не обрабатывается внутри блочных элементов HTML.
Но в отличие от блочных элементов HTML, во внутристрочных элементах HTML обрабатывается синтаксис Markdown.

## Автоматическое кодирование специальных символов

В языке HTML есть два символа, требующих специального к себе отношения: это `<` и `&`.  
Левая угловая скобка используется как начало тэга; амперсанды применяются для обозначения сущностей (entities).  
А чтобы использовать эти символы в их буквальном смысле, приходится их самих приводить как сущности, то есть `&lt;` и `&amp;` соответственно.
Markdown позволяет использовать эти символы естественным образом.

## Содержание
[Абзацы и переводы строки](https://github.com/GermanGorelkin/markdown-cheatsheet/blob/master/Basic.md#lines)  
[Заголовки](https://github.com/GermanGorelkin/markdown-cheatsheet/blob/master/Basic.md#headers)  
[Цитаты](https://github.com/GermanGorelkin/markdown-cheatsheet/blob/master/Basic.md#blockquotes)  
[Списки](https://github.com/GermanGorelkin/markdown-cheatsheet/blob/master/Basic.md#lists)  
[Блоки кода](https://github.com/GermanGorelkin/markdown-cheatsheet/blob/master/Basic.md#code)  
[Горизонтальная черта](https://github.com/GermanGorelkin/markdown-cheatsheet/blob/master/Basic.md#hr)  
[Ссылки](https://github.com/GermanGorelkin/markdown-cheatsheet/blob/master/Basic.md#links) 
[Выделение](https://github.com/GermanGorelkin/markdown-cheatsheet/blob/master/Basic.md#emphasis)  
[Таблицы](https://github.com/GermanGorelkin/markdown-cheatsheet/blob/master/Basic.md#tables)  
[Изображения](https://github.com/GermanGorelkin/markdown-cheatsheet/blob/master/Basic.md#images)  