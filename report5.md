# Куприянова Юлия, 241-353  
### Задание 
```
https://ctflearn.com/challenge/97
```
Переходя по ссылке, скачиваю изображение. Сразу проверяю его метаданные командой exiftools AGT.png\
<img src="image/73.png" alt="drawing" width="400"/>

Файл является JPEG, а не PNG, поэтому ищу скрытые файлы внутри изображения\
<img src="image/74.png" alt="drawing" width="400"/>

Скрыто множество файлов. Извлекаю их и перехожу в созданную папку\
<img src="image/75.png" alt="drawing" width="400"/>

Дальше просматриваю извлеченные файлы и перехожу в "Secret Stuff..." - "Don`t Open This...". В последней папке есть файл "I Warned You.jpeg".
<img src="image/76.png" alt="drawing" width="400"/>

Извлекаю строки этого файла, сразу же отфильтровывая по началу флага, и нахожу флаг\
<img src="image/77.png" alt="drawing" width="400"/>

<img src="image/78.png" alt="drawing" width="400"/>

```
ABCTF{Du$t1nS_D0jo}
```
