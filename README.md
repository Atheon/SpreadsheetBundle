# SpreadsheetBundle

This is a Symfony 3/4/5 Bundle helps you to read and write Spreadsheet files (including pdf, xls, xlsx, odt, csv), thanks to the PHPSpreadsheet library.

[![Total Downloads](https://poser.pugx.org/atheon/SpreadsheetBundle/downloads.png)](https://packagist.org/packages/roromix/SpreadsheetBundle)
[![Latest Stable Version](https://poser.pugx.org/atheon/SpreadsheetBundle/v/stable.png)](https://packagist.org/packages/roromix/SpreadsheetBundle)
[![Latest Unstable Version](https://poser.pugx.org/atheon/SpreadsheetBundle/v/unstable.png)](https://packagist.org/packages/roromix/SpreadsheetBundle)

## Forked from
https://github.com/roromix/SpreadsheetBundle

## Supported formats

The supported formats are sames of PhpSpreadsheet (Open Document .ods, Office Excel .xlsx, BIFF 8 .xls, CSV, PDF).

## Installation

**1**  Add to composer.json to the `require` key

``` json
    "repositories": [
        {
            "type": "vcs",
            "url": "https://github.com/Atheon/SpreadsheetBundle"
        }
    ],
    "require": {
        ....
        "atheon/spreadsheetbundle": "1.0.*",
    },
``` 

**2** Register the bundle :

Symfony standard installation : ``app/AppKernel.php``
``` php
    $bundles = array(
        // ...
        new Roromix\Bundle\SpreadsheetBundle\RoromixSpreadsheetBundle(),
    );
```
Symfony Flex installation (normaly, it's auto-generated) : ``config/bundles.php``
``` php
    return [
        // ...
        Roromix\Bundle\SpreadsheetBundle\RoromixSpreadsheetBundle::class => ['all' => true],
    ];
```

## License

This bundle is under the MIT license. See the complete license in the bundle:

[![License](https://poser.pugx.org/roromix/SpreadsheetBundle/license.png)](LICENSE)
