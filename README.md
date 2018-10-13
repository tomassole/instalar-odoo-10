# Instalación de Odoo 10

## str/str

```linux
$str = new Str('Hello, 世界');
$str->last(2); // 世界
$str->chars(); // ['世', '界']

$str
    ->ensureLeft('Hello, ') // Hello, 世界
    ->ensureRight('!!!') // Hello, 世界!!!
    ->trimRight('!') // Hello, 世界
    ->prepend('Str say - '); // Str say - Hello, 世界

$send = function (string $s) {};
$send((string)$str); // same
$send($str->getString()); // same
```


---------------------
