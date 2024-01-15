# ЛК_1 15.01.24
[Установка git bash](https://git-scm.com/downloads)
---
[Практические задания по гит](https://smartiqa.ru/courses/git/answer-key)
---

**git bash** - это команды для работы с гит из терминала  

**Прокси сервер** git config --global http.proxy 10.0.50.52:3128

![image](https://github.com/Katya6589/Semestr_6/assets/113089569/c0294fda-6f7f-4037-8034-da1bb7b16124)

Создаие репозитория на компьтере:
--
- инициализация git init
![image](https://github.com/Katya6589/Semestr_6/assets/113089569/ec7edef9-c3e8-4f7f-9d86-b798ea09cd96)

**$ cmd //c tree .git** - показывает структуру папки гит
  ![image](https://github.com/Katya6589/Semestr_6/assets/113089569/608a3012-6924-4146-af07-e0ce620481cb)

---
$ git status - (показывает статус репозитория)  
On branch master - (указывает имя ветки)  

No commits yet - (нет созраненных версий)  

Untracked files: - (не отслеживымаемые файлы)  
  (use "git add <file>..." to include in what will be committed) - (нужна комнда "добавить", чтобы зафиксировать версию для сохранения)  
  Список файлов для добавления (внизу 2 строки):   
          index.html  
          pictures/  

nothing added to commit but untracked files present (use "git add" to track) - (найдены файлы для добавления)  

![image](https://github.com/Katya6589/Semestr_6/assets/113089569/e9721c78-4316-4316-9d7f-e8fbddb1b505)

---


Настраиваем пользователя Git
--
Задаем имя и email пользователя для текущего репозитория 23-12 303-15  
$ git config --global user.name PK303-13  
$ git config --global user.email PK303-13@gmail.com  

Отменяет прокси сервер:  
git config --global –unset http.proxy  
git config --global --unset https.proxy  
git config --global --unset core.gitproxy  

Добавление файла ( * - все файлы):  
$ git add *
![image](https://github.com/Katya6589/Semestr_6/assets/113089569/598d2c69-8f14-4ef0-ae22-702c72f8c942)

Для фиксации версии нужно указать ее название, для этого созддается сообщение (-m)    
git commit -m "G-02: Initial"    

Выводим информмацию о фиксации:  
$ git log  
![image](https://github.com/Katya6589/Semestr_6/assets/113089569/0970f675-d68b-43bc-ab9a-2fa8a9e06c4f)
