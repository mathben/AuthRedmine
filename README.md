AuthRedmine
===========
@date : 7 november 2012
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
private $emailServer "changeme.com";
```

Add the include in the LocalSettings.php

```php
authentification with redmine
require_once("$IP/extensions/AuthRedmine/AuthRedmine.php");
$wgAuth = new AuthRedmine();
```

SYSTEM PREREQUISITES
--------------------
You need to active the api REST in redmine in administrator tools on the web page.

TODO
----
- Complete other function

Licence
-------
lpgl3

http://www.gnu.org/copyleft/lesser.html

