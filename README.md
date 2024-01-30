___Linux terminal (GitBash) commands___ 
___Homework 1___
___Elena Kot___ 


1) Посмотреть где я: 
   __$ pwd__
__/d/2024/GIT/Music__
2) Создать папку:  
__mkdir Music__                                   
1) Зайти в папку: 
__cd Music__
1) Создать 3 папки 
__mkdir Russian European American__
1) Зайти в любую папку  
__cd European__
1) Создать 5 файлов (3 txt, 2 json)    
__touch Meine.txt Mercury.txt McCartney.txt Taylor.json Mulyavin.json__  
1) Создать 3 папки  
mkdir {1..3}
1) Вывести список содержимого папки  
ls -la
1) + Открыть любой txt файл 
vim 1.txt 
1)  + написать туда что-нибудь
insert (кнопка i) любой текст  
1)  + сохранить и выйти 
escape, внизу написать :wq  нажать enter или escape,shift+zz
1)  Выйти из папки на уровень выше  
cd ..
1)  переместить любые 2 файла, которые вы создали, в любую другую папку в рамках одной директории  
mv 1.txt 2.txt dir_1  
У меня с помощью точки слеш или две точки слеш не перемещает из одной директории в другую поэтому я пишу mv пробел весь 
путь откуда пробел весь путь куда включая имя перемещаемого файла    еще вариант нашла mv имяпапки/имяфайла пробел имя папки
1)  скопировать любые 2 файла, которые вы создали, в любую другую папку 
cp 1.txt 2.txt dir_1
1)  Найти файл по имени  
find . -name file1.txt     
1)  просмотреть содержимое в реальном времени 
tail -f file1.txt 
1)  вывести несколько первых строк из текстового файла  
head -n3 имяфайла         
1)  вывести несколько последних строк из текстового файла   
tail -n2 имя_файла
17 и 18 может быть и без буквы n
1)  просмотреть содержимое длинного файла 
less имяфайла
1)  вывести дату и время 
date
--------------------------------------------------------------------------------------
"http://162.55.220.72:5005/get_method?name=kotlena&age=38"
["kotlena","38"]


#!/bin/bash

mkdir scriptdir
cd scriptdir
mkdir script1dir script2dir script3dir
cd script1dir
touch file1.txt file2.txt file3.txt 1.json 2.json
mkdir dir1 dir2 dir3
ls -la
mv file1.txt file2.txt dir1 это внутри скрипта  user@HOME-PC MINGW64 /d/Linux/group_23
$ ./firstscript.txt
total 4
drwxr-xr-x 1 user 197121 0 Oct  4 18:43 .
drwxr-xr-x 1 user 197121 0 Oct  4 18:43 ..
-rw-r--r-- 1 user 197121 0 Oct  4 18:43 1.json
-rw-r--r-- 1 user 197121 0 Oct  4 18:43 2.json
drwxr-xr-x 1 user 197121 0 Oct  4 18:43 dir1
drwxr-xr-x 1 user 197121 0 Oct  4 18:43 dir2
drwxr-xr-x 1 user 197121 0 Oct  4 18:43 dir3
-rw-r--r-- 1 user 197121 0 Oct  4 18:43 file1.txt
-rw-r--r-- 1 user 197121 0 Oct  4 18:43 file2.txt
-rw-r--r-- 1 user 197121 0 Oct  4 18:43 file3.txt


