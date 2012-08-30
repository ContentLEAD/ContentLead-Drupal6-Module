//
// Brafton Drupal 6 Module v1.0
// http://www.brafton.com/support
//

CONTENTS OF THIS FILE
---------------------
 * Introduction
 * Requirements
 * Installation
 * Settings
 * Operation

 
Introduction
------------

The Brafton Drupal 6 Module imports articles from the Brafton XML Feed. The content 
is loaded into a newly created content type called News Articles. 


Requirements
------------

Basic Operation
 - Drupal 6.X

Images
 - Content Construction Kit (CCK) Module
 - FileField Module
 - ImageField Module

 
Installation
------------

- Extract the module files from the zip
- Copy the brafton folder into the /sites/all/modules directory

Administer -> Site Building -> Modules
- Enable the Brafton Scheduled Feed Importer in the Feed Parser package and Save


Settings
--------

Administer -> Site Configuration -> Brafton settings

Feed #0 Author - Select user for the author of the Brafton articles
Brafton XML feed URL: Feed #0 - Enter Brafton XML feed URL with "/news" appended to the end
	e.g. http://api.brafton.com/XXXXXXXX-XXXX-XXXX-XXXX-XXXXXXXXXXXX/news


Operation
---------

The importer is triggered by the Drupal cron job. 
http://www.example.com/cron.php