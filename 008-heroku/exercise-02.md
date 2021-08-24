# Задание 2.  Создание и загрузка приложения на хостинг.  

## Описание

Давайте создадим и загрузим простое приложение на хостинг, сделав его общедоступным.   

В виде решения этого задания присылайте ссылку на репозиторий с кодом в github 
(или другом хранилище репозиториев) и url на вашу работу. 

## Техническое задание
1. Проделайте все шаги по установке композера и клиента хероку. 
1. Заведите публичный репозиторий на гитхабе для этой работу.
1. Скачайте шаблон приложения https://github.com/netology-code/php-heroku-template-simple/archive/master.zip 
1. Создайте файл `index.php` который будет через `include` подключать и отображать html-код содержащий
    * информацию о вас, как об авторе, 
    * форму отправляющую данные в `post.php` с текстовым полем подразумевающим ввод имени пользователя. 
1. Рядом создайте php-файл `post.php` файл, который будет принимать данные формы, 
   сохранять имя пользователя в сессию и перенаправлять браузер обратно на `index.php`.
1. Теперь вернитесь в `index.php` и добавьте проверку, если внутри сессии существует
  не пустая переменная с именем пользователя, то просто поприветствуйте пользователя, 
  не отображая форму и разместите ссылку на скрипт `exit.php`. 
  Иначе отобразите форму как было раньше.
1. В скрипте `exit.php` очищайте переменную сессию, содержащую имя пользователя 
   и перенаправлять браузер обратно на `index.php`.
1. Загрузите работу на хостинг. 

В результате должен получиться простой сайт, запоминающий имя пользователя (почти как авторизация, 
осталось только еще и пароль проверить) и позволяющий "выйти", завершив сессию и забыв имя пользователя. 
