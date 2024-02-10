---
Type: topic
tags: 
Data: 2024-02-10
---
Технічний фундамент AZS - це веб сервер. Заправок буде багато, і на кожній заправці буде стояти наш [[Веб сервер AZS]]. Веб сервер буде підключений до [[База даних AZS]]. 
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