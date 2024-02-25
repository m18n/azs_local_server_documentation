---
Type: fact
tags:
  - post
Data: 2024-02-25
---
Це api приймає данні в json. В json повинно бути вказано всі об'єкти такі як: [[Вид палива tovar]], [[Резервуар tank]], [[Колонка trk]], [[Каса]]
```json
{
	"tovars":[{...}],
	"tanks":[{...}],
	"trks":[{...}],
	"kasa":{}
}
```
Де вказано три крапки там будуть ті данні кожного об'єкту. Структуру даних об'єктів можна подивитись якщо зайти на них. Кожне поле повинно бути вказано. 
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