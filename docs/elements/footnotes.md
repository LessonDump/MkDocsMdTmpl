# Сноски

## Добавление ссылок на сноски

Ссылка на сноску должна быть заключена в квадратные скобки и должна начинаться с символа вставки ^, за которым непосредственно следует произвольный идентификатор, что аналогично стандартному синтаксису ссылок Markdown.

Lorem ipsum[^1] dolor sit amet, consectetur adipiscing elit.[^2]

## Добавление содержимого сноски

Содержимое сноски должно быть объявлено с тем же идентификатором, что и ссылка. Его можно вставить в произвольное место в документе, и он всегда отображается внизу страницы. Кроме того, автоматически добавляется обратная ссылка на сноску.

### На одной линии

[^1]: Lorem ipsum dolor sit amet, consectetur adipiscing elit.

### На несколько строк

Абзацы могут быть написаны на следующей строке и должны иметь отступ в четыре пробела:

[^2]:
    Lorem ipsum dolor sit amet, consectetur adipiscing elit. Nulla et euismod
    nulla. Curabitur feugiat, tortor non consequat finibus, justo purus auctor
    massa, nec semper lorem quam in massa.


