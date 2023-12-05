# [Bandit Level 2 → Level 3](https://overthewire.org/wargames/bandit/bandit3.html)

## Мета рівня

> Пароль для наступного рівня зберігається у файлі **spaces in this filename**, який знаходиться в домашній директорії.

## Команди, які можуть допомогти у вирішенні цієї задачі

| Команда                                        | Пояснення
|:---                                            | :---
| [ls](https://man7.org/linux/man-pages/man1/ls.1.html) | Виводить список вмісту каталогу (директорії)
| [cd](https://man7.org/linux/man-pages/man1/cd.1p.html) | Змінює робочу директорію
| [cat](https://man7.org/linux/man-pages/man1/cat.1.html) | Об'єднує файли та виводить їх на стандартний вивід
| [file](https://man7.org/linux/man-pages/man1/file.1.html) | Визначає тип файлу
| [du](https://man7.org/linux/man-pages/man1/du.1.html) | Оцінює місце на диску, яке займає файл
| [find](https://man7.org/linux/man-pages/man1/find.1.html) | Шукає файли в ієрархії каталогів (директорій)

## Рішення

### Крок 1
Підключаємося по ssh до bandit2:

`$ ssh -l bandit2 -p 2220 bandit.labs.overthewire.org`

### Крок 2
<!-- Вивести зміст файлу `-` за допомогою команди `cat -` не вдається.\ -->
<!-- В документації бачимо, що при відсутності файлу або ж якщо файл `-`, то читається стандартний ввід. -->
<!-- Тому, до назви файлу треба додати [абсолютний шлях](https://en.wikipedia.org/wiki/Path_(computing)), а саме `./-`: -->
Якщо спробувати вивести зміст файлу як минулого разу, то не вийде.\
Отримаємо помилку **No such file or directory**.\
Натомість, потрібно взяти файл у лапки (пр. `""` або `''`), для того щоб вказати, що назва з пробілами належить до одного файлу:

`$ cat 'cat spaces in this filename'`

## Результат
Копіюємо пароль та біжимо на наступний [рівень](https://overthewire.org/wargames/bandit/bandit4.html)!

<!-- entry pass rRGizSaX8Mk1RTb1CNQoXTcYZWU6lgzi -->
<!-- next pass aBZ0W5EmUfAf7kHTQeOwd8bauFJ2lAiG -->