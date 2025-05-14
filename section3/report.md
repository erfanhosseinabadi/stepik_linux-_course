---
title: "Отчёт по заданиям Stepik"
subtitle: "Раздел 1: Введение в Linux"
author: "Ерфан Хосейнабади"

## Generic options
lang: ru-RU
toc-title: "Содержание"

## Bibliography
bibliography: bib/cite.bib
csl: pandoc/csl/gost-r-7-0-5-2008-numeric.csl

## PDF output format
toc: true # Table of contents
toc-depth: 2
lof: true # List of figures
lot: true # List of tables
fontsize: 12pt
linestretch: 1.5
papersize: a4
documentclass: scrreprt

## I18n polyglossia
polyglossia-lang:
  name: russian
  options:
    - spelling=modern
    - babelshorthands=true
polyglossia-otherlangs:
  name: english

## Fonts
mainfont: IBM Plex Serif
romanfont: IBM Plex Serif
sansfont: IBM Plex Sans
monofont: IBM Plex Mono
mathfont: STIX Two Math
mainfontoptions: Ligatures=Common,Ligatures=TeX,Scale=0.94
romanfontoptions: Ligatures=Common,Ligatures=TeX,Scale=0.94
sansfontoptions: Ligatures=Common,Ligatures=TeX,Scale=MatchLowercase,Scale=0.94
monofontoptions: Scale=MatchLowercase,Scale=0.94,FakeStretch=0.9

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

## Pandoc-crossref LaTeX customization
figureTitle: "Рис."
tableTitle: "Таблица"
listingTitle: "Листинг"
lofTitle: "Список иллюстраций"
lotTitle: "Список таблиц"
lolTitle: "Листинги"

## Misc options
indent: true
header-includes:
  - \usepackage{indentfirst}
  - \usepackage{float} # keep figures where there are in the text
  - \floatplacement{figure}{H} # keep figures where there are in the text
---

# Выполнение заданий

## 1. Используемые операционные системы
![Выбор операционных систем](image/1.png){#fig:001 width=70%}

**Ответ:** Linux, Windows  
**Обоснование:** На скриншоте (рис. \ref{fig:001}) показан выбор двух операционных систем для работы, что подтверждает их совместное использование.

## 2. Определение виртуальной машины
![Вопрос о виртуальных машинах](image/2.png){#fig:002 width=70%}

**Ответ:** Специальная программа для запуска одной ОС внутри другой  
**Обоснование:** Рис. \ref{fig:002} демонстрирует правильное определение виртуальной машины как среды для запуска гостевой ОС.

## 3. Сохранение файла в формате FODT
![Экспорт документа](image/3.png){#fig:003 width=70%}

**Ответ:** Файл `gello_linux.fodt` успешно сохранен  
**Обоснование:** Как видно на рис. \ref{fig:003}, документ был экспортирован в открытый формат FODT с именем `gello_linux.fodt`, что подтверждается сообщением об успешной загрузке.

## 4. Формат пакетов в Ubuntu
![Вопрос о пакетах](image/4.png){#fig:004 width=70%}

**Ответ:** .deb  
**Обоснование:** На рис. \ref{fig:004} показан стандартный формат пакетов для дистрибутивов на основе Debian, включая Ubuntu.


### 5. Автор VLC  
![Информация о VLC](image/5.png){#fig:005 width=70%}  
**Ответ:** Denis-Courmont  
**Обоснование:** Указано в разделе "About" программы.  

---  

### 6. Функции Update Manager  
![Update Manager](image/6.png){#fig:006 width=70%}  
**Ответ:**  
- Обновление системы до новой версии.  
- Установка новых программ.  
- Обновление установленного ПО.  
**Обоснование:** Это основные задачи менеджера обновлений в Linux.  

---  

### 7. Термины для командной строки  
![Командная строка](image/7.png){#fig:007 width=70%}  
**Ответ:** Терминал, Консоль.  
**Обоснование:** Оба термина корректны для интерфейса командной строки.  

---  

### 8. Команда `pwd`  
![Вывод pwd](image/8.png){#fig:008 width=70%}  
**Ответ:** `pwd`  
**Обоснование:** Команда выводит текущий рабочий каталог (Print Working Directory).  

---  

### 9. Эквиваленты команды `ls`  
![Варианты ls](image/9.png){#fig:009 width=70%}  
**Ответ:**  
- `ls -Ah /some/directory`  
- `ls --human-readable -A -l /some/directory`  
**Обоснование:** Флаги `-A` (показывать скрытые файлы), `-h` (читаемый размер) и `-l` (длинный формат) эквивалентны.  

---  

### 10. Абсолютный и относительный пути  
![Пути к файлам](image/10.png){#fig:010 width=70%}  
**Ответ:**  
- `ls ./../Downloads` (относительный).  
- `ls /home/bi/Downloads` (абсолютный).  
**Обоснование:** Оба пути ведут к папке Downloads пользователя `bi`.  

---  

### 11. Удаление директорий  
![Команда rm](image/11.png){#fig:011 width=70%}  
**Ответ:** `rm -r`  
**Обоснование:** Флаг `-r` (рекурсивно) удаляет каталоги с содержимым.  

---  

### 12. Завершение работы терминала  
![Команда exit](image/12.png){#fig:012 width=70%}  
**Ответ:** Терминал закроется, Firefox останется работать.  
**Обоснование:** `exit` завершает сеанс терминала, но фоновые процессы не затрагиваются.  

---  

### 13. Запуск процесса в фоне  
![Управление процессами](image/13.png){#fig:013 width=70%}  
**Ответ:** Запуск, затем `Ctrl+Z` + `bg`.  
**Обоснование:** Комбинация приостанавливает процесс (`Ctrl+Z`) и возобновляет его в фоне (`bg`), аналогично `&`.  

---  

### 14. Исполнение скрипта  
![Вывод скрипта](image/14.png){#fig:014 width=70%}  
**Ответ:**  
```  
2025-05-12 17:07:26  
Control sum: 950  
```  
**Обоснование:** Скрипт выполнен после назначения прав (`chmod +x`).  

---  

### 15. Поток `stderr`  
![Стандартный поток ошибок](image/15.png){#fig:015 width=70%}  
**Ответ:** Выводится на экран.  
**Обоснование:** По умолчанию ошибки (`stderr`) направляются в терминал.  

---  

### 16. Перенаправление `stderr` в файл  
![Перенаправление ошибок](image/16.png){#fig:016 width=70%}  
**Ответ:**  
- `program 2> file.txt`  
- `program >> file.txt 2>&1`  
**Обоснование:** Первый вариант записывает только ошибки, второй — добавляет вывод и ошибки в конец файла.  

---  

### 17. Конвейер и `stderr`  
![grep и pipe](image/17.png){#fig:017 width=70%}  
**Ответ:** Ошибки выводятся в терминал.  
**Обоснование:** Конвейер (`|`) передаёт только `stdout`, `stderr` остаётся в терминале.  

---  

### 18. Скачивание файла через `wget`  
![Загрузка файла](image/18.png){#fig:018 width=70%}  
**Ответ:** `/home/alex/1.jpg`  
**Обоснование:** Файл сохранён в домашней директории пользователя `alex`.  

---  

### 19. Тихий режим `wget`  
![Подавление вывода](image/19.png){#fig:019 width=70%}  
**Ответ:** `-q` или `--quiet`  
**Обоснование:** Эти флаги отключают вывод лога загрузки.  

---  

### 20. Рекурсивная загрузка изображений  
![wget -r](image/20.png){#fig:020 width=70%}  
**Ответ:** Будут загружены только `.jpg` файлы.  
**Обоснование:** Флаг `-A jpg` фильтрует файлы по расширению.  

---  

### 21. Удаление оригинала `gzip`  
![Сжатие gzip](image/21.png){#fig:021 width=70%}  
**Ответ:** `gzip` удаляет исходный файл после сжатия.  
**Обоснование:** Это стандартное поведение утилиты.  

---  

### 22. Архивирование директорий  
![tar и zip](image/22.png){#fig:022 width=70%}  
**Ответ:** `tar`, `zip`  
**Обоснование:** Обе утилиты поддерживают создание архивов.  

---  

### 23. Опции `tar` для bzip2  
![tar -cjf](image/23.png){#fig:023 width=70%}  
**Ответ:** `-cjf`  
**Обоснование:**  
- `-c` — создать архив.  
- `-j` — использовать bzip2.  
- `-f` — указать имя файла.  

---  

### 24. Маски поиска файлов  
![Шаблоны имён](image/24.png){#fig:024 width=70%}  
**Ответ:**  
- `alexey.*`  
- `*.jpg`  
**Обоснование:** Маски соответствуют имени и расширению целевого файла.  

---  

### 25. Поиск слова `world`  
![Команда grep](image/25.png){#fig:025 width=70%}  
**Ответ:**  
- The world is not enough  
- The "world" is not enough  
- world  
- The beautiful-world is not enough  
**Обоснование:** Все варианты содержат искомое слово (регистронезависимо).  

---  

## Выводы  
В ходе работы освоены ключевые аспекты работы в Linux:  
- Управление файлами и директориями.  
- Перенаправление потоков ввода/вывода.  
- Использование утилит (`wget`, `grep`, `tar`).  
- Поиск и фильтрация данных.  
Приобретённые навыки позволяют эффективно решать задачи администрирования и автоматизации.  
```  
