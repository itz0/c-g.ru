# Программы обработчики для сайта c-g.ru

<br>

## Состав программ: 
- **[c-g-isbn](https://github.com/itz0/c-g.ru/tree/main/c-g-isbn)** - эта программа позволяет быстро получить информацию о доступных книгах на сайте c-g.ru, путем запроса через поиск сайта списка isbn кодов или book id (ids) кодов 
- **[c-g-text](https://github.com/itz0/c-g.ru/tree/main/c-g-isbn)** - эта программа позволяет быстро получить информацию о доступных книгах на сайте c-g.ru, путем запроса через поиск сайта списка текстового названия книг, для дальнейшей обработки полученных book id (ids) кодов в программе **c-g-isbn**
- **[c-g-images](https://github.com/itz0/c-g.ru/tree/main/c-g-images)** - эта программа позволяет загружать изображения по доступным книгам на сайте c-g.ru, использует в своей работе информацию полученную в результате работы другой программы **c-g-isbn**

<br>

## Для кого эти программы?
для фрилансеров и всех кто работает с большим объемом книг и конкретно с сайтом c-g.ru

<br>

## Системные требования и ограничения программ
программы гарантированно работают на ОС Windows 10 x64, Windows 8.1 32-bit (только 32-битный билд), интернет желательно быстрый, проводной..

<br>

## По поводу вирусов, троянов и закрытого кода
данные программы гарантированно ***мною*** не содержит в себе вирусов, троянов и прочего малваря, кто сомневается можете запускать из песочницы, виртуальных машин, программы написаны на чистом питоне и скомпилированы на gcc последних версий, по известным причинам я не публикую исходный код программ также как не использую реальное название сайта в данном проекте и его описании..

<br>

## Состав дистрибутивов программ
в дистрибутив программы входят исполняемые файлы и необходимые для работы программы библиотеки, всегда читайте внимательно описание к [релизу](https://github.com/itz0/c-g.ru/releases/) и скачивайте правильную версию под Вашу ОС

<br>

## О разделе [Wiki](https://github.com/itz0/c-g.ru/wiki/%D0%9E-%D0%BF%D1%80%D0%BE%D0%B3%D1%80%D0%B0%D0%BC%D0%BC%D0%B5) 
в этом разделе не всегда выложенна актуальная информация по использованию программ, **актуальное видео по работе с конкретной программой, всегда присутствует в архиве под названием c-g-readme*.zip, вместе с конкретным релизом.**

<br>

## Возможные ошибки - большинство ошибок при запуске и работе программы связанны c данными важными моментами:

<br>

## 1. Не закрытые или не правильно заполненные XLSX, CSV файлы
формат заполненния файлов прост, как правило это два первых столбца, оба из которых должны быть заполненны правильно, также в файлах не допускается пустых строк между данными.

<br>

## 2. Не подходящие headers
- **сайт c-g.ru использует защиту Incapsula пока для её обхода требуется выполнить несколько условий:**
- иметь белый, пушистый русский ip адрес, проверьте, откройте веб броузер перейдите на сайт c-g.ru если у Вас выскакивает капча при входе на сайт c-g.ru, то у Вас не подходящий ip адрес.. возможное решение - используйте vpn или прокси..
- скопировать свежие headers из Вашего веб броузера и вставить их в файл headers.txt в каталоге с программой, как это сделать рассказываю в этом **[видео](https://streamable.com/evo4rh)**

<br>

## 3. Не обрабатывайте более 500 isbn кодов за раз, меньше - лучше и быстрее)
если возникает ошибка попробуйте разбить свой список isbn кодов на несколько и таким образом обработать большую часть isbn кодов и возможно найти на каком конкретном isbn коде программа падает

<br>

## _обо всех остальных ошибках в работе программ прошу Вас сообщать мне_
если программа крэшится попробуйте запустить ее внутри следующего c-g.bat файла, сделайте скриншот и пришлите мне этот скриншот вместе со списком ваших isbn кодов, к примеру
```
с-g-isbn.exe
pause
```










