**1) Посмотреть где я ---** pwd  
**2) Создать папку ---** mkdir newfolder  
**3) Зайти в папку ---** cd newfolder  
**4) Создать 3 папки ---** mkdir NewFolder_{1..3}  
**5) Зайти в любоую папку ---** cd NewFolder_1  
**6) Создать 5 файлов (3 txt, 2 json) ---** touch {1..3}.txt {1..2}.json  
**7) Создать 3 папки ---**  mkdir Folder_{1..3}  
**8) Вывести список содержимого папки ---** ls -la  
**9) + Открыть любой txt файл ---** vim 1.txt  
**10) + написать туда что-нибудь, любой текст. ---** i, Hello World!  
**11) + сохранить и выйти. ---** Esc, :wq  
**12) Выйти из папки на уровень выше ---** cd ../  
**13) переместить любые 2 файла, которые вы создали, в любую другую папку. ---** mv NewFolder_1/1.txt NewFolder_1/2.txt NewFolder_2  
**14) скопировать любые 2 файла, которые вы создали, в любую другую папку. ---** cp NewFolder_1/1.json NewFolder_1/2.json NewFolder_2  
**15) Найти файл по имени ---** find -name 1.json  
**16) просмотреть содержимое в реальном времени (команда grep) изучите как она работает. ---** grep 'mv' script.sh  (script.sh создан в последнем задании со звёздочкой) tail -F script.sh | grep "name",
если нужна запись в другой txt -- tail -F 1.txt | grep --line-buffered qw | cat >> 2.txt  
**17) вывести несколько первых строк из текстового файла ---** head -3 script.sh  
**18) вывести несколько последних строк из текстового файла ---** tail -3 script.sh  
**19) просмотреть содержимое длинного файла (команда less) изучите как она работает. ---** less script.sh  
**20) вывести дату и время ---** date  
**Задание ***  
**1) Отправить http запрос на сервер.
http://162.55.220.72:5005/terminal-hw-request** --- curl http://162.55.220.72:5005/terminal-hw-request --- curl 'http://162.55.220.72:5005/get_method?name=(Sergey)&age=(34)'  
**2) Написать скрипт который выполнит автоматически пункты 3, 4, 5, 6, 7, 8, 13**  
touch script.sh
cat > script.sh
#!/bin/bash
cd c:
cd newfolder
mkdir NewFolder_{1..3}
cd NewFolder_1
touch {1..3}.txt {1..2}.json
mkdir Folder_{1..3}
ls -la
cd ../
mv NewFolder_1/1.txt NewFolder_1/2.txt NewFolder_2
Enter
Control+C

sh script.sh
