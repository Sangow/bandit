# [Bandit Level 0](https://overthewire.org/wargames/bandit/bandit0.html)

## Мета рівня

> Мета цього рівня - залогінитися за допомогою SSH. Хост, до я кого треба підключитися - **bandit.labs.overthewire.org**, порт **2220**. Користувач - **bandit0**, а пароль - **bandit0**. Після входу перейти на сторінку [Рівня 1](https://overthewire.org/wargames/bandit/bandit1.html), щоб дізнатися як його ~~побити~~ перемогти.

## Команди, які можуть допомогти у вирішенні цієї задачі

| Команда                                        | Пояснення
|:---                                            | :---
| [ssh](https://linux.die.net/man/1/ssh)         | OpenSSH SSH клієнт

## Рішення

`$ ssh -l bandit24 -p 2220 bandit.labs.overthewire.org`