---
Type: fact
tags: 
Data: 2024-02-10
---
Тут написані всі посилання back-end
## System
1. **/public/(path)** #get  [[BACK_C Отримати public файли]]
2. **/settings/dberror** #get  **~** [[PAGE База Даних]]  **~** [[BACK_С База Даних PAGE]]
3. **/settings/dberror/send** #post   [[BACK_C Зміна даних підключення до БД]]
4. **/settings/dberror/check** #post -  [[BACK_C Статус підключення до бази даних]]
## Auth
1. **/** #get **~** [[PAGE Авторизація]] **~** [[BACK_С Авторизація PAGE]]
2. **/auth** #post **~**[[BACK_C Підтвердження авторизації]]
## Main
1. **/main** #get **~**[[PAGE Головна]]**~** [[BACK_С Головна PAGE]]
2. **/main/settings** #get **~**[[PAGE Сервіси]] **~** [[BACK_С Сервіси PAGE]]
3. **/main/settings/configuration** #get **~** [[PAGE Налаштування]] **~** [[BACK_С Налаштування PAGE]]
## API
1. **/api/pump/save** #post **~** [[API Зберігання положення TRK]]
2. **/api/out** #get **~** [[API Вихід з Акаунту]] 
3. **/api/outshift/** #get **~** [[API Закриття зміни]]
4. **/api/settings/get** #get  **~** [[API Отримати данні для конфігурації AZS]] 
#### links
[[Back-end]], [[Веб сервер AZS]]
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