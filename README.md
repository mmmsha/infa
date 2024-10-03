## 1 задание
Я установила дистрибутив linux ubuntu на виртуальную машину, после чего зашла в терминал и создала новый файл с именем script.bash, написав в терминале touch script.bash

Затем я открыла файл script.bash, выполнив в терминале gedit script.bash
![image](https://github.com/user-attachments/assets/43ab98f4-8099-4094-91a7-4bae3502c791)

В файл я вписала скрипт
#!/bin/bash
echo “Welcome to ITMO University”
![image](https://github.com/user-attachments/assets/e2281a16-03bd-4b21-bad6-70a1f8de6812)

Затем я сохранила файл, закрыла текстовый редактор gedit
Я выполнила в терминале bash script.bash, тем самым запустив bash-скрипт. В терминале отобразилось “Welcome to ITMO University”
 ![image](https://github.com/user-attachments/assets/4b05c5a7-c9b6-4670-9d79-7b69952d4658)

## 2 задание
Затем я модифицировала файл script.bash так, чтобы он выводил приветствие с любым введенным именем в терминале в виде
“Welcome, Vasya Pupkin”
Для этого я сначала написала в файле следующее:
#!/bin/bash
read name
echo “Welcome, $name”

![image](https://github.com/user-attachments/assets/92e55696-dd31-4ecd-9c9b-4601a5ecb018)

Однако при вводе данных функция read читает следующую строку, поэтому ввод в терминале выглядел как
bash script.bash
Vasya Pupkin

![image](https://github.com/user-attachments/assets/8e4197cb-cafe-4d10-8a2c-60535e45fd34)

Поэтому я поменяла содержимое файла на другую функцию, которая считывает информацию с той же строки:
#!/bin/bash
echo “Welcome, $*”

![image](https://github.com/user-attachments/assets/cadd868e-7bdb-4c14-9b39-3455d35f647e)

В итоге терминал стал воспринимать информацию об имени для приветствия в одной строке вместе с командой bash 

![image](https://github.com/user-attachments/assets/513c7ef1-971b-4f60-84f2-c341b5619923)



