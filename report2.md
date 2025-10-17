# Куприянова Юлия, 241-353 

### Задание 1. 
1. Нахожу ip-адрес Metasploitable3 с помощью команды: 
```
nmap -sn 192.168.0.0/24
```
<img src="image/6.png" alt="nmap" width="400"/>\
2. Перехожу на сайт DVWA\ 
<img src="image/7.png" alt="DVWA" width="400"/>\
3. C помощью dirbuster провожу сканирование директории vulnerabilities\ 
<img src="image/8.png" alt="\vulnerabilities\" width="400"/>\
Ответ: 4 директории\ 

### Задание 2.
1. Устанавливаю уровень безопасности DVWA Low\
<img src="image/9.png" alt="Low" width="400"/>\
2. Настраиваю Proxy в браузере для Burp Suite\
<img src="image/10.png" alt="Proxy" width="400"/>\
3. Вписываю рандомные логин, пароль и перехватываю GET запрос с ними\
<img src="image/11.png" alt="GET" width="400"/>\
4. В Intruder в режиме Cluster bomb провожу атаку, используя прикрепленный словарь, и нахожу нужную комбинацию\
<img src="image/12.png" alt="Attack" width="400"/>\
Ответ: логин: admin, пароль: password\

### Задание 3.
1. Перейдя по ссылке, ввожу рандомные логин и пароль\
<img src="image/13.png" alt="Low" width="400"/>\
2. Перехватываю запрос с помощью Burp Suite и перенаправляю его в Intruder. Сканирую все логиы, прикрепленные в задании и нахожу верный - auction\
<img src="image/14.png" alt="Low" width="400"/>\
<img src="image/15.png" alt="Low" width="400"/>\
4. Затем меняю логин в запросе на "auction" и далее сканирую все пароли. Верный - michelle\
<img src="image/16.png" alt="Low" width="400"/>\
<img src="image/17.png" alt="Low" width="400"/>\

### Задание 4.
С помощью декодера определяю, что фраза закодирована в Base64. Декодировав ее, получаю: U vas poluchiloc\
<img src="image/18.png" alt="Low" width="400"/>\
