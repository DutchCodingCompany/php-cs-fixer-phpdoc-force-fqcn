# php-cs-fixer-phpdoc-force-fqcn

[php-cs-fixer](https://github.com/FriendsOfPHP/PHP-CS-Fixer) rule to force using FQCN (Fully-Qualified Class Name) in DocBlock comments. 

Fork of [adamwojs/php-cs-fixer-phpdoc-force-fqcn](https://github.com/adamwojs/php-cs-fixer-phpdoc-force-fqcn)

## Installation

You can install the package via composer:

```bash
composer require --dev dutchcodingcompany/php-cs-fixer-phpdoc-force-fqcn
```

## Usage

In your .php-cs-fixer.php file: 

```php
<?php

// PHP-CS-Fixer 2.x syntax
return PhpCsFixer\Config::create()
    // (1) Register \AdamWojs\PhpCsFixerPhpdocForceFQCN\Fixer\Phpdoc\ForceFQCNFixer fixer
    ->registerCustomFixers([
        new \AdamWojs\PhpCsFixerPhpdocForceFQCN\Fixer\Phpdoc\ForceFQCNFixer()
    ])
    ->setRules([
        // ... 
        // (2) Enable AdamWojs/phpdoc_force_fqcn_fixer rule
        'AdamWojs/phpdoc_force_fqcn_fixer' => true,
    ])
    // ...
    ;
```
