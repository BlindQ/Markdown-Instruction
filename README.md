##### <a name="Markdown"></a>
# Что такое Markdown?
Markdown - это облегченный язык разметки созданный с целью обозначения форматирования в простом тексте, с максимальным сохранением его читаемости человеком, и пригодный для машинного преобразования в языки для продвинутых публикаций[1](https://ru.wikipedia.org/wiki/Markdown).</br>
Документы, созданные при помощи Markdown универсалены и легко конвертируемы. Они представляют из себя обычные текстовые файлы (.txt), а это означает, что их можно открыть в любом текстовом редакторе на любой платформе. Помимо этого, документы Markdown, могут быть конвертированые во многие другие удобные форматы, такие как: PDF, DOC, ODT, HTML.</br>


Однако главной особенностью данного языка можно считать максимально простой синтаксис, который служит для упрощения написания и чтения кода разметки, что, в свою очередь, позволяет легко его корректировать. Именно об основных правилах синтаксиса Markdown и будет описано в данной инструкции.
# Содержание
+ [Что такое Markdown?](#Markdown)
+ [Синтаксис заголовков](#Heading)
+ [Форматирование текста](#Text_Formatting)
+ [Цитирование](#Citation)


##### <a name="Heading"></a>
# Синтаксис заголовков

В Markdown представлена возможность создавать до 6 различных заголовков, отличающихся своим размером. Синтаксическое обозначение заголовка производится при помощи символа («#»). В зависимости от уровня заголовка - изменяется количество символов перед наименованием. Пример представлен ниже:</br>

```
# Заголовок 1 уровня
## Заголовок 2 уровня
### Заголовок 3 уровня
#### Заголовок 4 уровня
##### Заголовок 5 уровня
###### Заголовок 6 уровня
```

В результате, на экране появится следующее:
# *Заголовок 1 уровня*
## *Заголовок 2 уровня*
### *Заголовок 3 уровня*
#### *Заголовок 4 уровня*
##### *Заголовок 5 уровня*
###### *Заголовок 6 уровня*


Так же существует альтернативный вариант разметки заголовков первого и второго уровня. Для заголовка первого уровня можно использовать конструкцию («===»), сразу после написания названия заголовка. Второй уровень отличается от первого лишь типом конструкции. Для него вместо символов равенства будут использоваться дефисы («---»). Пример представлен ниже:</br>

```
Альтернативный заголовок 1 уровня
====
Альтернативный заголовок 2 уровня
---
```

В этом случае на экране будет следующее:

*Альтернативный заголовок 1 уровня*
===
*Альтернативный заголовок 2 уровня*
--- 

Как видно, фактический отличий для результата - нет. Однако данный вариант разметки можно считать удобочитаемым только в случае, если в создаваемом тексте не более двух различных уровней заголовков. Так как использование для заголовка третьего уровня символов («#») негативно отразится на унифицированности разметки, что в будущем может затруднить процесс редактирования.

##### <a name="Text_Formatting"></a>

# Форматирование текста
Markdown использует собственную модель форматирования текста. Количество пробелов между символами, в реалиях данного синтаксиса, не имеет никакого значения. По этой же причине одинарное нажание клавишы `Enter` для отступа не принесет ожидаемого результата. Например в синтаксисе Markdown следующие строки:

```
Количество           пробелов    не имеет                никакого значения
Одинарный перевод
```

Будет выглядеть следующим образом:

*Количество           пробелов    не имеет                никакого значения
Одинарный перевод*

Для нормализации формирования абзацев можно использовать один из двух механизмов. В основе первого лежит использование двойного отступа при помощи клавиши `Enter`, что будет создавать видимый разрыв. Если существует необходимость перехода на новую строку без данного разрыва - можно разместить закрывающий тэг `</br>` в конце текста. Например разметка Markdown:

```
Первый абзац</br>
Второй абзац


Третий абзац с разрывом
```
Будет выглядет следующим образом:


*Первый абзац</br>
Второй абзац*


*Третий абзац с разрывом*


##### <a name="Citation"></a>

# Цитирование
Обозначение цитат в Markdown производится с помощью символа больше («>"). Цитаты отличаются от обычного текста специальным выделением, и отлично подходят для вставки дополнительной информации в исходный текст. Синтаксис Markdown поддерживает вложенное цитирование с количеством уровней равным пятнадцати. Пример цитирования представлен ниже:

```
> Это цитата
>> Вторая интересная цитата
>>> Третья, ещё более интересная цитата
```

Результатом использования данной конструкции будет:
> *Это цитата*
>> *Вторая интересная цитата*
>>> *Третья,ещё более интересная цитата*
