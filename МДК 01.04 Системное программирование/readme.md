# ЛК_1 15.01.24
[Установка git bash](https://git-scm.com/downloads)
---
[Практические задания по гит](https://smartiqa.ru/courses/git/answer-key)
---

``git bash`` - это команды для работы с гит из терминала  

**Прокси сервер** `git config --global http.proxy 10.0.50.52:3128`

![image](https://github.com/Katya6589/Semestr_6/assets/113089569/c0294fda-6f7f-4037-8034-da1bb7b16124)

Создаие репозитория на компьтере:
--
- инициализация `git init`
![image](https://github.com/Katya6589/Semestr_6/assets/113089569/ec7edef9-c3e8-4f7f-9d86-b798ea09cd96)

`$ cmd //c tree .git` - показывает структуру папки гит
  ![image](https://github.com/Katya6589/Semestr_6/assets/113089569/608a3012-6924-4146-af07-e0ce620481cb)

---
`$ git status` - (показывает статус репозитория)  
`On branch master` - (указывает имя ветки)  

`No commits yet` - (нет созраненных версий)  

`Untracked files:` - (не отслеживымаемые файлы)  
 ` (use "git add <file>..." to include in what will be committed)` - (нужна комнда "добавить", чтобы зафиксировать версию для сохранения)  
  Список файлов для добавления (внизу 2 строки):   
          `index.html`  
          `pictures/`  

`nothing added to commit but untracked files present (use "git add" to track)` - (найдены файлы для добавления)  

![image](https://github.com/Katya6589/Semestr_6/assets/113089569/e9721c78-4316-4316-9d7f-e8fbddb1b505)

---


Настраиваем пользователя Git
--
Задаем имя и email пользователя для текущего репозитория 23-12 303-15  
`$ git config --global user.name PK303-13`  
`$ git config --global user.email PK303-13@gmail.com`  

Отменяет прокси сервер:  
`git config --global --unset http.proxy`  
`git config --global --unset https.proxy`  
`git config --global --unset core.gitproxy`  

Добавление файла ( * - все файлы):  
`$ git add *`  
![image](https://github.com/Katya6589/Semestr_6/assets/113089569/598d2c69-8f14-4ef0-ae22-702c72f8c942)

Для фиксации версии нужно указать ее название, для этого созддается сообщение (`-m`)    
`git commit -m "G-02: Initial"`    

Выводим информмацию о фиксации:  
`$ git log`  
![image](https://github.com/Katya6589/Semestr_6/assets/113089569/0970f675-d68b-43bc-ab9a-2fa8a9e06c4f)

Подтверждение 
---
![image](https://github.com/Katya6589/Semestr_6/assets/113089569/b59cc504-ae7a-49c9-bd49-0ab906c9d6fe)
![image](https://github.com/Katya6589/Semestr_6/assets/113089569/ea43f864-8177-4e16-a16c-8ab24a551ed8)

![image](https://github.com/Katya6589/Semestr_6/assets/113089569/d3f951bf-a460-4699-bf34-6eab5625123f)  

Основные ошибки:  
--
1. `remote` - подлючение к удаленному репозиторию (показывает на какой репозиторий мы хотим сохарнить данные). Может быть ошибка, что неправильно указали ссылку, чтобы изменить надо добавить `set url`
2. Авторизация - гит хабу нужно передать данные пользователя (логин, пароль или токен)
3. Прокси сервер  - проверять включен или нет

# ЛК_2 22.01.24
1. Если есть папка `.git`, то команду `git init` НЕ нужно
2. Команда `config` настраиваются на ПК 1 раз
3. `git remote` указывается один раз   
![image](https://github.com/Katya6589/Semestr_6/assets/113089569/2ef7f763-4c05-445c-a094-8678678a2f2a)  
![image](https://github.com/Katya6589/Semestr_6/assets/113089569/1d429a55-ea93-4bcf-8d37-f1146371af24)  

# Задание 1. Знакомство с компилятором gcc
![image](https://github.com/Katya6589/Semestr_6/assets/113089569/05e5ab08-747a-46bc-9c82-d7f92242f787)
![image](https://github.com/Katya6589/Semestr_6/assets/113089569/25567386-eb6c-4610-a1d9-533970057ad0)
Debian:
`логин: stud`   
`пароль: qwerty`  
`RedOS: 12345678 `  
![image](https://github.com/Katya6589/Semestr_6/assets/113089569/5bb57255-2ff5-48ba-ace1-b26a5ba24667)

# ЛК_3 05.02.24 Работа с файлами
1. Создание
2. Перенесение
3. Редактирование
4. Удаление

**Обычный или regular файл**
--

1)`touch kstr.txt`   
2)`nano kstr.txt/home/stud/'Рабочий стол'`    
3)`mv kstr.txt/home/stud/'Рабочий стол'`    
4)`rm /home/stud/'Рабочий стол'/kstr.txt`     
5)`cat /home/stud/'Рабочий стол'/kstr.txt`     

`mv` - перемешение  
`rm` - удалить(каталог можно удалить только с `-r`, тк там внутри файлы)   
`ls` - просмотреть    
`-r` - рекурсия    
`cat` - чтение   
`mkdir` - создает директорию       
![image](https://github.com/Katya6589/Semestr_6/assets/113089569/c21fd701-a775-4daf-8b13-0da3561e92c5)  

**Папка (directory)**
--
1)`mkdir /home/stud/ kss`   
2)`mkdir /home/stud/kss home/stud/ksss`    
3)`touch home/stud/ksss/mayy`    
4)`touch home/stud/ksss`    
5)`rm -r home/stud/ksss`    
![image](https://github.com/Katya6589/Semestr_6/assets/113089569/60778296-0b41-47a7-b999-a269b02fc7dc)

## Устройства
### 1. Символьные (мышь, клавиатура и т.д.)
![image](https://github.com/Katya6589/Semestr_6/assets/113089569/9c8f87c9-6927-4c6e-9fca-95ca9c37f569)
![image](https://github.com/Katya6589/Semestr_6/assets/113089569/50741f5c-331f-4ad5-a269-59bdbf0ea972)  
`c` - cимвольные
### 2. Блочные (флешки)
![image](https://github.com/Katya6589/Semestr_6/assets/113089569/9b26fe19-4fbc-47d1-a259-28dcd489b7c9)
![image](https://github.com/Katya6589/Semestr_6/assets/113089569/9d493268-ccdf-481d-89a7-681e298bcf97)
![image](https://github.com/Katya6589/Semestr_6/assets/113089569/8bb85531-1449-4cdb-8885-a36853b5a841)
Пытались создать флешку
`b ` - блок

### Жесткая ссылка   
Создание - `ln mamka.txt dochka.txt`
`mamka.txt` - уже существующий файл в папке
`dochka.txt` - новый 
![image](https://github.com/Katya6589/Semestr_6/assets/113089569/fdb99092-b082-40e7-8351-0fb4e976ff61)     
Файлам присваиваются уникальные номера `inod`, посмотреть с комндой `ls -li1`    
![image](https://github.com/Katya6589/Semestr_6/assets/113089569/e6032559-d9e5-4e3c-8cd3-4e9be75b0bfe)    
 
Жесткие ссфлки имеют такой же номер как и сходный файл, и это можно импользовать, чтобы найти все жесткие ссылки    
![image](https://github.com/Katya6589/Semestr_6/assets/113089569/a50bd299-e1a3-40a2-8ded-fd67179569cd)       


