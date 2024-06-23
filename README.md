<div align=center>
    
# Парсер документации python

![Python](https://img.shields.io/badge/python-3670A0?style=for-the-badge&logo=python&logoColor=ffdd54)

</div>

## Описание проекта

Данный парсер умеет:

1. Собирать ссылки на статьи о нововведениях в Python, переходить по ним и забирать информацию об авторах и редакторах статей.
2. Собирать информацию о статусах версий Python.
3. Скачивать архив с актуальной документацией.
4. Выводить результат в консоль в обычном формате, в виде таблицы или в файл csv.

## Технологии

- Python 3.10.11
- beautifulsoup4 4.12.3
- tqdm 4.66.4
- prettytable 2.1.0

## Запуск проекта

1. Cклонировать проект:

```bash
git clone git@github.com:JustLight1/parser_docs_python.git
```

2. Создать виртуальное окружение и активировать:

```bash
python -m venv venv
source venv/Scripts/activate - windows
```

3. Установить библиотеки из файла requirements.txt:

```bash
pip install -r requirements.txt
```

4. Перейти в директорию src для дальнейшей работы:

```bash
cd src/
```

## Пример работы парсера

Парсер может работать в разных режимах с разными аргументами:

```bash
usage: main.py [-h] [-c] [-o {pretty,file}]
               {whats-new,latest-versions,download}
```

1. Режимы работы парсера:

   positional arguments:
   whats-new - Парсинг новостей
   latest-versions - Парсинг версий
   download - Загрузка архива с документацией в формате pdf

2. Дополнительные аргументы:

   optional arguments:
   -h, --help "show this help message and exit"
   -c, --clear-cache "Очистка кеша"
   -o {pretty,file}, --output {pretty,file} "Дополнительные способы вывода данных"
