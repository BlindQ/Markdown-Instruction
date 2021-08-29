##### <a name="Markdown"></a>
# :one: Что такое Markdown?
Markdown - это облегченный язык разметки созданный с целью обозначения форматирования в простом тексте, с максимальным сохранением его читаемости человеком, и пригодный для машинного преобразования в языки для продвинутых публикаций[1](https://ru.wikipedia.org/wiki/Markdown).</br>
Документы, созданные при помощи Markdown универсалены и легко конвертируемы. Они представляют из себя обычные текстовые файлы (.txt), а это означает, что их можно открыть в любом текстовом редакторе на любой платформе. Помимо этого, документы Markdown, могут быть конвертированые во многие другие удобные форматы, такие как: PDF, DOC, ODT, HTML.</br>


Однако главной особенностью данного языка можно считать максимально простой синтаксис, который служит для упрощения написания и чтения кода разметки, что, в свою очередь, позволяет легко его корректировать. Именно об основных правилах синтаксиса Markdown и будет описано в данной инструкции.
# Содержание
+ [Что такое Markdown?](#Markdown)
+ [Синтаксис заголовков](#Heading)
+ [Форматирование текста](#Text_Formatting)
+ [Цитирование](#Citation)
+ [Выделение текста](#Text_Highlighting)
+ 


##### <a name="Heading"></a>
# :two: Синтаксис заголовков

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

>*Количество           пробелов    не имеет                никакого значения
Одинарный перевод*

Для нормализации формирования абзацев можно использовать один из двух механизмов. В основе первого лежит использование двойного отступа при помощи клавиши `Enter`, что будет создавать видимый разрыв. Если существует необходимость перехода на новую строку без данного разрыва - можно разместить закрывающий тэг `</br>` в конце текста. Например разметка Markdown:

```
Первый абзац</br>
Второй абзац


Третий абзац с разрывом
```
Будет выглядет следующим образом:


>*Первый абзац</br>
Второй абзац*


>*Третий абзац с разрывом*


##### <a name="Citation"></a>

# Цитирование
Обозначение цитат в Markdown производится с помощью символа больше («>»). Цитаты отличаются от обычного текста специальным выделением, и отлично подходят для вставки дополнительной информации в исходный текст. Синтаксис Markdown поддерживает вложенное цитирование с количеством уровней равным пятнадцати. Пример цитирования представлен ниже:

```
> Это цитата
>> Вторая интересная цитата
>>> Третья, ещё более интересная цитата
```

Результатом использования данной конструкции будет:
> *Это цитата*
>> *Вторая интересная цитата*
>>> *Третья,ещё более интересная цитата*

##### <a name="Text_Highlighting"></a>

# Выделение текста

В Markdown существует несколько возможностей для выделения текста. Как и вклассических текстовых редакторов поддерживается:
1. *курсивное выделение* 
2. **жирное выделение**
3. ~~зачеркивание~~
4. ***жирное и курсивное выделение***
5. ~~***комбинированное выделение***~~
6. `изменение подложки`

Для выделения текста курсивом может использоваться одна из двух конструкций. В первой используется символ («\*») в начале и конце выделяемого отрывка. Во втором меняется лишь используемый символ на («\_»). Пример использования в разрезе синтаксиса Markdown:

```
*Курсивный шрифт*

_Альтернативный курсивный шрифт_
```

В результате на экране появится следующее:

>*Курсивный шрифт*</br>
_Альтернативный курсивный шрифт_


Жирное выделение реализуется аналогичным механизмом. Изменяется лишь количество специальных символов в начале и конце выделяемого отрывка текста. В этом случае число символов («\*») или («\_») становится равным двум. Пример:

```
**Жирный шрифт*


__Альтернативный жирный шрифт__
```

Результат выполнения:

>**Жирный шрифт**</br>
__Альтернативный жирный шрифт__


В случае, если некоторую часть в курсивном тексте необходимо сделать жирным, следует воспользоваться наличием двух различных специальных символов, выполняющих одну и ту же функцию. В качестве примера можно привести текст:

```
*Данный текст необходимо сделать __курсивным__, ведь по другому быть не может*
```

Что даст в результате:

>*Данный текст необходимо сделать __курсивным__, ведь по другому быть не может*

Зачеркивание части текста производится при помощи двух подряд идущих символов тильда («\~~»). В качестве примера приведён следующая часть текста:
```
~~Данная операция поддерживается только в версии 7.0.0.1~~ 
```

В результате выполнения получится:</br>
>~~Данная операция поддерживается только в версии 7.0.0.1~~ 

Для выделения частей кода, либо для простого изменения цвета подложки текста следует использовать символ апострофа («`») в начале и конце выделяемого участка текста. Так же существует возможность блочного выделения. Для этого можно в начале и конце абзаца поставить три подряд идущих апострофа («```»). При этом в некоторых редакторах поддерживается возможность проверки синтаксиса языка программирования, если он используется в выделяемом участке текста. Для этого в начале абзаца после трёх символов апострофа можно написать название языка программирования.

```
' Изменение подложки в рамках одной строки '

 ```
Изменение подложки
в рамках
нескольких строк

 ```
```
