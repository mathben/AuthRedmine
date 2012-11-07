AuthRedmine
===========
@date : 7 november 2012
@author : Mathieu Benoit

Plugin of mediawiki to authenficate user on redmine system with api REST.

INSTALLATION
============
# Add the code in the extensions repertory
repOfMediaWiki=/var/www/mediawiki/
cd $repOfMediaWiki/extensions
git clone https://github.com/mathben/AuthRedmine.git

# Change private $emailServer "changeme.com"; in the file AuthRedmine.php

# Add the include in the LocalSettings.php
#authentification with redmine
require_once("$IP/extensions/AuthRedmine/AuthRedmine.php");
$wgAuth = new AuthRedmine();

TODO
============
- Complete other function

