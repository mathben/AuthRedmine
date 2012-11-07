AuthRedmine
===========
@date : november 2012

@author : Mathieu Benoit

Plugin of mediawiki to authenficate user on redmine system with api REST.

INSTALLATION
------------
Add the code in the extensions repertory

```bash
repOfMediaWiki=/var/www/mediawiki/
cd $repOfMediaWiki/extensions
git clone https://github.com/mathben/AuthRedmine.git
```

Adapt the following line in the file AuthRedmine.php
```php
	private $emailServer = "changeme.com";
	private $hostname = "127.0.0.1";
```

Add the include in the LocalSettings.php

```php
authentification with redmine
require_once("$IP/extensions/AuthRedmine/AuthRedmine.php");
$wgAuth = new AuthRedmine();
```

Contributing
------------
[Pull requests][] are welcome.

SYSTEM PREREQUISITES
--------------------
You need to active the api REST in redmine in administrator tools on the web page.

TODO
----
- Complete other function

Licence
-------
The AuthRedmine is released under [Lpgl3 License][]

[Lpgl3 License]: http://www.gnu.org/copyleft/lesser.html
[Pull requests]: http://help.github.com/send-pull-requests

