---
Type: task
tags: 
Data: 2024-02-13
---
 Видає все в одному. Це те само що окремо викликати:
 1. [[API Отримати всі trk]]
 2. [[API Отримати всі tovar]]
 3. [[API Отримати всі tank]]
 4. [[API Отримати kasa]]
 Цей api буде повертати json. Структура json така:
 ```json
 {
	"tovars":[{...}],
	"tanks":[{...}],
	"trks":[{...}],
	"kasa":{}
}
```
 Це будуть масиви об'єктів. Структуру об'єктів можна подивитись тут: [[Вид палива tovar]], [[Резервуар tank]],[[Колонка trk]],[[Каса]]
 [[Front-End]] буде отримувати данні роблячи post запит у форматі json. Для того щоб відобразити цю сторінку [[PAGE Налаштування]].
#### links
[[Всі API]]
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