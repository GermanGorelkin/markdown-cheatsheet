# Абзацы и переводы строки

Абзац записывается в Markdown весьма просто: это одна или несколько строк текста,  
отделённые от окружающего текста одной (или более чем одной) пустой строкою.  
Чтобы вставить видимый перенос строки (элемент `<br />`) посредством Markdown,  
необходимо добавить **два пробела**.

# Заголовки

Markdown поддерживает два стиля заголовков: подчёркнутые и выделенные символом «#»:

```
# H1
## H2
### H3
#### H4
##### H5
###### H6
```
```
Alt-H1
======
Alt-H2
------
```

# H1
## H2
### H3
#### H4
##### H5
###### H6

Alt-H1
======
Alt-H2
------

# Цитаты

Markdown использует email-подобный стиль использования символов > для оформления цитат:

> This is a blockquote with two paragraphs. Lorem ipsum dolor sit amet,
> consectetuer adipiscing elit. Aliquam hendrerit mi posuere lectus.
> Vestibulum enim wisi, viverra nec, fringilla in, laoreet vitae, risus.
> 
> Donec sit amet nisl. Aliquam semper ipsum sit amet velit. Suspendisse
> id sem consectetuer libero luctus adipiscing.

Markdown позволяет ставить > только перед первой строкой абзаца:

> This is a blockquote with two paragraphs. Lorem ipsum dolor sit amet,
consectetuer adipiscing elit. Aliquam hendrerit mi posuere lectus.
Vestibulum enim wisi, viverra nec, fringilla in, laoreet vitae, risus.

Цитаты могут быть вложенными:

> This is the first level of quoting.
>
> > This is nested blockquote.
>
> Back to the first level.

Цитаты могут содержать и другие элементы Markdown — заголовки, списки, кодовые блоки:

> ## This is a header.
> 
> 1.   This is the first list item.
> 2.   This is the second list item.
> 
> Here's some example code:
> 
>```return shell_exec("echo $input | $markdown_script");```

# Списки

Markdown позволяет составлять нумерованные и ненумерованные списки.

```
*   Red
*   Green
*   Blue
```
```
+   Red
+   Green
+   Blue
```
```
-   Red
-   Green
-   Blue
```

*   Red
*   Green
*   Blue

+   Red
+   Green
+   Blue

-   Red
-   Green
-   Blue

Нумерованные списки используют в качестве маркеров числа с точкою:

```
1.  Bird
2.  McHale
3.  Parish
```
1.  Bird
2.  McHale
3.  Parish

Если элементы списка разделяются пустыми строками, то Markdown обернёт эти элементы тэгами `<p>` в своём итоговом HTML-коде:

```angular2html
*   Red

*   Green
```
*   Red

*   Green

Элементы списка могут состоять из нескольких абзацев. Второй, и третий, и каждый последующий абзац элемента должны снабжаться отступом из четырёх пробелов:

```
1.  This is a list item with two paragraphs. Lorem ipsum dolor
    sit amet, consectetuer adipiscing elit. Aliquam hendrerit
    mi posuere lectus.

    Vestibulum enim wisi, viverra nec, fringilla in, laoreet
    vitae, risus. Donec sit amet nisl. Aliquam semper ipsum
    sit amet velit.

2.  Suspendisse id sem consectetuer libero luctus adipiscing.
```

Если внутри элемента списка располагается цитата, то надобно снабжать отступом разделители «>»:

```
*   A list item with a blockquote:

    > This is a blockquote
    > inside a list item.
```
*   A list item with a blockquote:

    > This is a blockquote
    > inside a list item.

Чтобы поместить кодовый блок внутри элемента списка, этот кодовый блок надобно снабдить двукратным отступом, то есть либо восемью пробелами, либо двумя символами табуляции:

```
*   A list item with a code block:

        <code goes here>
```
*   A list item with a code block:

        <code goes here>

Вложенные списки:

```
* One
  * One v2
  * Two v2
* Two
```

# Блоки кода

Блоки кода выделяются либо тремя обратными апострофами ` ``` ` либо четырьмя пробелами в каждой строке.  
В отличие от обычных абзацев, переносы строк в кодовом блоке воспринимаются буквально.  
Markdown обрамляет кодовый блок сразу двумя элементами HTML — и `<pre>`, и `<code>`.  
Внутри кодового блока амперсанды («&») и угловые скобки («<» и «>») автоматически преобразуются в HTML-сущности (HTML entities).

# Горизонтальная черта

Чтобы создать горизонтальную черту (соответствующую HTML-элементу `<hr />`), достаточно поместить три (или более) дефиса, или звёздочки, или символа подчёркивания:

```
* * *

***

*****

- - -

---------------------------------------
```

# Ссылки

