---
Last modified: 05 June 2024
Class: "[[Класс - Мета класс]]"
tags:
  - Template/01
Шаблон: "[[Шаблон - Мета-заметка]]"
icon: FiCompass
---
## To-Do list
[[To Do List]]

## Организационные заметки
```dataview
table
	without id
	file.link as "Ссылка", type as "Тип"

where
	 Class = link(this.file.name) 
	 AND startswith(file.name, "Шаблон") = false

sort
	type desc,
	file.name asc
```

## Результаты

1. Визуальная новелла "Охотники за историями"
	- Команда из 4 человек: Геймдизайнер (Я), Программист, Геймификатор, Дизайнер
	- Ссылка на игру: https://anroidevel.itch.io/storyhunters
	- Мои задачи
		- ТЗ на разработку, арт [link](https://docs.google.com/document/d/1PbcVF4ACR7gwXOHp960QTTbFoxXX6Spian8BndYrhjw/edit)
		- Ручное тестирование
		- Сценарий в Twine
