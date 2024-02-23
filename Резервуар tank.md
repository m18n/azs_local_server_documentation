---
Type: fact
tags: 
Data: 2024-02-23
---
Резервуар це об'єкт для якого потрібно прив'язати [[Вид палива tovar]] для того щоб визначити що це резервуар.
Він зберігається у [[База даних AZS]] таблиця **tank**
## Структура tank
```json
{
  "id_tank":"Унікальний код резервуару",
  "id_tovar":"Унікальний код види палива",
  "valume":"Максимальна заповнюваність резервуара",
  "remain":"Мертвий залишок у ньому"
}
```
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