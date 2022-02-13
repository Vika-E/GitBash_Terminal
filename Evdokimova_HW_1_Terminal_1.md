1) Посмотреть где я === pwd
2) Создать папку === mkdir new_folder
3) Зайти в папку === cd new_folder
4) Создать 3 папки === mkdir f_1 f_2 f_3
5) Зайти в любоую папку === cd f_1
6) Создать 5 файлов (3 txt, 2 json) === touch t_file1.txt t_file2.txt t_file3.txt j_file1.json j_file2.json
7) Создать 3 папки === mkdir ff_1 ff_2 ff_3
8. Вывести список содержимого папки === ls -la
9) + Открыть любой txt файл === vim t_file1.txt
10) + написать туда что-нибудь, любой текст. === i Hey guys!
11) + сохранить и выйти. === нажать esc, ввести :wq, нажать enter
12) Выйти из папки на уровень выше === cd .. 
—
13) переместить любые 2 файла, которые вы создали, в любую другую папку. === mv f_1/t_file1.txt f_1/t_file2.txt f_2
14) скопировать любые 2 файла, которые вы создали, в любую другую папку. === cp f_1/j_file1.json f_1/j_file2.json f_3
15) Найти файл по имени === find . -name "j_file.json" 
16) просмотреть содержимое в реальном времени (команда grep) изучите как она работает.===  tail -f t_file4.txt
17) вывести несколько первых строк из текстового файла === head t_file4.txt
18) вывести несколько последних строк из текстового файла === tail t_file4.txt
19) просмотреть содержимое длинного файла (команда less) изучите как она работает. ===  less t_file4.txt (или можно cat t_file4.txt)
20) вывести дату и время === date  
=========

__Задание *__

1) Отправить http запрос на сервер. 
http://162.55.220.72:5005/terminal-hw-request === 

    1.  curl http://162.55.220.72:5005/terminal-hw-request
    2.  curl  "http://162.55.220.72:5005/get_method?name=(Vika)&age=(35)"

2) Написать скрипт который выполнит автоматически пункты 3, 4, 5, 6, 7, 8, 13 ===

    ___1. Создание файла___  
touch my_script  
vim my_script  
i  

    ___2. Сам скрипт___  
#!/bin/bash  
cd new_folder  
mkdir f_4 f_5 f_6  
cd f_6  
touch t_file1.txt t_file2.txt t_file3.txt j_file1.json j_file2.json  
mkdir ff_1 ff_2 ff_3  
ls -la  
mv t_file1.txt t_file2.txt ../f_5  

    ___3. Запуск скрипта___  
chmod ugo+x my_script  
./my_script  

