---
Last modified: 30 May 2024
Class: "[[Класс - Тематика]]"
tags:
  - Template/01
  - RefactorVersion/1
---

```dataview
table
	without id
	file.link as "Ссылка"

where
	contains(Theme, link(this.file.name))
```