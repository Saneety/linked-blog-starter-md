---
Last modified: 31 May 2024
Class: "[[Main - Столица заметок]]"
tags:
  - Template/01
Type: Обсидиан
---
```plantuml
!theme sunlust
autonumber
skinparam MaxMessageSize 150
footer "Это футер"

Сканер -> Папка_In1: Положить скан в папку In1
Папка_In1 -> Папка_L1: RS ищет ШК и перекладывает в папку L1
Папка_L1 -> Папка_In2: Aryan проверяет ШК == DS_Documents.Barcode ? и перекладывает в папку In2
Папка_In2 -> Папка_L2: RS распознает текст и перекладывает в папку L2
Папка_L2 -> БД: Aryan сохраняет файл в БД
```

```plantuml
autonumber

Сканер -> RS: Положить файл в In1
RS -> RS: Найти файл в In1
RS -> RS: Распознать и внести ШК в файл
RS -> Aryan: Положить файл в L1
Aryan -> Aryan: Найти файл в L1
Aryan -> Aryan: ШК есть в DS_Documents.Barcode?
Aryan --> RS: Положить файл в In2
RS -> RS: Найти файл в In2
RS -> RS: Распознать и внести текст в файл
RS -> Aryan: Положить файл в L2
Aryan -> БД: Сохранить файл в БД
```
