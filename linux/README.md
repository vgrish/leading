Основные команды Unix
=======================

Архивирование
--------------------------- 
tar -czf <архив> <что-архивировать>

Для Петерхоста:

заходим в каталог www

tar -czf ../backup-file ./site<N>

 

Архивировать в ZIP (ключ -r для того, чтобы архивировать со всеми поддиректориями)

zip -r archiv.zip files

Распаковка архива zip-формата
--------------------------- 
unzip
 
Удаление файла
--------------------------- 
rm <файл>
 
Удаление каталога
--------------------------- 
rm -r <каталог>
 
Копирование файла
--------------------------- 
cp <откуда> <куда>
 
Копирование каталога
--------------------------- 
cp -r <откуда> <куда>
 
Создание символической ссылки
--------------------------- 
ln -s <на-что-ставим-ссылку> <имя-ссылки>  
ln -s /home/<login>/cgi-bin/parser3 parser3
 
Узнать дисковую квоту
--------------------------- 
quota
 
Тип процессора и версия операционной системы
--------------------------- 
uname -a

или 

cat /proc/cpuinfo

Платформа i386 является тридцати двух разрядной.
 
