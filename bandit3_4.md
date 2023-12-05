# [Bandit Level 3 → Level 4](https://overthewire.org/wargames/bandit/bandit4.html)

## Мета рівня
> Пароль для наступного рівня зберігається у прихованому файлі в директорії **inhere**.

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
Підключаємося по ssh до bandit3:

`$ ssh -l bandit3 -p 2220 bandit.labs.overthewire.org`

### Крок 2
Переходимо у директорію **inhere**:

`$ cd inhere`

### Крок 3
Дивимося вміст директорії за допомогою команди `ls`.\
`$ ls`\
Нічого не сталося, так як вище сказано, що файл прихований.\
Для цього, як пише мануал, треба додати параметр, який **не ігнорує** файли, які починаються з `.`, тобто приховані:\
`$ ls -a`\
**аутпут:** `.  ..  .hidden`\
Ми отримали назву файлу.

### Крок 4
Виводимо зміст файлу:

`$ cat .hidden`

## Результат
Копіюємо пароль та біжимо на наступний [рівень](https://overthewire.org/wargames/bandit/bandit5.html)!

<!-- entry pass aBZ0W5EmUfAf7kHTQeOwd8bauFJ2lAiG -->
<!-- next pass 2EW7BBsr6aMMoJ2HjW067dm8EgX26xNe -->