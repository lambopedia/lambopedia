---
title: 'Как заводить пользователей'
media_order: 'Screenshot_6.jpg,Screenshot_7.jpg'
---

## Создание через админку
Создание пользователей происходит через левую панель админки:
![](Screenshot_6.jpg)

Далее в верхнем правом углу необходимо нажать на кнопку "Добавить". Откроется форма добавления пользователя. В ней необходимо задать логин. Логин в последствии не меняется. При необходимости изменить логин нужно заводить нового пользователя.
![](Screenshot_7.jpg)

Далее откроется форма настроек пользователя, в которой необходимо задать параметры пользоватлеля:
+ email
+ начальный пароль 
+ полное имя
+ заголовок - это роль пользователя на сайте
+ язык (по умолчанию)

"2-Factor Authentication" - это двухфакторная авторизация. Она не доступна и включать её не нужно, она не будет работать.

Далее необходимо определить уровни доступа. Для редактирования статей достаточно прав:
+ site.login
+ admin.pages
