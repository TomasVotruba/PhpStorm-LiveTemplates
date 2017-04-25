# My Handy PhpStorm Live Templates

![Constructor Live Template](phpstorm_live_templates.png)

## Install

1. Find your folder with live templates XML files:

    - **Linux**: `~/.PhpStormVERSION/config/templates`
    - **MacOS**: `~/Library/Preferences/PhpStormVERSION/templates`
    - **Windows**: `HOME_DIRECTORY\.PhpStormVERSIONS\config\templates`

2. Download XML with Templates

    ```bash
    cd ~/.PhpStorm2017.1/config/templates
    wget https://raw.githubusercontent.com/TomasVotruba/PhpStorm-LiveTemplates/master/tomas_votruba_php.xml
    ```

3. Restart PhpStorm and profit!


## What is in this package?

#### `st`

```php
declare(strict_types=1);
```

#### `ctor`

```php
public function __construct($END$)
{
}
```

#### `pub`

```php
public function $NAME$($ARGS$)
{
    $END$
}
```

#### `pri`

```php
/***/
private function $NAME$($ARGS$)
{
    $END$
}
```

#### `vs`

```php
/**
 * @var string
 */
```

#### `va`

```php
/**
 * @var string[]
 */
```

#### `vi`

```php
/**
 * @var int
 */
```

#### `ra`

```php
/**
 * @return string[]
 */
```
