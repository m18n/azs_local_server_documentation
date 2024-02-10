---
Type: fact
tags: 
Data: 2024-02-10
---
Тут написані всі посилання back-end
1. **/public/(path)** #get path це шлях до любого файлу в папці azs_site
2. **/** #get це шлях до авторизації файл **login.html**
3. **/auth** #post  це сторінка для підтвердження авторизації та отримання вдалості. якщо вхід вдалий то повертається в json {"status": "yes"} якщо ні то {"status":"no"}
4. **/settings/dberror** #get  це сторінка налаштування бази даних при відсутності підключення до неї. Видає файл **settings_db_error.html**
5. **/settings/dberror/send** #post  це сторінка для відправки даних на підключення якщо дані записались то відправляється у відповідь {"status": "yes"} якщо ні то {"status":"no"}
6. **/settings/dberror/check** #post - це сторінка для отримання інформації про підключення. На нього потрібно робити постійні запити при підключенні до бази щоб знати  статус. він повертає такі статуси {"status": "process"} {"status": "connect"} {"status": "disconnect"} по назвам я думаю все зрозуміло.
#### links
[[Back-end]]
## Facts
```dataview
LIST FROM ""
WHERE contains(file.outlinks, this.file.link)
AND contains(Type, "fact")
```
## Topics
```dataview
LIST FROM ""
WHERE contains(file.outlinks, this.file.link)
AND contains(Type, "topic")
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