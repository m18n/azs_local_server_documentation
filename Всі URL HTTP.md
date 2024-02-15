---
Type: fact
tags: 
Data: 2024-02-10
---
Тут написані всі посилання back-end
## System
1. **/public/(path)** #get path це шлях до любого файлу в папці azs_site
2. **/settings/dberror** #get  це сторінка налаштування бази даних при відсутності підключення до неї. Видає файл **settings_db_error.html**. Це [[Сторінка База Даних]]
3. **/settings/dberror/send** #post  це сторінка для відправки даних на підключення якщо дані записались то відправляється у відповідь {"status": "yes"} якщо ні то {"status":"no"}
4. **/settings/dberror/check** #post - це сторінка для отримання інформації про підключення. На нього потрібно робити постійні запити при підключенні до бази щоб знати  статус. він повертає такі статуси {"status": "process"} {"status": "connect"} {"status": "disconnect"} по назвам я думаю все зрозуміло.
## Auth
1. **/** #get це шлях до авторизації файл **login.html**
2. **/auth** #post  це сторінка для підтвердження авторизації та отримання вдалості. якщо вхід вдалий то повертається в json {"status": "yes"} якщо ні то {"status":"no"}
## Main
1. **/main** #get - це головна сторінка де виводяться всі колонки видається файл **serv.html**
2. **/main/settings** #get - це сторінка сервіси видається файл **settings_azs.html**. Це [[Сторінка Сервіси]]
3. **/main/settings/configuration** #get - це сторінка з налаштуванням видів палива, резервуарів, колонки. повертає файл **configuration.html**. Це [[Сторінка Налаштування]]
## API
1. **/api/pump/save** #post - це сторінка для зберігання колонок
2. **/api/out** #get - це для очищення cookie тобто входу
3. **/api/outshift/** #get - закриття зміни
4. **/api/settings/get** #get - отримати данні для сторінки [[Сторінка Налаштування]]
#### links
[[Back-end]]
## Topics
```dataview
LIST FROM ""
WHERE contains(file.outlinks, this.file.link)
AND contains(Type, "topic")
```
## Facts
```dataview
LIST FROM ""
WHERE contains(file.outlinks, this.file.link)
AND contains(Type, "fact")
```
## Questions
```dataview
LIST FROM ""
WHERE contains(file.outlinks, this.file.link)
AND contains(Type, "question")
```
## Bugs
```dataview
LIST FROM ""
WHERE contains(file.outlinks, this.file.link)
AND contains(Type, "bug")
```
## Tasks
```dataview
LIST FROM ""
WHERE contains(file.outlinks, this.file.link)
AND contains(Type, "task")
```
## Roots
```dataview
LIST FROM ""
WHERE contains(file.inlinks, this.file.link)
```

## Childs
```dataview
LIST FROM ""
WHERE contains(file.outlinks, this.file.link)
```