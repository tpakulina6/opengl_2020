# Репозиторий для приема заданий по компьютерной графике // ФИВТ МФТИ 2019 // Семинарист Якимушкина А.О.
## План занятий и сдач
За изменениями следите в tg-канале.

Ссылки на семинары доступны в [Wiki проекта](https://bitbucket.org/arina5arina/opengl_tasks_2020/wiki/Home).

№ | Дата | Тема
-:|-------|------------------|
1 | 08 февраля | Семинар
2 | 15 февраля | Семинар
- | 22 февраля | Неучебный день - олимпиада МФТИ
3 | 29 февраля | Семинар
4 | 7 марта | [Прием задания 1](https://bitbucket.org/arina5arina/opengl_tasks_2020/wiki/Home)
5 | 14 марта | Семинар
6 | 21 марта | Семинар
7 | 28 марта | Семинар
8 | 4 апреля | Семинар
9 | 11 апреля | Семинар
10 | 18 апреля | [Прием задания 2](https://bitbucket.org/arina5arina/opengl_tasks_2020/wiki/Home)
11 | 25 апреля | Семинар
? | 2 мая | Семинар
- | 9 мая | День Победы
12 | 16 мая | Семинар
13 | 23 мая | [Прием задания 3](https://bitbucket.org/arina5arina/opengl_tasks_2020/wiki/Home)

## Краткое руководство по встраиванию

* Создайте форк этого репозитория.
* Для каждого задания выделена отдельная папка (*task1*, *task2*).
* В папке с заданием создайте свою папку `<номер группы><фамилия на латинице>` (например, *123Ivanov*), работайте только в этой папке.
* Создайте вложенную подпапку `<номер группы><фамилия на латинице>Data<номер задания>` (например, *123IvanovData1*). Используйте эту папку для размещения загружаемых в программе файлов (3D модели, изображения и т.д.).
* В папке `<номер группы><фамилия на латинице>` создайте файл CMakeLists.txt следующего содержимого

```
set(SRC_FILES
    Main.h
    Main.cpp
)

MAKE_OPENGL_TASK(123Ivanov 1 "${SRC_FILES}")
```

Здесь в переменной **SRC_FILES** укажите имена ваших файлов с исходным кодом.
    
В аргументах макроса **MAKE_OPENGL_TASK** укажите имя папки и номер задания (1, 2 или 3).

### Образец
В репозитории приведены примеры: задание 2 по OpenGL (скопированы из примеров к курсу).

### Зависимости
Не рекомендуется инклюдить файлы из примеров оформления задания: они общие, вдруг вам понадобится что-то поменять.
Скопируйте всё, что вам нужно.