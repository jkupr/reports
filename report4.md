# Куприянова Юлия, 241-353  
## PortSwigger
### Задание 1. 
Ссылка задания ведет на блог, у которого под постами можно оставлять комментарии\
<img src="image/45.png" alt="drawing" width="400"/>\
Можно провести DOM Clobbering атаку, перезаписав переменную defaultAvatar и выполнив XSS через onerror\
<img src="image/46.png" alt="drawing" width="400"/>\
Оставляю второй комментарий, чтобы страница перезагрузилась и код выполнился\
<img src="image/47.png" alt="drawing" width="400"/>\
<img src="image/48.png" alt="drawing" width="400"/>\
<img src="image/49.png" alt="drawing" width="400"/>\

### Задание 2. 
Вхожу в аккаунт и меняю почту, перехватывая запрос в Burp\
<img src="image/50.png" alt="drawing" width="400"/>\
<img src="image/51.png" alt="drawing" width="400"/>\
Дальше сделать не получилось, тк нужна про версия Burp\
<img src="image/52.png" alt="drawing" width="400"/>\

### Задание 3.
В строку поиска добавляю скрипт и перехватываю запрос в Burp\
<img src="image/53.png" alt="drawing" width="400"/>\
Полезная нагрузка отражается, но CSP препятствует выполнению скрипта\
<img src="image/55png" alt="drawing" width="400"/>\
Меняю токен, чтобы разрешить скрипт\
<img src="image/56.png" alt="drawing" width="400"/>\
<img src="image/57.png" alt="drawing" width="400"/>\
<img src="image/58.png" alt="drawing" width="400"/>\

## DVWA
### Задание 1 - XSS (Reflected).
Создаю полезную нагрузку и ввожу ее в поле name, отправляя форму. Браузер жертвы подключился к BeEF
<img src="image/62.png" alt="drawing" width="400"/>\

### Задание 2 - XSS (DOM).
В параметр default добавляю скрипт\
<img src="image/63.png" alt="drawing" width="400"/>\
После перезагрузки страницы отобразилось всплывающее окно с подтверждение уязвимости\
<img src="image/64.png" alt="drawing" width="400"/>\

### Задание 3 - XSS (Stored).
В поле Message ввожу полезную нагрузку, отправляю форму. Отображается уведомление, подтверждая наличие уязвмости\
<img src="image/65.png" alt="drawing" width="400"/>\

### Задание.
Перехожу по ссылке, внизу страницы есть поле для ввода комментариев\
<img src="image/69.png" alt="drawing" width="400"/>\
Ввожу комментарий с формой ввода информации, чтобы пользователя перевело на страниу с флагом\
<img src="image/67.png" alt="drawing" width="400"/>\
<img src="image/68.png" alt="drawing" width="400"/>\

