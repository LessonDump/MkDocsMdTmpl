# Главная

[MkDocs](https://www.mkdocs.org/) Project documentation with Markdown.

### Теги страницы

``` markdown
---
title: Lorem ipsum dolor sit amet
---

# Document title
...
```

[Подробнее](elements/reference.md)

### Блоки кода

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
