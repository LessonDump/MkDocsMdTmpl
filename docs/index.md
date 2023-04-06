# Главная

[MkDocs](https://www.mkdocs.org/) Project documentation with Markdown.

## Теги страницы

``` markdown
---
title: Lorem ipsum dolor sit amet
---

# Document title
...
```

[Подробнее](elements/reference.md)

## Блоки кода

``` sql
SELECT weight_class, CORR(list_price, min_price) "Correlation"
    FROM product_information
    GROUP BY weight_class
    ORDER BY weight_class, "Correlation";
 
--Результат:    
WEIGHT_CLASS Correlation
------------ -----------
           1  .999149795
           2  .999022941
           3  .998484472
           4  .999359909
           5  .999536087
```

[Подробнее](elements/code_blocks.md)

## Предостережения

!!! Примечание

    Lorem ipsum dolor sit amet, consectetur adipiscing elit. Nulla et euismod
    nulla. Curabitur feugiat, tortor non consequat finibus, justo purus auctor
    massa, nec semper lorem quam in massa.

[Подробнее](elements/admonitions.md)

## Кнопки

[Подробнее](elements/buttons.md){ .md-button }

## Таблицы данных

| Method   | Description                          |
|----------|--------------------------------------|
| `GET`    | :material-check:     Fetch resource  |
| `PUT`    | :material-check-all: Update resource |
| `DELETE` | :material-close:     Delete resource |

[Подробнее](elements/data-tables.md)

## Диаграммы

``` mermaid
graph LR
  A[Start] --> B{Error?};
  B -->|Yes| C[Hmm...];
  C --> D[Debug];
  D --> B;
  B ---->|No| E[Yay!];
```

[Подробнее](elements/diagrams.md)

## Сноски

[Подробнее](elements/footnotes.md)

## Форматирование

++ctrl+alt+del++

[Подробнее](elements/formatting.md)

## Иконки, Эмоджи

[Подробнее](https://squidfunk.github.io/mkdocs-material/reference/icons-emojis/)

## Изображения

![Image title](https://dummyimage.com/300x200/f5f5f5/aaaaaa#only-light)
![Image title](https://dummyimage.com/300x200/21222c/d5d7e2#only-dark)

[Подробнее](elements/images.md)

## Списки

- [x] Lorem ipsum dolor sit amet, consectetur adipiscing elit
- [ ] Vestibulum convallis sit amet nisi a tincidunt
    * [x] In hac habitasse platea dictumst
    * [x] In scelerisque nibh non dolor mollis congue sed et metus
    * [ ] Praesent sed risus massa
- [ ] Aenean pretium efficitur erat, donec pharetra, ligula non scelerisque

[Подробнее](elements/lists.md)
