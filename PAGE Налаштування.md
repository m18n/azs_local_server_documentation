---
Type: fact
tags: 
Data: 2024-02-14
---
Вкладка Налаштування це конфігурація видів палива, резервуарів, та колонок, Каса.

## Види палива


## Колонки

#### Пістолети 

#### Налаштування колонки


## Резервуари


## Каса




Яке посилання цієї сторінки можна подивитись тут [[Всі URL HTTP]]
#### links
[[Веб сервер AZS]], [[Всі сторінки]]
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