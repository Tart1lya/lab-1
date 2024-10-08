## Отчёт по лабораторной работе №1

1. Сначала создаю файл с именем `script.bash`
```bash
touch script.bash
```
2. Далее, так как у меня macOS, открываю TextEdit для редактирования файла `script.bash` и вписываю следующий скрипт:
```bash
#!/bin/bash

echo "Welcome to ITMO University"
```
3. После этого сохраняю этот файл и запускаю bash-скрипт в терминале:
```bash
bash script.bash
```

![image](https://github.com/user-attachments/assets/13004fb0-32e9-4448-aba4-06a4b2b6c113)

4. Далее нужно решить следующую задачу:

Модифицируйте файл `script.bash` так, чтобы при его запуске в терминале в виде

```bash
bash script.bash Vasya Pupkin
```

Вывод был

`Welcome, Vasya Pupkin`

*Hint:* Скрипт должен работать для любых имен, даже если это Benedict Timothy Carlton Cumberbatch.

## Решение

Я воспользовался дополнительными источниками информации. Чтобы решить данную задачу нам нужно:

1. Снова открыть с помощью TextEdit файл `script.bash`
2. Далее объявляем переменную, в которой будет храниться имя, которое будет выводится в терминале. Обозначим эту переменную как `name`
3. После этого присваиваем переменной имя, которое хотим вывести в терминале
```bash
name="Vasya Pupkin"
```
4. Далее пишем следующую команду
```bash
echo "Welcome, $name"
```
Благодаря значку доллара, мы можем в строку, которую мы будем выводить, вставить переменную. Данный метод вывода переменных вместе с текстом мне напомнил вывод в Kotlin'е, где мы так же используем значок доллара, чтобы вывести переменную вместе с текстом.

И вот что мы получаем при запуске данного скрипта:
![image](https://github.com/user-attachments/assets/9f4accdf-be61-4afc-9244-e7e29855fc97)

И даже с такими значениями работает
![image](https://github.com/user-attachments/assets/a0b099d8-730d-47f9-98c0-5f9daeb0a172)

