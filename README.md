___Linux terminal (GitBash) commands___ 

___Homework 1___

___Elena Kot___ 


1) Посмотреть где я: 
   
   __pwd__

    >__/d/2024/GIT/Music__
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
>__mv Meine.txt Scorpions__ __mv Mercury.txt Taylor.json Queen__ __mv McCartney.txt Beatles__  
// если перемещать файлы за пределы текущей директории, то этот способ не работает, нужно указывать весь путь перемещения:
>__mv /D/2024/GIT/Music/European/Mulyavin.json /D/2024/GIT/Music/Russian__ __mv /D/2024/GIT/Music/European/Rihanna.txt /D/2024/GIT/Music/American__
14)  скопировать любые 2 файла, которые вы создали, в любую другую папку 
>__cp Mercury.txt Taylor.json /D/2024/GIT/Music__
15)  Найти файл по имени:  
__$ find . -name Mercury.txt__
>__./Music/European/Queen/Mercury.txt__
>__./Music/Mercury.txt__

16)  просмотреть содержимое в реальном времени: 
__tail -f Mercury.txt__ 
>__Freddie Mercury was the leader of the musical group Queen.__
17)  вывести несколько __первых__ строк из текстового файла  
__head -n3 Taylor.json__ где n это нужное количество строк
>__123
456
789
10 11 12
13 14 15__
      
18)  вывести несколько __последних__ строк из текстового файла   
__tail -n5 Taylor.json__
>__19 20 21
22 23 24
25 26 27
28 29 30
31 32 33__

      //17 и 18 может быть и без буквы n
__tail -6 Taylor.json__
>__16 17 18
19 20 21
22 23 24
25 26 27
28 29 30
31 32 33__
19)  просмотреть содержимое __длинного__ файла 
__less Taylor.json__
>__123
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
20)  вывести дату и время 
>__date__
--------------------------------------------------------------------------------------
Отправить http запрос на сервер:
    http://162.55.220.72:5005/terminal-hw-request :

curl "http://162.55.220.72:5005/get_method?name=kotlena&age=40"
["kotlena","40"]


Написать скрипт:
>#!/bin/bash
mkdir Music
cd Music
mkdir Russian European American
cd European
touch  Meine.txt Mercury.txt McCartney.txt Taylor.json 
mkdir Queen Beatles Scorpions
ls -la
mv Meine.txt Scorpions
mv Mercury.txt Taylor.json Queen
mv McCartney.txt Beatles
ls -la
./firstscript.txt

>user@HOME-PC MINGW64 /d/2024/GIT/Music/Music/European/Music/European/Music/European (main)
$ ls -la
total 4
drwxr-xr-x 1 user 197121 0 Feb  4 22:54 ./
drwxr-xr-x 1 user 197121 0 Feb  4 22:54 ../
drwxr-xr-x 1 user 197121 0 Feb  4 22:54 Beatles/
drwxr-xr-x 1 user 197121 0 Feb  4 22:54 Queen/
drwxr-xr-x 1 user 197121 0 Feb  4 22:54 Scorpions/



