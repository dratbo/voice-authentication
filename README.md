<h1 align="center"> Привет!<a target="_blank">
<img src="https://github.com/blackcater/blackcater/raw/main/images/Hi.gif" height="32"/></h1>

<h2 align="center"> Данная работа на тему: "Веб-приложение для биометрической аутентификации по голосу" является ВКР бакалавриата. Выкладываю чтобы просто было!

<h2 align="center"> Технический стек работы смотрите в прикрепленном вордовском файле --> "voice_auth_tech_description_17384546.docx"


<h3 align="center"> Ниже приведенна инструкция работы программы и её установки <h3>

<h3>1. Скачивание файлов</h3>

Находим в репозитории папку "Ссылка на яндекс диск с работой", находим ссылку на яндекс диск и скачиваем .rar файлик.


Скачали, открыаем, видим там два файла, "vebAUUU" и "ffmpeg". Главное не скачивать эти файлы с путем overdrive, иначе при работе программа будет выдавать ошибку.

В моём случае оба эти файлы находились в разных папках на диске C (C:\ffmpeg) (C:\vebAUUU)


<h3>2. Распоковка работы. Скачивание библиотек </h3>


Я использовал рабочую среду PyCharm.
Сакчиваем библиотеки из файлика --> "requirements.txt"

Открываем проект в рабочей среде.

После успешного скачивания всех библиотек прописываем:

1. python manage.py makemigrations
2. python manage.py migrate 
3. python manage.py runserver  

Обязательно смотрите путь, где вы прописываете команды, вы должны быть в проекте!!!!!

Вот пример, того, что выводят команды 


<img width="1539" height="698" alt="image" src="https://github.com/user-attachments/assets/f1328787-06a1-45ff-8195-9a8a34f26e95" />


После этого переходим по ссылке http://127.0.0.1:8000/



<img width="814" height="97" alt="image" src="https://github.com/user-attachments/assets/c80e57c9-4755-4add-ab6a-51439ac6d4e3" />



Попадаем на приветсвенную страницу


<img width="1909" height="967" alt="image" src="https://github.com/user-attachments/assets/ea45f45d-7d3a-4b21-842d-011df7e5d6df" />


Переходим по --> "Регистрация"


<img width="1909" height="958" alt="image" src="https://github.com/user-attachments/assets/f258c47c-9cc7-463b-9ff5-8f6c162ad15f" />


Вводим свое или тестовое имя, после чего нажимаем --> "Записать голос"


<img width="1913" height="974" alt="image" src="https://github.com/user-attachments/assets/3fcf97e5-a7f7-4c0b-be95-7a391d5ec481" />


Всё записали, прослушали на всякий, нужен качественно записанный голос:) Жмём --> "Зарегистрироваться"


Попадаем на страницу авторизации, нажимаем --> "записать голос"


<img width="1912" height="964" alt="image" src="https://github.com/user-attachments/assets/3224176d-2bfe-47e9-8f1c-b2248d170de3" />


Записали голос, жмем кнопочку --> "Войти"


<img width="1912" height="948" alt="image" src="https://github.com/user-attachments/assets/26a18903-3ad7-4056-bf68-db68959a463a" />


При успешной проверке на голос вас пустит в систему, если нет, выдаст ошибку


<img width="1918" height="965" alt="image" src="https://github.com/user-attachments/assets/5eeb2670-1dc8-4a62-a624-34740aaca098" />


При неудачной попытке вы увидете уведомление "Голос не распознан. Похожесть: 0.73" 
Данное значение можно регулировать в коде. В моём случае, если значение меньше 0.75, то меня не пропустит. 


<img width="1157" height="595" alt="image" src="https://github.com/user-attachments/assets/2c5f2536-c8de-42ca-9c80-5af5026b21d1" />


Данное значение можно спокойно менять под свои нужды.
Также данная работу не подразумевает "кодового слова", тоесть просто пытается определить по голосу, но значение "похожести" будет лучше, если говорить то, что сказали при регистрации.


