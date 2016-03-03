# PhpStorm Live Templates

## Installation

First, find your configuration folder.

	Windows: <your home directory>\.WebIde<version>\config
	Linux: ~\.WebIde<version>\config
	MacOS: ~/Library/Preferences/WebIde<version>

On my linux, it would be `~/.WebIde110/config`. There is a `templates/` directory, that contains XML files with Live Templates.

To allow more template collections, use simply `wget`:

	$ cd ~/.WebIde110/config/templates
	$ wget https://github.com/Zenify/PhpStorm-LiveTemplates/archive/master.zip
	$ unzip master.zip
	$ mv PhpStorm-LiveTemplates-master/* .
	$ rm -r PhpStorm-LiveTemplates-master && rm master.zip && rm README.md


Restart PhpStorm and profit!


## Live Templates

### PHP Templates

#### ctor

```php
public function __construct($END$)
{
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

#### pro

```php
/***/
protected function $NAME$($ARGS$)
{
    $END$
}
```

#### pub

```php
public function $NAME$($ARGS$)
{
    $END$
}
```

#### id

```php
/**
 * {@inheritdoc}
 */
```

#### try

```php
try {
	$SELECTION$

} catch ($EXCEPTION_TYPE$ $exception) {
	$END$
}
```

#### t

```php
$this->$END$
```

### Doctrine Templates

#### col

```php
/**
 * @ORM\Column(type="$TYPE$", nullable=TRUE)
 * @var $TYPE$$END$
 */
private $$$PROPERTY$;
```

#### oto

```php
/**
 * @ORM\OneToOne(targetEntity="$TYPE$", $COMPLETE$="$INVERSE_PROPERTY$"$END$, cascade={"persist"})
 * @ORM\JoinColumn(name="$PROPERTY$_id", referencedColumnName="id")
 * @var $TYPE$
 */
private $$$PROPERTY$;
```

#### otm

```php
/**
 * @ORM\OneToMany(targetEntity="$TYPE$", mappedBy="$OTHER_PROPERTY$"$END$, cascade={"persist"})
 * @var $TYPE$
 */
private $$$PROPERTY$;
```

#### mto

```php
/**
 * @ORM\ManyToOne(targetEntity="$TYPE$", inversedBy="$OTHER_PROPERTY$"$END$, cascade={"persist"})
 * @ORM\JoinColumn(name="$COL$_id", referencedColumnName="id")
 * @var $TYPE$
 */
private $$$PROPERTY$;
```

#### mtm

```php
/**
 * @ORM\ManyToMany(targetEntity="$TYPE$", $COMPLETE$="$INVERSE_PROPERTY$"$END$, cascade={"persist"})
 * @ORM\JoinTable(name="$TABLE_NAME$",
 * 		joinColumns={@ORM\JoinColumn(name="$JOIN_COL$_id", referencedColumnName="id")},
 * 		inverseJoinColumns={@ORM\JoinColumn(name="$INVERSE_COL$_id", referencedColumnName="id")} 
 * 	)
 * @var $TYPE$[]|\Doctrine\Common\Collections\ArrayCollection
 */
private $$$PROPERTY$;
```

#### uid

```php
	/**
	 * @ORM\Id
	 * @ORM\Column(type="string", length=36)
	 * @var $END$Id
	 */
	private $id;
```

#### uc

```php
uniqueConstraints={
*        @ORM\UniqueConstraint(name="$NAME$", columns={"$COLUMN1$", "$COLUMN2$"})     
* }
```

## Next Inspiration

- If you love Symfony, check [live templates from @knpuniversity](https://github.com/knpuniversity/phpstorm-settings).
- If you love Nette, check [live templates from @fprochazka](https://github.com/fprochazka/phpstorm-livetemplates)
