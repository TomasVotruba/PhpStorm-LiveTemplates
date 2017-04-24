# My Handy PhpStorm Live Templates

## Install

Find your folder with live templates XML files:

- **Linux**: `~/.PhpStormVERSION/config/templates`
- **MacOS**: `~/Library/Preferences/PhpStormVERSION/templates`
- **Windows**: `HOME_DIRECTORY\.PhpStormVERSIONS\config\templates`

On my Linux, it would be `~/.PhpStorm2017.1/config/templates`.

### Download and Unpack This Package

```bash
cd ~/.PhpStorm2017.1/config/templates
wget https://github.com/TomasVotruba/PhpStorm-LiveTemplates/archive/master.zip
unzip master.zip
mv PhpStorm-LiveTemplates-master/* .
rm -r PhpStorm-LiveTemplates-master && rm master.zip && rm README.md
```

Restart PhpStorm and profit!


## Live Templates

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

#### pub

```php
public function $NAME$($ARGS$)
{
    $END$
}
```

#### pri

```php
/***/
private function $NAME$($ARGS$)
{
    $END$
}
```

#### vs

```php
/**
 * @var string
 */
```

#### va

```php
/**
 * @var string[]
 */
```

#### vi

```php
/**
 * @var int
 */
```

#### ra

```php
/**
 * @return string[]
 */
```
