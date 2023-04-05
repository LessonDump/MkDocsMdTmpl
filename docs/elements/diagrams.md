# Диаграммы

Эта конфигурация обеспечивает встроенную поддержку диаграмм [Mermaid.js](https://mermaid.js.org/). MkDocs автоматически инициализирует среду выполнения `JavaScript`, когда страница содержит блок кода `mermaid`:

## Блок-схема

``` mermaid
graph LR
  A[Start] --> B{Error?};
  B -->|Yes| C[Hmm...];
  C --> D[Debug];
  D --> B;
  B ---->|No| E[Yay!];
```
