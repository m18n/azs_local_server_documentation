---
Type: topic
tags: 
Data: 2024-02-10
---
База даних буде розміщена на кожній заправці(AZS). В неї записується все від запуску насосів палева і до товарів. 
#### links
[[AZS]]
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