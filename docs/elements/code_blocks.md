# Блоки кода

## [Лексеры для блоков кода](https://pygments.org/docs/lexers/)

## Лексера `py`:

``` py
@dp.message_handler(commands=['start', 'help'])
async def send_welcome(message: types.Message):
    await message.answer(
        MESSAGES['welcome'], parse_mode=types.ParseMode.MARKDOWN)
```

## Лексера `sql`:

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

## Лексера `html`:

``` html
<!DOCTYPE html>
<html lang="ru-RU">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1">
<meta name="viewport" content="width=device-width">

<title>SQL Helper</title>
```

## Лексера `css`:

``` css
.row {
    margin-right: -10px;
    margin-left: -10px;
}

.col-md-4,
.col-xs-6,
.col-sm-4 {
    float: left;
    min-height: 1px;
    position: relative;
}

.list-grp {
    border: 0;
    border-radius: 0;
    box-shadow: 0 0 0;
    margin: 0;
}
```

## Лексера `kotlin`:

``` kotlin
class MainActivity : AppCompatActivity() {

    private lateinit var binding: ActivityMainBinding

    @SuppressLint("SetJavaScriptEnabled")
    override fun onCreate(savedInstanceState: Bundle?) {
        super.onCreate(savedInstanceState)
        binding = ActivityMainBinding.inflate(layoutInflater)
        setContentView(binding.root)

        binding.webView.webViewClient = MyWebViewClient()

        binding.webView.apply {
            with(settings) {
                this.javaScriptEnabled = true
                this.builtInZoomControls = true
                this.displayZoomControls = false
            }
        }

        if (savedInstanceState == null) {
            binding.webView.loadUrl("file:///android_asset/index.html")
        }
    }
}
```

## Блок кода с заголовком:

``` py title="bubble_sort.py"
def bubble_sort(items):
    for i in range(len(items)):
        for j in range(len(items) - 1 - i):
            if items[j] > items[j + 1]:
                items[j], items[j + 1] = items[j + 1], items[j]
```

## Блок кода с аннотацией:

``` yaml
theme:
  features:
    - content.code.annotate # (1)
```

1. :man_raising_hand: I'm a code annotation! I can contain `code`, __formatted
    text__, images, ... basically anything that can be written in Markdown.

## Блок кода с аннотацией, зачищенный (удалён символ комментария):

``` yaml
theme:
  features:
    - content.code.annotate # (1)!
```

1.  Look ma, less line noise!

## Блок кода с номерами строк:

``` py linenums="1"
def bubble_sort(items):
    for i in range(len(items)):
        for j in range(len(items) - 1 - i):
            if items[j] > items[j + 1]:
                items[j], items[j + 1] = items[j + 1], items[j]
```

## Блок кода с выделенными строками

``` py hl_lines="2 3"
def bubble_sort(items):
    for i in range(len(items)):
        for j in range(len(items) - 1 - i):
            if items[j] > items[j + 1]:
                items[j], items[j + 1] = items[j + 1], items[j]
```

## Блок встроенного кода

Функция `#!py range()` используется для генерации последовательности чисел.
