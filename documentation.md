##Documentation

```
$ tree -tL 2 > totrash.txt


.
├── totrash.txt :personnal file to doc
├── vendor: External vendor module (don't touch)
│   ├── autoload.php
│   ├── composer
│   ├── zendframework
│   ├── doctrine
│   ├── slm
│   ├── bin
│   ├── phpunit
│   ├── symfony
│   ├── knmnyn
│   ├── dyve
│   ├── dagwieers
│   ├── citation-style-language
│   ├── MartinPaulEve
│   ├── README.md
│   └── xmlps
├── composer.phar
├── module
│   ├── PdfConversion
│   ├── ReferencesConversion
│   ├── User : (Auth+Registration+Password)
│   ├── XmpConversion
│   ├── ZipConversion
│   ├── Admin : (Super user to manages User)
│   ├── Api: (simple rest api to submit and retrieve jobs and to provides funcitonality for the front end)
│   ├── Application : (Zend framework application)
│   ├── BibtexConversion
│   ├── BibtexreferencesConversion
│   ├── CitationstyleConversion
│   ├── DocxConversion
│   ├── EpubConversion
│   ├── HtmlConversion
│   ├── Manager :(receives conversion jobs + Job list+ Handles job distribution to queues)
│   └── NlmxmlConversion
├── phpunit.xml (php unit...)
├── public
│   ├── css
│   ├── favicon.ico
│   ├── fonts
│   ├── img
│   ├── index.php
│   └── js
├── start_queues.sh :(Shelll process to start queues on Document conversion type)
├── style : (this folder is required by /assets.yml I think it's a requirement for ZendFramework)
│   ├── css
│   └── scss
├── unittest.sh :(shell script to start phpunit)
├── var :(shell script to start phpunit)
│   ├── documents
│   ├── uploads
│   ├── cache
│   └── doctrine
├── assets.yml :(calling the assets to compile or to output the path)
├── BatchTestSuite.php :(script that sends a document corpus to the markup server and collects conversion success for Statistic:... ask more about that file)
├── composer.json
├── composer.lock
├── config :(Zend Framework related)
│   ├── autoload
│   └── application.config.php
├── docs :(not sure if it's important)
│   ├── fonts
│   └── init.d
├── Guardfile
├── init_autoloader.php
├── javascript (assets...why does the js and stylesheets are in the root...is it a Zend framework convention)
│   ├── footable.js
│   ├── jquery-2.0.3.js
│   ├── jquery.autocomplete.js -> ../vendor/dyve/jquery-autocomplete/src/jquery.autocomplete.js
│   └── script.js
├── LICENSE
├── README.md
└── UnitTestBootstrap.php (I don't know ... must be for Zend Framework)

50 directories, 23 files



todo:
Look at composer.json and go to each github repositories
```
-----------
Documentation to install xmlp

1. 	go to github and follow the instructions
2. 	php -S 0.0.0.0:8080 -t public/ public/index.php 


-----------
Documentation to install ZendFramework 2

```
mkdir new_directory
composer create-project -n -sdev zendframework/skeleton-application path/to/new_directory
curl -s https://getcomposer.org/installer | php 
php composer.phar require coolcsn/csn-user:0.1.0

```

#####https://www.youtube.com/watch?v=L29onMRiP3U 8:42
