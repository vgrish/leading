Регистрация пакета на Bower
===========================

```
bower register khusamov-sencha-extjs git://github.com/khusamov/sencha-extjs.git
```

Особенность команды, в отличии от регистрации например npm-пакета, заключается в том, что ее можно запускать где угодно. 
Главное чтобы был под рукой сам bower. А вот сам пакет не нужен.

Команда скачает пакет из репозитория и затем зарегистрирует. То есть, по-сути можно любой чужой репозиторий зарегистрировать.

Поэтому регистрировать пакет нужно на локальном компьютере. В Cloud9 не получится, просто не хватит дискового пространства 

## Обновление пакета

Специально обновлять зарегистрированный пакет не нужно. Достаточно создать метку с новой версией пакета в зарегистрированном репозитории, и эта новая версия сразу же будет доступна. Перед созданием метки обязательно обновить файл bower.json (как минимум указать новый номер версии). Для проверки можно использовать команду `bower info my-package-name`.
(будет скачан пакет, потом он будет распакован, потом ...).

Более подробно:
[www.codehint.ru](http://www.codehint.ru/articles/2015-04-26_create-and-update-bower-packages)
