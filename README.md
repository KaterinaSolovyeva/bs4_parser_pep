# Проект парсинга PEP и официального сайта документации Python
В данном проекте реализованы:
- парсер, который собирает информацию о версиях Python — номера, статусы (in development, pre-release, stable и так далее) и ссылки на документацию. 
- парсер данных обо всех документах PEP
- сравнение статусов на странице PEP со статусом в общем списке
- посчитано количество PEP в каждом статусе и общее количество PEP
- возможность сохранения результатов в табличном виде в csv-файле
Итоговая таблица состоит из двух колонок: «Статус» и «Количество». Последняя строка таблицы Total показывает общее количество PEP.
# Как запустить проект:

Клонировать репозиторий и перейти в него в командной строке:
```
git clone https://github.com/KaterinaSolovyeva/bs4_parser_pep

```
```
cd bs4_parser_pep
```
- Установите и активируйте виртуальное окружение
- Установите зависимости из файла requirements.txt
```
pip install -r requirements.txt
```
- Перейдите в папку src
- Можете обращаться к парсеру через командную строку. Пример:
Документацию Python можно скачать на ваш локальный диск с помощью команды
```
python main.py download

```
# Другие команды парсера:
usage: main.py [-h] [-c] [-o {pretty,file}] {whats-new,latest-versions,download,pep}

Парсер документации Python

positional arguments:
  {whats-new,latest-versions,download,pep}
                        Режимы работы парсера

optional arguments:
  -h, --help            show this help message and exit
  -c, --clear-cache     Очистка кеша
  -o {pretty,file}, --output {pretty,file}  Дополнительные способы вывода данных
