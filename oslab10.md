---
# Front matter
title: "Лабораторная работа 10"
subtitle: "Отчёт"
author: "Новосельцев Данила Сергеевич"

# Generic otions
lang: ru-RU
toc-title: "Содержание"

# Bibliography
bibliography: bib/cite.bib
csl: pandoc/csl/gost-r-7-0-5-2008-numeric.csl

# Pdf output format
toc: true # Table of contents
toc_depth: 2
lof: true # List of figures
lot: true # List of tables
fontsize: 12pt
linestretch: 1.5
papersize: a4
documentclass: scrreprt
## I18n
polyglossia-lang:
  name: russian
  options:
	- spelling=modern
	- babelshorthands=true
polyglossia-otherlangs:
  name: english
### Fonts
mainfont: PT Serif
romanfont: PT Serif
sansfont: PT Sans
monofont: PT Mono
mainfontoptions: Ligatures=TeX
romanfontoptions: Ligatures=TeX
sansfontoptions: Ligatures=TeX,Scale=MatchLowercase
monofontoptions: Scale=MatchLowercase,Scale=0.9
## Biblatex
biblatex: true
biblio-style: "gost-numeric"
biblatexoptions:
  - parentracker=true
  - backend=biber
  - hyperref=auto
  - language=auto
  - autolang=other*
  - citestyle=gost-numeric
## Misc options
indent: true
header-includes:
  - \linepenalty=10 
  - \interlinepenalty=0 
  - \hyphenpenalty=50 
  - \exhyphenpenalty=50 
  - \binoppenalty=700 
  - \relpenalty=500 
  - \clubpenalty=150 
  - \widowpenalty=150 
  - \displaywidowpenalty=50 
  - \brokenpenalty=100 
  - \predisplaypenalty=10000 
  - \postdisplaypenalty=0 
  - \floatingpenalty = 20000 
  - \raggedbottom 
  - \usepackage{float} 
  - \floatplacement{figure}{H} 
---

# Лабораторная работа 10
 Новосельцев.Д.С. 
 НФИбд-02-20

---

Цель работы: 
познакомиться с операционной системой Linux, получить практические навыки работы с редактором Emacs.

---

Ход работы:

1.Открыл emacs.

2.Создал файл lab07.sh с помощью комбинации Ctrl-x Ctrl-f (C-x C-f).

![](https://imgur.com/GNolh7z.png)

3.Набрал текст:

#!/bin/bash

HELL=Hello

function hello {

LOCAL HELLO=World

echo $HELLO

}

echo $HELLO

hello

![](https://imgur.com/eK3HmMx.png)

4. Сохранил файл с помощью комбинации Ctrl-x Ctrl-s (C-x C-s).

5. Проделал с текстом стандартные процедуры редактирования, каждое действие осуществлялось комбинацией клавиш.

5.1. Вырезал одной командой целую строку (С-k).

![](https://imgur.com/hHkpt0r.png)

5.2. Вставил эту строку в конец файла (C-y).

![](https://imgur.com/j2ENHkb.png)

5.3. Выделил область текста (C-space).

![](https://imgur.com/yPmN4kF.png)

5.4. Скопировал область в буфер обмена (M-w).

5.5. Вставил область в конец файла.

![](https://imgur.com/0n4JnX5.png)

5.6. Вновь выделил эту область и на этот раз вырезал её (C-w).

![](https://imgur.com/cd3DFy0.png)

5.7. Отменил последнее действие (C-/).

![](https://imgur.com/AH58xO8.png)

6. Научился использовать команды по перемещению курсора.

6.1. Переместил курсор в начало строки (C-a).

6.2. Переместил курсор в конец строки (C-e).

6.3. Переместил курсор в начало буфера (M-<).

![](https://imgur.com/btCcFeX.png)

6.4. Переместил курсор в конец буфера (M->).

![](https://imgur.com/4aHn9es.png)

7. Управление буферами.

7.1. Вывел список активных буферов на экран (C-x C-b).

![](https://imgur.com/pDjBC9F.png)

7.2. Переместился во вновь открытое окно (C-x) o со списком открытых буферов и переключился на другой буфер.

![](https://imgur.com/tukcYDH.png)

7.3. Закрыл это окно (C-x 0).

7.4. Вновь переключился между буферами, но без вывода их списка на экран (C-x b).

![](https://imgur.com/sgZg8cK.png)

8. Управление окнами.

8.1. Поделил фрейм на 4 части: разделил фрейм на два окна по вертикали
(C-x 3), а затем каждое из этих окон на две части по горизонтали (C-x 2).

![](https://imgur.com/WEstZTL.png)
![](https://imgur.com/GRh8YAP.png)

8.2. В каждом из четырёх созданных окон открыл новый буфер (файл) и ввел несколько строк текста.

![](https://imgur.com/Dk5dWR6.png)

9. Режим поиска

9.1. Переключился в режим поиска (C-s) и нашёл несколько слов, присутствующих в тексте.

![](https://imgur.com/KvZZ4Qw.png)

9.2. Переключался между результатами поиска, нажимая C-s.

![](https://imgur.com/nJYQbBR.png)

9.3. Вышел из режима поиска, нажав C-g.

![](https://imgur.com/Dk5dWR6.png)

9.4. Испробовал другой режим поиска, нажав M-s o. Он отличается от обычного режима тем, что при поиске указывает номера строк в которых найдено введённое слово и выделяет их цветом. В обычном режиме выделение цветом появляется, только когда нужно подтвердить замену.

![](https://imgur.com/IICJjE1.png)

Вывод: познакомился с операционной системой Linux, получил практические навыки работы с редактором Emacs.

Ответы на контрольные вопросы:

1. Emacs представляет собой мощный экранный редактор текста, написанный на

языке высокого уровня Elisp.

2. Развитие Emacs в сторону его многогранности послужило причиной того, что и без

того интуитивно непонятная программа стала чрезвычайно сложной в применении. В частности, управление осуществляется при помощи различных клавиатурных комбинаций, запомнить которые будет непросто.

3. Буфер – что-то, состоящее из текста.

Окно – область с одним из буферов.

4. В одном окне можно открыть больше 10 буферов.

5. После запуска emacs без каких-либо параметров в основном окне отображается буфер *scratch*, который используется для оценки выражений Emacs Lisp, а также для заметок, которые вы не хотите сохранять. Этот буфер не сохраняется автоматически.

6. Чтобы ввести следующую комбинацию C-c | я нажму клавиши: Control+c и Shift+\, и для C-c C-|: Control+c и Control+Shift+\.

7. Поделить текущее окно на две части можно двумя комбинациями клавиш:

C-x 3 или C-x 2.

8. Настроить или расширить Emacs можно написав или изменив файл ~/.emacs.

9. Клавиша ß выполняет функцию перемещения курсора в открытом окне также, как и многие другие клавиши её можно переназначить.

10. Редактор emacs показался мне удобнее из-за возможности открытия нескольких окон с буферами и работать комбинациями клавиш в этот редакторе мне было проще.