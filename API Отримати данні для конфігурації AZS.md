---
Type: task
tags: 
Data: 2024-02-13
---
 [[Front-End]] буде отримувати данні роблячи post запит у форматі json. Для того щоб відобразити цю сторінку **/main/settings/configuration**([[Сторінка Налаштування]]).

 Інформацію про посилання можна подивитись тут [[Всі URL HTTP]]. Це завдання для [[Back-end]]
## Завдання
1. [ ] Створити шлях **/api/settings/get** на [[Back-end]] у відповідь буде даватись -> [[Json конфігурація AZS]]
#### links

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