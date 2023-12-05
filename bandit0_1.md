# [Bandit Level 0 → Level 1](https://overthewire.org/wargames/bandit/bandit1.html)

## Мета рівня

> Пароль для наступного рівня зберігається у файлі під назвою **readme**, який розташований в домашньому каталозі. Використайте цей пароль щоб залогінитись в bandit1 за допомогою SSH. Щоразу, коли знаходите пароль для рівня, використовуйте SSH (порт 2220), щоб увійти на цей рівень та продовжити гру.

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
Підключаємося по ssh до bandit0:

`$ ssh -l bandit0 -p 2220 bandit.labs.overthewire.org`

### Крок 2
Виводимо зміст файлу `readme`:

`$ cat readme`

## Результат
Копіюємо пароль та біжимо на наступний [рівень](https://overthewire.org/wargames/bandit/bandit2.html)!

<!-- next pass NH2SXQwcBdpmTEzi3bvBHMM9H66vVXjL -->