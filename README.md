##### <a name="Markdown"></a>
# :one: Что такое Markdown?
Markdown - это облегченный язык разметки созданный с целью обозначения форматирования в простом тексте, с максимальным сохранением его читаемости человеком, и пригодный для машинного преобразования в языки для продвинутых публикаций[[1]](https://ru.wikipedia.org/wiki/Markdown).</br>
Документы, созданные при помощи Markdown универсалены и легко конвертируемы. Они представляют из себя обычные текстовые файлы (.txt), а это означает, что их можно открыть в любом текстовом редакторе на любой платформе. Помимо этого, документы Markdown, могут быть конвертированые во многие другие удобные форматы, такие как: PDF, DOC, ODT, HTML.</br>


Однако главной особенностью данного языка можно считать максимально простой синтаксис, который служит для упрощения написания и чтения кода разметки, что, в свою очередь, позволяет легко его корректировать. Именно об основных правилах синтаксиса Markdown и будет описано в данной инструкции.
# Содержание
+ [Что такое Markdown?](#Markdown)
+ [Синтаксис заголовков](#Heading)
+ [Форматирование текста](#Text_Formatting)
+ [Цитирование](#Citation)
+ [Выделение текста](#Text_Highlighting)
+ [Нумерация](#Numbering)
+ [Создание таблиц](#Tables_Creating)
+ [Экранирование символов](#Escaping_characters)
+ [Создание таблиц](#Tables_Creating)
+ [Гиперссылки](#Hyperlinks)
+ [Вставка медиаконтента](#Media)



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
`Изменение подложки в рамках одной строки`

 ```
Изменение подложки
в рамках
нескольких строк
 ```
 
 ```python
def between_markers(text: str, begin: str, end: str) -> str:
    return(text[text.index(begin)+1:text.index(end)])



if __name__ == '__main__':
    print('Example:')
    print(between_markers('What is >apple<', '>', '<'))
 ```
 
```

Результат выполнения будет соответствующим:

>`Изменение подложки в рамках одной строки`

```
Изменение подложки
в рамках
нескольких строк
```

```python
def between_markers(text: str, begin: str, end: str) -> str:
    return(text[text.index(begin)+1:text.index(end)])



if __name__ == '__main__':
    print('Example:')
    print(between_markers('What is >apple<', '>', '<'))
```

##### <a name="Numbering"></a>

# Нумерация

Для создания нумерованного списка в языке разметки Markdown предусмотрен следующий механизм: перед каждым пунктом ставится числовое значение, условный номер пункта, обязательно оканчивающийся точкой. При этом не имеет значение порядок идущих чисел, ведь Markdown самостоятельно пронумерует их в правильном порядке. Так же поддерживается и вложенная нумерация списков. Для этого необходимо произвести дополнительный отсутуп (4 пробела), от начала строки, после предыдущего нумерованного пункта. Например нумерованный список:

```
1. Первый пункт
2. Второй пункт
    1. Второй пункт, первый подпункт
    2. Второй пункт, второй подпункт
4. Специально пропущенный третий пункт всё равно окажется на своём месте
```

При выполнении приобретёт следующий вид:

1. Первый пункт
2. Второй пункт 
    1. Второй пункт, первый подпункт
    2. Второй пункт, второй подпункт
4. Специально пропущенный третий пункт всё равно окажется на своём месте

В Markdown так же есть возможность создавать списки без нумерации. Для этого вместо числовых значений следует использовать символ дефис («-») или звуздочку («\*»). Следовательно ненумерованный список:
```
* Первый пункт
- Второй пункт
```

Будет выглядеть следующим образом:
* Первый пункт
- Второй пункт


##### <a name="Escaping_characters"></a>

# Экранирование символов
Чтобы вставить спецсимвол, используемый в разметке, как обычный символ, его нужно предварить символом обратного слэша («\»). Экранироваться должны следующие символы: `* _ { } [ ] ( ) # + - . !`. Например, следующие два текста будут отражаться по-разному:

```
*Это жирный текст*</br>
\*Это не жирный текст*
```

В результате получится:

>*Это курсивный текст*</br>
\*Это не курсивный текст*\

##### <a name="Tables_Creating"></a>

# Создание таблиц

Markdown поддерживает возможность разметки таблиц. Для этого используются вертикальные линии («|») для обозначения столбцов, и символы дефис («-») для отделения шапки таблицы. Внутри таблиц так же имеется возможность выбрать тип выравнивания:
- По левому краю
- По центру
- По правому краю

Для этого, при отделении шапки таблицы, может использоваться одна из трёх конструкций, содержащая двоеточие («:»). Выравнивание по левому краю используется по умолчанию, и не требует использования специального символа. Выравнивание по центру требует использование символа двоеточие в начале и конце в местае отделения шапки от тела таблицы. А выравнивание по правому краю требует использование двоеточия только в конце. Для удобного понимания синтаксиса таблиц будет представлен следующий пример:

```
| Первый столбец       | Второй столбец              | Третий столбец |
| -------------------- |:---------------------------:| --------------:|
| Тут будет выравнивание по левому краю     | Тут будет выравнивание по центру    |  Тут будет выравнивание по правому краю. Для этого добавим больше текста|
| Тут будет выравнивание по левому краю   | Тут будет выравнивание по центру |   Тут будет выравнивание по правому краю. Для этого добавим больше текста |
| Тут будет выравнивание по левому краю | Тут будет выравнивание по центру     |   Тут будет выравнивание по правому краю. Для этого добавим больше текста |
```

В результате будет сформирована следующая таблица:

| Первый столбец       | Второй столбец              | Третий столбец |
| -------------------- |:---------------------------:| --------------:|
| Тут будет выравнивание по левому краю     | Тут будет выравнивание по центру    |  Тут будет выравнивание по правому краю. Для этого добавим больше текста|
| Тут будет выравнивание по левому краю   | Тут будет выравнивание по центру |   Тут будет выравнивание по правому краю. Для этого добавим больше текста |
| Тут будет выравнивание по левому краю | Тут будет выравнивание по центру     |   Тут будет выравнивание по правому краю. Для этого добавим больше текста |

##### <a name="Hyperlinks"></a>

# Гиперссылки
Гиперссылка в основе своей содержит две части - основную текстовую и ссылочную. Первая - это то что отражается на экране, а вторая - сетевой путь, куда приведён нажатие на данную ссылку. Следовательно в синтаксисе Markdown необходимо разметить обе части гиперссылки. Текстовая часть ссылки заключается в квадратные скобки («\[]»), а ссылочная - в круглые(«()»). Между этими частями не должно быть пробелов или других символов. Если есть необходимость, вставить всплывающий текст при наведении - его следует указать в кавычках после ссылки в круглых скобках. Существует возможность создания сносок в тексте. Это очень удобно, если ссылка длинная, и мешает читаемости исходного текста. Для этого после текстовой части ставятся ещё одни квадратные скобки, внутри которых можно написать число сноски, а в конце текста связать данное число с итоговой ссылкой, при помощи присваивания символом («:»). Рассмотрим несколько примеров:

```
Советую перейти на [сайт](google.com "Сайт гугл")

Советую перейти на [сайт][1]

[1]:(google.com)
```

В результате получится следующее:

>Советую перейти на [сайт](https://google.com "Сайт гугл")</br>
>Советую перейти на [сайт][1]

[1]: https://google.com

##### <a name="Media"></a>

# Вставка медиаконтента

Схожим, с размещением гиперссылок, образом, производится установка изображений в тексте. Для этого в качестве ссылки следует использовать относительный или абсолютный путь до картинки, а перед текстовой части гиперссылки нужно установить восклицательный знак («!») Например:

```
![Лого Markdown](https://upload.wikimedia.org/wikipedia/commons/thumb/3/37/Markdown-mark-solid.svg/1200px-Markdown-mark-solid.svg.png)
```

В результате на экране появится следующее изображение:</br>
>![Лого Markdown](https://upload.wikimedia.org/wikipedia/commons/thumb/3/37/Markdown-mark-solid.svg/1200px-Markdown-mark-solid.svg.png)

Аналогичным образом можно производить вставку gif-анимаций. 

Так же Markdown поддерживает использование эмоджи. Процесс их размещения схож с аналогичными из Discord. Кодовое слово эмоджи следует разместить между символами двоеточия. Например:

```
:man:
```

В результате даст:

> :man:
