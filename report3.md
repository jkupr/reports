# Куприянова Юлия, 241-353 

### Задание "Странный файл"  
1. Проверяю файл в hex-редакторе, так как файл слишком много весит. Меняю расширение на .rar 
<img src="image/19.png" alt=".rar" width="500"/>
2. Открываю архив, вижу еще файл, тоже проверяю его в hex-реадкторе, меняю расширение на .zip
<img src="image/20.png" alt=".zip" width="500"/>
4. Нахожу в одном из архивов код, написанный на python
<img src="image/21.png" alt="python" width="500"/>
<img src="image/22.png" alt="code" width="500"/>
5. Меняю код и вывожу флаг в расшифрованном виде
<img src="image/23.png" alt="flag1" width="500"/>
```
Ответ: mospoly{x0r_4nd_b4s364_jUFSY7fd}
```

### Задание "Admin panel" 
1. Перехожу по данному в задании IP и ввожу рандомные данные для регистрации 
<img src="image/24.png" alt="registration" width="500"/>
2. После регистрации перехожу в Admin panel, вижу флаг, но он неверный 
<img src="image/25.png" alt="Admin panel" width="500"/>
3. В HTTP history в запросе есть JWT-токен авторизации 
<img src="image/26.png" alt="token" width="500"/>
4. Отправляю запрос в Repeater, меняю роль и имя на admin, алгоритм на none и удаляю подпись в самом JWT 
<img src="image/27.png" alt="repeater" width="500"/>
<img src="image/28.png" alt="repeater2" width="500"/>
5. Отправляю запрос и получаю флаг 
<img src="image/29.png" alt="flag" width="500"/>
```
Ответ: CODEBY{I'M_G0NN4_H4V3_70_F1R3_7H3_C0D3R}
```

### Задание "PDF-библиотека" 
1. В файле в заголовке присутствует шестнадцатеричный код 
<img src="image/30.png" alt="url" width="500"/> 
2. Если вместо имеющегося кода подставить index.php в 16-ричном формате, то файл не будет прогружаться 
<img src="image/31.png" alt="index.php" width="500"/> 
3. Открываю pdf-файл с измененной ссылкой, в нем есть две закомментированные строки 
<img src="image/32.png" alt="file" width="500"/> 
4. Название файла с флагом перевожу в 16-ричный код, добавив две точки и слеш, чтобы оказаться на директорию выше, и открывваю файл
<img src="image/33.png" alt="hex" width="500"/> 
<img src="image/34.png" alt="flag" width="500"/>
```
Ответ: CODEBY{h3x3d_lf1_beaut1fulll}
```
### Задание Binary Reverse 
1. Извлекаю читаемые строчки из файла
<img src="image/35.png" alt="bin" width="500"/>
2. В функциях бинарного файла ищу те, которые в названи содержат get_key 
<img src="image/36.png" alt="flag" width="500"/>
3. Вывожу ассемблерный код только по адресам о 0x1220 до 0x1250 
<img src="image/37.png" alt="flag" width="500"/>
4. Извлекаю данные из секции .rodata и сохраню в файл enc.hex 
<img src="image/38.png" alt="flag" width="500"/>
5. С помощью кода нахожу флаг 
<img src="image/39.png" alt="flag" width="500"/>
```
Ответ: FLAG{bin_user_2_A13f8f02} 
```
