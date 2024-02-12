---
Type: topic
tags: 
Data: 2024-02-10
---
Цей проект для операторів заправки.
## Технічні аспекти реалізації AZS
Все можна подивитись тут [[Аспекти технічної реалізації AZS]]
## Переглянути завдання до проекту
Тут -> [[Перегляд завдань]]
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