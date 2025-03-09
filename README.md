# Установка Git и Visual Studio Code

***Git*** — это система контроля версий, которая позволяет отслеживать любые изменения в файлах, хранить их версии и оперативно возвращаться в любое сохранённое состояние. 1

***Для чего нужен Git:***

Помогает разработчикам параллельно работать над проектом, не мешать друг другу и добавлять в основную ветку только качественный код.

Позволяет откатить текущую версию кода до предыдущей или сразу на несколько шагов назад. Это удобно, если после изменения коммита допущена ошибка.

Код хранится и на сервере, и локально, то есть на компьютерах разработчиков. Это значит, что код нельзя случайно (или специально) удалить — всегда найдётся версия, из которой можно восстановить сразу всё.

**Установка Git для Windows, MAC, Linux:** https://git-scm.com/downloads

**Установка VSCode для Windows, MAC, Linux:** https://code.visualstudio.com/Download

При первом использовании Git необходимо представиться. Для
этого нужно ввести в терминале 2 команды:

**git config --global user.name «Ваше имя английскими буквами»**

**git config --global user.email ваша почта@example.com**

# Основные команды Git

✦ git init – инициализация локального репозитория

✦ git status – получить информацию от git о его текущем состоянии

✦ git add – добавить файл или файлы к следующему коммиту

✦ git commit -m “message” – создание коммита.

✦ git log – вывод на экран истории всех коммитов с их хеш-кодами

✦ git checkout – переход от одного коммита к другому

✦ git checkout master – вернуться к актуальному состоянию и продолжить работу

✦ git diff – увидеть разницу между текущим файлом и закоммиченным файлом

# Синтаксис языка Markdown
Справочник по Markdown от Microsoft:
https://docs.microsoft.com/ru-ru/contribute/markdown-reference

✦ # Заголовок – выделение заголовков. Количество символов “#” задаёт уровень заголовка
(поддерживается 6 уровней).

✦ = или - – подчёркиванием этими символами (не менее 3 подряд) выделяют заголовки первого
(“=”) и второго (“-”) уровней.

✦ ** Полужирное начертание** или __ Полужирное начертание__

✦ *Курсивное начертание* (**) или _Курсивное начертание_ (__ __)

✦ ***Полужирное курсивное начертание*** (*** ***)

✦ ~~Зачёркнутый текст~~ (~~ ~~)

✦ * Строка – ненумерованные списки, символ “*” в начале строки

✦ 1, 2, 3 … – нумерованные списки

# Markdown
Язык разметки Markdown широко распространён в вебе. На нём пишут readme-файлы и документацию, а его принципы работы используют для оформления сообщений и публикаций в мессенджерах и социальных сетях.

Markdown легко конвертируется в HTML, открывается во всех текстовых редакторах и легко читается даже в виде исходного кода. При этом писать на нём куда проще, чем на других языках разметки: HTML, XML, TeX и так далее.
 
## Диалекты и редакторы
Базовым Markdown уже мало кто пользуется. Зато у него существуют спецификации и диалекты, которые добавляют в язык новые функции: встраивание HTML-тегов, создание таблиц и чекбоксов, зачёркивание текста, разные варианты переноса строки.

Разные редакторы Markdown могут поддерживать или не поддерживать часть новых функций — учтите это при выборе платформы, на которой будете работать.

Самый распространённый Markdown — диалект ***GitHub Flavored Markdown***, основанный на спецификации ***CommonMark***. В этой статье мы пользуемся редактором ***Markdown Editor***, который поддерживает практически все инструменты этой парочки (кроме чекбоксов).

## Параграфы и разрывы строк (paragraphs and line breaks)

Чтобы поделить текст на параграфы, между ними нужно оставить пустую строку. Строка считается пустой, даже если в ней есть пробелы и табуляции. Если же строки находятся рядом, то они автоматически склеиваются в одну.

Пример:

Первый параграф

Второй параграф
Продолжение второго параграфа

#### Для переноса строки внутри одного параграфа есть три метода:

поставить в конце строки два или больше пробела;<br>
поставить в конце строки обратную косую черту;<br>
использовать HTML-тег "br". <br>

#### Пример:
Перенос с помощью пробелов  
Перенос с помощью обратного слеша\
Перенос с помощью тега <br> Последняя строка

#### Обратите внимание, что у каждого из методов есть свои недостатки:

1. пробелы в конце строки бывает трудно заметить, и это может запутать читателя;<br>
2. обратный слеш вводится в стандарте CommonMark и может поддерживаться не всеми редакторами;<br>
3. HTML-теги в Markdown также поддерживаются не всеми редакторами.<br>
## Заголовки (headings)
В синтаксисе Markdown есть шесть уровней заголовков: от H1 (самого большого) до H6 (самого маленького). Для их выделения используют решётки #, при этом есть несколько тонкостей:

1. решётки можно ставить как перед заголовком, так и с двух сторон от него (на уровень заголовка влияют только те #, которые находятся перед ним);
2. количество решёток соответствует уровню заголовка: одна для первого уровня, две для второго и так далее;
3. между решёткой и текстом ставится пробел.

#### Пример заголовков:
# Заголовок первого уровня.
## Заголовок второго уровня .
### Заголовок третьего уровня.
#### Заголовок четвёртого уровня.
##### Заголовок пятого уровня. ############
###### Заголовок шестого уровня.

\
У заголовков первого и второго уровня есть альтернативный способ выделения: на следующей строке после них нужно поставить знаки равенства = или дефисы -. Вот несколько правил:

знак "=" применяется для заголовков H1;\
дефис применяется для заголовков H2;\
если в одной строке поставить оба знака, то работать ничего не будет;\
можно ставить любое количество знаков, и на тип заголовка это не повлияет;\
между заголовком и знаками не должно быть пустых строк.\

#### Пример:
Заголовок первого уровня
=
Заголовок первого уровня
=========
Заголовок второго уровня
-
Заголовок второго уровня
----------

&nbsp;
&nbsp;
&nbsp;

## Выделение текста (emphasis)
Чтобы изменить начертание текста, нужно выделить его с двух сторон спецсимволами следующим образом: <спецсимвол>текст<спецсимвол>.\
### Курсив (italic)
Для выделения текста курсивом нужно использовать одну звёздочку * или нижнее подчёркивание _.\
#### Пример:

*Текст курсивом*

_Текст курсивом_
### Жирный (bold)
Для выделения текста жирным нужно использовать две звёздочки ** или два нижних подчёркивания __.
#### Пример:

**Жирный текст**

__Жирный текст__

#### Обратите внимание, что если вы хотите выделить фрагмент внутри слова, то это корректно сработает только при использовании звёздочек.

#### Пример:
Кор*рек*тно, кор**рек**тно, кор***рек***тно

Некор_рек_тно, некор__рек__тно, некор___рек___тно

### Зачёркнутый (strikethrough)
Чтобы зачеркнуть текст, нужно использовать две тильды ~~. Такая опция есть только в диалекте GitHub Flavored Markdown.

~~Зачёркнутый текст~~

Отображение результата в браузере
Скриншот: Skillbox Media
### Подчёркнутый (underline)
В синтаксисе Markdown нет встроенного способа подчеркнуть текст. Но если ваш редактор поддерживает HTML, то можно использовать теги:

<u>Подчёркнутый текст</u>

Отображение результата в браузере
Скриншот: Skillbox Media
### Разделители (horizontal rules)
Чтобы оформить горизонтальный разделитель, нужно поставить три или больше специальных символа: звёздочки *, дефиса - или нижних подчёркивания _. Они должны находиться на отдельной строке, и между ними можно ставить любое количество пробелов и табуляций.

Если ваш редактор поддерживает HTML-теги, то для разметки можно также использовать тег <hr>.

***
---
___
*	*  **

Отображение результата в браузере
Скриншот: Skillbox Media
### Цитаты (blockquotes)
Чтобы параграф отобразился как цитата, нужно поставить перед ним закрывающую угловую скобку >.

> Оформление цитатой
последовательных строк
внутри одного параграфа

Отображение результата в браузере
Скриншот: Skillbox Media
Внутрь одного блока цитаты можно поместить сразу несколько параграфов и использовать любые элементы оформления. Например, заголовки и другие цитаты. Чтобы сделать это, нужно поместить закрывающую угловую скобку перед началом каждой строки.

> # Заголовок
> Первый параграф
>
> Второй параграф
>
> > Вложенная цитата
> > > Цитата третьего уровня
>
> Продолжение основной цитаты

Отображение результата в браузере
Скриншот: Skillbox Media
### Списки (lists)
В синтаксисе Markdown есть несколько видов списков. Для их оформления перед каждым пунктом нужно поставить подходящий тег и отделить его от текста пробелом.

### Нумерованные (ordered)
Для создания нумерованного списка перед пунктами нужно поставить число с точкой. При этом нумерация в разметке ленивая. Неважно, какие именно числа вы напишете: Markdown пронумерует список автоматически.

1. Первый пункт
2. Второй пункт
3. Третий пункт


1. Первый пункт
1. Второй пункт
1. Третий пункт


1. Первый пункт
73. Второй пункт
5. Третий пункт

Отображение результата в браузере
Скриншот: Skillbox Media
Список можно начинать и не с единицы. Для нумерации важно только число, которое стоит перед первым пунктом.

27. Первый пункт
27. Второй пункт
27. Третий пункт

Отображение результата в браузере
Скриншот: Skillbox Media
Обратите внимание, что между двумя нумерованными списками, идущими подряд, нужно отбить две пустые строки. Если отбить только одну, то Markdown воспримет два списка как один. Некоторые редакторы в таком случае увеличивают интервал между пунктами.

1. Первый пункт
2. Второй пункт
3. Третий пункт

1. Четвёртый пункт
2. Пятый пункт
3. Шестой пункт

Отображение результата в браузере
Скриншот: Skillbox Media
### Ненумерованные (unordered)
Для создания ненумерованного списка нужно поставить перед каждым пунктом звёздочку *, дефис - или плюс +.

* Первый пункт
* Второй пункт
* Третий пункт
- Первый пункт
- Второй пункт
- Третий пункт
+ Первый пункт
+ Второй пункт
+ Третий пункт

Отображение результата в браузере
Скриншот: Skillbox Media
Обратите внимание, что Markdown относит к разным спискам пункты, перед которыми стоят разные маркеры. Даже несмотря на то, что мы не оставляем пустых строк между списками.

Если же два списка идут подряд, а перед их пунктами стоят одинаковые маркеры, тогда между ними нужно отбить две пустые строки (как в случае с нумерованными списками).

### Чекбоксы (checkboxes)
Чтобы сделать чекбоксы, нужно использовать маркированный список, но между маркером и текстом поставить [x] для отмеченного пункта и [] — для неотмеченного.

Чекбоксы доступны в диалекте GitHub Flavored Markdown (тот самый, который умеет зачёркивать текст) и поддерживаются не всеми редакторами Markdown. Например, нам для демонстрации примера пришлось открывать другой.

- [x] Отмеченный пункт
- [ ] Неотмеченный пункт

Отображение результата в браузере
Скриншот: Skillbox Media
### Вложенные (nested)
Чтобы создать вложенный список, нужно поставить перед его пунктами табуляцию или несколько пробелов. В Markdown одна табуляция соответствует четырём пробелам.

Список одного вида можно вкладывать в любой другой.

1. Пункт
	1. Подпункт
		1. Подподпункт

- Пункт
	- Подпункт
		- Подподпункт


1. Пункт
	- Подпункт
		* Подподпункт

+ Пункт
	1. Подпункт

- Пункт
  - [x] Отмеченный подпункт
  - [ ] Неотмеченный подпункт
    1. Подподпункт

Отображение результата в браузере
Скриншот: Skillbox Media
На самом деле количество пробелов, которые нужно поставить для корректного отступа, рассчитывается чуть сложнее. Берётся количество символов в маркере (один для *, - и +, два для 1., три для 10.), и к нему прибавляется любое число от 1 до 4.

Таким образом, если в маркере 1 символ, нужно поставить от 2 до 5 пробелов, если 2 символа — от 3 до 6, если 3 символа — от 4 до 7.

### Другие элементы внутри списков
В пункты списков можно добавлять другие элементы оформления. Например, параграфы или цитаты. Для этого нужно сделать отступ, как если бы вы добавляли вложенный список.

1. Первый пункт
	> Цитата внутри первого пункта
1. Второй пункт
 	
    Параграф внутри второго пункта
1. Третий пункт

Отображение результата в браузере
Скриншот: Skillbox Media
### Ссылки (links)
Самый лёгкий способ поместить ссылку в Markdown — заключить её в угловые скобки. Несмотря на простоту, он не является основным и был добавлен только в спецификации CommonMark.

<https://skillbox.ru/media/code/>

Отображение результата в браузере
Скриншот: Skillbox Media
Чтобы оформить ссылкой часть текста, используется такой синтаксис: [текст](ссылка). Можно сделать всплывающую подсказку при наведении курсора. Для этого в круглых скобках после ссылки нужно поставить пробел и написать текст подсказки в кавычках.

[Skillbox Media](https://skillbox.ru/media/) без подсказки

[Skillbox Media](https://skillbox.ru/media/ "Всплывающая подсказка") с подсказкой

Отображение результата в браузере
Скриншот: Skillbox Media
Ещё один способ оформить ссылку — справочный. Он работает как сноски в книгах: [текст][имя сноски]. При таком способе организации ссылок в конце документа нужно также написать и оформить саму сноску: [имя сноски]: ссылка. При желании после ссылки можно добавить подсказку — точно так же, как в предыдущем методе.

Имя сноски может быть любым сочетанием символов: цифрами, буквами и даже знаками препинания. На одну и ту же сноску в тексте можно ссылаться сколько угодно раз.

Ссылки, оформленные справочным методом, выглядят и работают точно так же, как и в предыдущем способе. Сами сноски в отформатированном документе не отображаются.

[Skillbox Media][1]

[Раздел «Код»][code]


[1]: https://skillbox.ru/media "Всплывающая подсказка"
[code]: https://skillbox.ru/media/code/

Отображение результата в браузере
Скриншот: Skillbox Media
### Картинки (images)
Изображения в Markdown оформляются по принципу, схожему с принципом оформления ссылкок, только перед квадратными скобками нужно поставить восклицательный знак: ![текст](путь к изображению). Здесь также можно сделать всплывающую подсказку.

![Изображение](https://upload.wikimedia.org/wikipedia/commons/thumb/4/48/Markdown-mark.svg/1920px-Markdown-mark.svg.png "Логотип Markdown")

Отображение результата в браузере
Скриншот: Skillbox Media
Можно использовать и справочный метод: ![текст][имя сноски]. Сноски оформляются так же, как и в ссылках: [имя сноски]: путь к изображению, — в них тоже можно добавлять подсказки.

![Изображение][1]


[1]: https://upload.wikimedia.org/wikipedia/commons/thumb/4/48/Markdown-mark.svg/1920px-Markdown-mark.svg.png "Логотип Markdown"
Такая разметка выведет тот же результат, что и предыдущая.

### Вставка кода (code)
В Markdown есть несколько способов выделить исходный код:

Если надо отобразить фрагмент кода внутри строки с каким-то текстом, нужно с двух сторон выделить этот код одним или несколькими обратными апострофами (`; их ещё называют бэктиками).
Чтобы выделить фрагмент из нескольких строк, нужно с двух сторон выделить его тремя обратными апострофами.
Также перед фрагментом кода можно поставить табуляцию или четыре пробела, при этом предыдущая строка должна быть пустой.
Функция `print (x)` выводит содержимое переменной ```x```.

```
#include <stdio.h>
int main() {
   printf("Hello, World!");
   return 0;
}
```

	let x = 12;
	let y = 6;
	console.log(x + y);

Отображение результата в браузере
Скриншот: Skillbox Media
Если обрамлять код тремя обратными апострофами, то после первой тройки можно указать язык программирования — тогда Markdown правильно подсветит элементы кода.

```python
if x > 0:
	print (x)
else:
	print ('Hello, World!')
```

```c
#include <stdio.h>
int main() {
   printf("Hello, World!");
   return 0;
}
```

```javascript
let x = 12;
let y = 6;
console.log(x + y);
```

Отображение результата в браузере
Скриншот: Skillbox Media
Возможность вставлять блоки кода тремя обратными апострофами появилась в спецификации CommonMark, но там не указан список псевдонимов: как правильно называть языки, чтобы Markdown понял, о чём речь.

Поэтому каждая реализация ведёт свой собственный список языков и их псевдонимов. Так как их очень много, да ещё и новые время от времени добавляются, то удобных таблиц обычно не делают. Предлагают сразу ознакомиться с конфигурационным файлом.

Вот такой список языков, например, поддерживает диалект GitHub Flavored Markdown.

### Таблицы (tables)
В уже упомянутом выше диалекте GitHub Flavored Markdown (и некоторых других тоже) есть возможность оформлять таблицы. Столбцы разделяются вертикальными линиями |, а строка с шапкой отделяется от остальных дефисами -, которых можно ставить сколько угодно.

|Столбец 1|Столбец 2|Столбец 3|
|-|--------|---|
|Длинная запись в первом столбце|Запись в столбце 2|Запись в столбце 3|
|Кртк зпс| |Слева нет записи|

Отображение результата в браузере
Скриншот: Skillbox Media
Чтобы выровнять весь столбец по правому краю, в строке с дефисами сразу после дефисов можно поставить двоеточие :. Чтобы выровнять содержимое по центру, надо поставить двоеточия с обеих сторон.

|Столбец 1|Столбец 2|Столбец 3|
|:-|:-:|-:|
|Равнение по левому краю|Равнение по центру|Равнение по правому краю|
|Запись|Запись|Запись|

Отображение результата в браузере
Скриншот: Skillbox Media
### Экранирование (escaping characters)
Многие символы в Markdown выполняют роль служебных. Если они встречаются в вашем тексте сами по себе, то для корректного отображения их стоит экранировать (иначе они просто не только не отобразятся сами, но и добавят вашему тексту какое-нибудь ненужное форматирование). Для этого перед ними ставится обратная косая черта \.

Вот список символов, которые нужно экранировать: \`*_{}[]<>()#+-.! |. Делать это постоянно необязательно — достаточно ставить экран только в тех случаях, когда Markdown может воспринять эти символы как служебные. Например, если строка начинается с символа #, то экранировать её надо — потому что программа может решить, что вы хотите сделать заголовок. А вот если решётка находится где-то в центре строки, то экранировать ничего не надо — редактор поймёт, что тут она просто часть текста.

### Как использовать Markdown в мессенджерах
Как мы уже писали, принципы Markdown используются при разметке текста во многих мессенджерах. Обычно он используется для выделения текста, при этом синтаксис у каждой платформы свой.

Жирный:

Telegram и Discord — **две звёздочки с двух сторон**;
WhatsApp и Viber — *одна звёздочка с двух сторон*.
Курсив:

Telegram — __два нижних подчёркивания с двух сторон__;
WhatsApp и Viber — _одно нижнее подчёркивание с двух сторон_;
Discord — *одна звёздочка с двух сторон* или _одно нижнее подчёркивание с двух сторон_.
Подчёркнутый:

Discord — __два нижних подчёркивания с двух сторон__.
Зачёркнутый:

WhatsApp и Viber — ~одна тильда с двух сторон~;
Discord — ~~две тильды с двух сторон~~.
Моноширинный (используется для вставки кода):

Telegram, WhatsApp, Viber и Discord — ```три обратных апострофа с двух сторон```;
в Discord точно так же, как и в Markdown, можно указывать язык программирования для подсветки синтаксиса.
Спойлер:

Telegram и Discord — ||две вертикальные черты с двух сторон||.
### Резюмируем
Этой шпаргалки по разметке Markdown будет достаточно для создания полноценного документа. А там, где возможностей языка не хватит, можно встраивать HTML-код.

Синтаксис Markdown простой, гибкий и нетребовательный. У него есть несколько реализаций, благодаря которым в нём можно:

выделять параграфы и переносить строки,
оформлять заголовки,
изменять начертание текста,
ставить горизонтальные разделители,
выделять цитаты,
составлять списки,
прикреплять ссылки,
вставлять картинки и исходный код,
делать таблицы.
И ещё одно небольшое примечание. Если вы форматируете текст с помощью HTML-тегов или форматируете код тремя обратными апострофами, то Markdown будет автоматически пытаться искать закрывающий символ — то есть будет придумывать, куда его поставить, даже если у вас его нет. Остальные симметричные символы (*_~`) работают в пределах одной строки.
## Создание коммитов
### Git add
Для добавление изменений в коммит используется команда ```git add``` и имя файла<br>
Например, ```git add README.md```

![1](Task/1.png)
### Оправить коммит
```git commit -m "first commit"``` - команда для отправки коммита<br>
* ```git commit``` - обращение к **GIT**
* ```-m``` - добавить сообщение *(коментарий)*
* ```"first commit"``` - коментрарий *(в кавычках)*

![2](Task/2.png)
### Посмотреть список коммитов
* ```git log``` - стандартный вид


* ```git log --graph``` - вид с графическим отображением веток

![3](Task/(3.png)
### Перейти к сохранению
* ```git checkout```
* ```git checkout <номер коммита, первые 4 символа>``` - перейти к определенному изменению
* ```git master``` - перейти к изменению последнего коммита
### Посмотреть есть ли не сохранненные изменения репозитория (файлов)
* ```get status```

![4](Task/4.png)
## Работа с ветками
* ```git branch``` - посмотреть список веток

![5](Task/5.png)
* ```git branch <название ветки>``` - создать ветку (новая ветка унаследует коммиты родительской ветки)
![6](Task/6.png)
* ```git checkout <название ветки>``` - перейти на ветку
![7](Task/7.png)
* ```git branch -d <название ветки>``` - удалить ветку после merge
* ```git branch -D <название ветки>``` - удалить ветку принудительно
![8](Task/8.png)
* ```git merge <название сливаемой ветки>``` - сливание веток

## конфликт 

![9](Task/9.png)
