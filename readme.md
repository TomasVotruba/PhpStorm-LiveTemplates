# PhpStorm Live Templates


## Installation

First, find your configuration folder.

	Windows: <your home directory>\.WebIde<version>\config
	Linux: ~\.WebIde<version>\config
	MacOS: ~/Library/Preferences/WebIde<version>

On my linux, it would be `~/.WebIde80/config`. There is a `templates/` directory, that contains XML files with Live Templates.

To allow more template collections, use simply `wget`:

	$ cd ~/.WebIde80/config/templates
	$ wget https://github.com/Zenify/PhpStorm-LiveTemplates/archive/master.zip
	$ unzip master.zip
	$ mv PhpStorm-LiveTemplates-master/* .
	$ rm -r PhpStorm-LiveTemplates-master && rm master.zip && rm readme.md


Restart PhpStorm and profit!