# srm

### Всем привет!
В данном репозитории размещен скрипт, позволяющий удалять файлы или директории. При использовании скрипта вы можете быть уверены в том, что случайно удаленный файл можно будет восcтановить в течение **7 дней**. Данный скрипт применим для ОС Ubuntu. 

# Что такое Ubuntu?
Ubuntu — дистрибутив Linux, основанный на Debian GNU/Linux. В основном взаимодействие человека системой при помощи *terminal*. 

# Как скачать себе это скрипт? 
Для того, что бы скачать скрипт тебе необходимо его клонироать на свою рабочую машину командой **git clone** 
    - `git clone https://github.com/rinAkhm/second_week.git`
Далее тебе будет предложено ввести логин и пароль своей учетной записи.

# Предисловие
Для удобства использования скрипта рекомендуется проделать ряд манипуляций. 
   - создать в домашней директории папку **bin/**
   `mkdir bin/`
   - Создать файл `.bash_profle` и добавь в него строку `export PATH="${PATH}:~/bin"`
   `echo export 'PATH="${PATH}:~/bin"' >> ~/.bash_profile && source ~/.bash_profile` 
   -  Перемести или скопируй скрипт srm из папки second_week в папку `bin/`
   
Ура! Теперь ты можешь запускать свой скрипт из любой директории введя только его название. 

# Как начать пользоваться скриптом или просто его запустить? 
Для начала тебе нужен файл или папка, которую ты хочешь удалить. После того, как ты нашел, что будешь удалять тебе нужно вместо **namefile** или **namefolder** написать твой любой файл или папку:
   - `srm namefile/namefolder`

# Как все это работает? 
При первом запуске скрипта у тебя в домашней диретории создается папка под названием **RECYCLE**. Все то, что ты пытаешься удалить перемещается в данную папку с расширем **.gz** и храниться там **7 дней**. При каждом запуске скрипта просходить архирование файла, а также удаление содержимого, если оно было неактивно больше **7 дней**. 



