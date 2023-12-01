---
kanban-plugin: basic
created: <% tp.file.creation_date("yyyy-MM-DD") %>
tags:
  - semanal
people: 
publish: false
name: Tool
site: https://tool.io/
status:
  - hold|assess|trial|adopt
topic:
  - machine learning
  - frontend
  - systems
history:
  - 2021-03-14: adopt
type: reuniao
company: 
summary:
---

# Tópico
- 

# Conceitos
- 

# Notas
- 
# Perguntas
- 
# <% moment(tp.file.title,'YYYY-MM-DD').format("dddd, MMMM DD, YYYY") %>

Um ano atrás: [[<% tp.date.now("YYYY-MM-DD", "P-1Y") %>]]

<< [[<% tp.date.now("YYYY-MM-DD", -1, tp.file.title, "YYYY-MM-DD") %>]] | [[<% tp.date.now("YYYY-MM-DD", 1, tp.file.title, "YYYY-MM-DD") %>]]>>

---
### 📅 Questões diárias
- 

---
# 📝 Notas
- 

---
### Notes created today
```dataview
List FROM "" WHERE file.cday = date("<% tp.date.now("YYYY-MM-DD")%>") SORT file.ctime asc
```

### Notes last touched today
```dataview
List FROM "" WHERE file.mday = date("<% tp.date.now("YYYY-MM-DD") %>") SORT file.mtime asc
```
# Tool
Brief description of the tool.

## Reasoning for

## Reasoning against

## Alternatives considered

## Resources
Link to relevant blog posts here.


<%*
  let title = tp.file.title
  if (title.startsWith("Untitled")) {
    title = await tp.system.prompt("Title");
    await tp.file.rename(title);
  } 
  tR += "---"
%>
title: <%* tR += title %>
created: <% tp.file.creation_date("yyyy-MM-DD") %>
aliases: 
tags: []
note_status: working
publish: false
---
<%*
  let title = tp.file.title
  if (title.startsWith("Untitled")) {
    title = await tp.system.prompt("Title");
    await tp.file.rename(title);
  } else {
	  let title = tp.file.title
  }
  tR += "---"
%>
company:
location:
title:  <%* tR += title %>
email:
aliases:
languages:
publish: false
date_last_spoken:
follow_up:
---
# <% title %>

<% await tp.file.move("pessoa/" + title) %>
# [[<% TP.FILE.TITLE %>]]

## Participantes

- 

## Agenda



## Log



## Próximas ações




![[{{sunday:gggg-MM-DD}}]]
![[{{monday:gggg-MM-DD}}]]
![[{{tuesday:gggg-MM-DD}}]]
![[{{wednesday:gggg-MM-DD}}]]
![[{{thursday:gggg-MM-DD}}]]
![[{{friday:gggg-MM-DD}}]]
![[{{saturday:gggg-MM-DD}}]]