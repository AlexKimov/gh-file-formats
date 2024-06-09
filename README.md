# Описание

Форматы файлов и инструменты для игр от Haggard Games. Описание форматов в виде шаблонов для 16ричного редактора.  

### Краткое введение в форматы файлов

##### Игровые ресурсы   
Файлы находятся в архивах VFS, ресурсы разделены по назначению: модели, текстуры и т.д.. Для сжатия данных используется zlib.

##### Форматы для моделей и текстур  
Для текстур используются форматы DDS. Модели находятся в файлах SMF. Анимации для моделей в файлах SKL.

## Форматы

#### Смерть Шпионам (2007)

| № | Формат  | Шаблон (010 Editor) |  Описание   |
| :-- | :------- | :-- |  :-- | 
|  **1**  | SKL | [SKL.bt](templates/010editor/SKL.bt)  | анимации для трехмерных моделей | 
|  **2**  | SMF | [SMF.bt](templates/010editor/SMF.bt)  | трехмерные модели | 
|  **3**  | VFS | [VFS.bt](templates/010editor/VFS.bt)/[VFS_FILESREC.bt](templates/010editor/VFS_FILESREC.bt)  | ресурсы игр | 

    Как использовать скрипты  010Editor
    0. Установить 010Editor.
    1. Открыть нужный файл.
    2. Применить скрипт через меню Script-Run script. 

## Инструменты

#### QuickBms

| № | Скрипт | Описание  |
| :-- | :------- | :-------  | 
| **1**  | [unpack_vfs.bms](scripts/qbms/unpack_vfs.bms)  | распаковка архивов игры VFS |   

    Как использовать quickbms скрипты
    1. Нужен quickbms https://aluigi.altervista.org/quickbms.htm
    2. Для запуска в репозитории лежит bat файл с настройками, нужно открыть его и задать свои пути: до места, где находится quickbms, папки с игрой и места куда нужно сохранить результат.
    3. Запустить процесс через bat файл или вручную (задав свои параметры для запуска quickbms, документация на английском есть здесь https://aluigi.altervista.org/papers/quickbms.txt ). 
