___Linux terminal (GitBash) commands___ 

___Homework 1___

___Elena Kot___ 


1) Посмотреть где я: 
   
   __pwd__

    __/d/2024/GIT/Music__
1) Создать папку:  
__mkdir Music__                                   
1) Зайти в папку: 
__cd Music__
1) Создать 3 папки: 
__mkdir Russian European American__
1) Зайти в любую папку:  
__cd European__
1) Создать файлы формата txt и json:    
__touch Rihanna.txt Meine.txt Mercury.txt McCartney.txt Taylor.json Mulyavin.json__  
1) Создать 3 папки:  
__mkdir Queen Beatles Scorpions__
//__mkdir {1..3}__ как альтернативный вариант.
1) Вывести список содержимого папки:  
__ls -la__
1) Открыть любой txt файл: 
__vim Mercury.txt__ 
1)  написать туда что-нибудь:
нажать кнопку __insert__ и ввести следующее предложение
 __Freddie Mercury was the leader of the musical group Queen.__ 
 
1)  сохранить и выйти: 
нажать кнопку __escape__, внизу окошка написать __:wq__  нажать __enter__ 
либо нажать кнопку __escape__,а затем нажать кнопку __shift__, удерживать ее и дважды нажать кнопку __z__
1)  Выйти из папки на уровень выше:  
__cd ..__
// выйти из папки на два уровня выше __cd ../..__
// выйти из папки на три уровня выше __cd ../../..__ и так далее.
1)  переместить любые 2 файла, которые вы создали, в любую другую папку в рамках одной директории:  
__mv Meine.txt Scorpions__

      __mv Mercury.txt Taylor.json Queen__

     __mv McCartney.txt Beatles__  
// если перемещать файлы за пределы текущей директории, то этот способ не работает, нужно указывать весь путь перемещения:
__mv /D/2024/GIT/Music/European/Mulyavin.json /D/2024/GIT/Music/Russian__

     __mv /D/2024/GIT/Music/European/Rihanna.txt /D/2024/GIT/Music/American__
1)  скопировать любые 2 файла, которые вы создали, в любую другую папку 
__cp Mercury.txt Taylor.json /D/2024/GIT/Music__
1)  Найти файл по имени:  
__$ find . -name Mercury.txt__
__./Music/European/Queen/Mercury.txt__
__./Music/Mercury.txt__

1)  просмотреть содержимое в реальном времени: 
__tail -f Mercury.txt__ 
__Freddie Mercury was the leader of the musical group Queen.__
1)  вывести несколько __первых__ строк из текстового файла  
__head -n3 Taylor.json__ где n это нужное количество строк
__123
456
789
10 11 12
13 14 15__
      
1)  вывести несколько __последних__ строк из текстового файла   
__tail -n5 Taylor.json__
__19 20 21
22 23 24
25 26 27
28 29 30
31 32 33__

      //17 и 18 может быть и без буквы n
__tail -6 Taylor.json__
__16 17 18
19 20 21
22 23 24
25 26 27
28 29 30
31 32 33__
1)  просмотреть содержимое __длинного__ файла 
__less Taylor.json__
__123
456
789
10 11 12
13 14 15
16 17 18
19 20 21
22 23 24
25 26 27
28 29 30
31 32 33
Taylor.json (END)__
//для выхода из утилиты и возвращения к командной строке терминала нажать q, ZZ
1)  вывести дату и время 
__date__
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


