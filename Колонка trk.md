---
Type: fact
tags: 
Data: 2024-02-23
---
Колонка або TRK це об'єкт де є пістолети які прив'язані до [[Резервуар tank]].  
Він зберігається у [[База даних AZS]] таблиця **trk**
## Структура TRK
```json
{
  "id_trk":"Унікальний код колонки",
  "id_pist":"Унікальний код пістолету",
  "id_tank":"Унікальний код резервуару"
}
```
#### Налаштування колонки
Номер каналу
Діскретність датчику
Флаги
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