# hello-composer


```php
namespace emacle\HelloComposer; // 自定义命名空间，注意不要与已有的重复

class HelloComposer
{
    // 静态方法 static 使用时，可不用声明类，直接调用方法
    public static function greet()
    {
        echo "Hello, Composer!", PHP_EOL;
    }
}
```

```
composer require emacle/hello-composer
```

```php
use emacle\HelloComposer\HelloComposer;  // 引入 namespace 并加入类名 HelloComposer

<?php
    $test = new HelloComposer(); // 声明类 HelloComposer
    var_dump($test->greet()); // 调用 HelloComposer类方法 greet()
   
    var_dump(HelloComposer::greet()); // 如果类方法greet为 static 方法则不用声明直接调用
```
