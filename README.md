# bayan


### bayan утилита для обнаружения файлов-дубликатов c бережным обращением с дисковым вводом выводом

#### Пример использования
```
./bayan -s ~/.. -e Qt -l1 -f1 -b100 -m t?g*.*

```
### Аргументы:

***
**-h, --help**
>Справка

**-s, --scan-dir**
>Директории для сканирования (может быть несколько), по умолчанию все

**-e, --excl-dir**
>Директории для исключения из сканирования (может быть несколько)

**-l, level-scan**
>Уровень сканирования (1 на все директории, 0 - только указанная
директория без вложенных), по умолчанию 0

**-f, --file-scan**
>Минимальный размер файла, по умолчанию проверяются все файлы
больше 1 байта.

**-m, --file-mask**
>Маски имен файлов разрешенных для сравнения (не зависят от
регистра), по умолчанию *

**-b, --block-size**
>Размер блока, которым производится чтения файлов, по умолчанию 10 байт

**-c, --hash**
>Один из имеющихся алгоритмов хэширования: crc32 или md5, по умолчанию crc32