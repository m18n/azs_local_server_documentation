---
Type: fact
tags: 
Data: 2024-02-23
---
Вид палива це об'єкт який визначає паливо та його характеристики.
Він зберігається у [[База даних AZS]] таблиця **tovar**
## Структура вида палива
```json
{
  "id_tovar":"Унікальний код вида палива",
  "name":"Коротка назва вида палива",
  "price":"Ціна вида палива",
  "name_p":"Коротка назва для каси",
  "name_p_f":"Довга назва для каси",
  "name_p_v":"Одиниця вимірювання для каси",
  "color":"Кольор палива"
}
```
#### links
[[База даних AZS]], 
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