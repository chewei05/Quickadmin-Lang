# Quickadmin-lang

 [![Latest Stable Version](https://poser.pugx.org/chewei05/quickadmin-lang/v/stable)](https://packagist.org/packages/chewei05/quickadmin-lang) 
[![Total Downloads](https://poser.pugx.org/chewei05/quickadmin-lang/downloads)](https://packagist.org/packages/chewei05/quickadmin-lang)
[![Latest Unstable Version](https://poser.pugx.org/chewei05/quickadmin-lang/v/unstable)](https://packagist.org/packages/chewei05/quickadmin-lang)
[![License](https://poser.pugx.org/chewei05/quickadmin-lang/license)](https://packagist.org/packages/chewei05/quickadmin-lang)

    Traditional Chinese (zh-TW) Language for Quickadmin 2.x
    Quickadmin 2.x 的正體中文(繁體中文)語系檔.

## Requirements
    laraveldaily/quickadmin: ^2.1.0

## Installation
Open the root directory of your Laravel project in terminal(CLI), and follow the following steps.

1. Install [**laraveldaily/quickadmin**](https://github.com/LaravelDaily/quickadmin) first.
    ```
    composer require laraveldaily/quickadmin
    ```
2. Install this package **QuickAdmin-Lang**
    ```
    composer require chewei05/quickadmin-lang
    ```
## Copy Language Files

### Copy Directly
* Files of languages are in "vendor/chewei05/src/lang" directory
* Copy the folders of languages to the *resources/lang/vendor/laraveldaily* folder of your Laravel 5 project.

### Via Laravel Service Provider

1. Add service provider to **config/app.php**.
    ```php
    'providers' => [
        ...

        CheweiHu\QuickadminLang\QuickadminLangServiceProvider::class,
    ],
    ```
2. Run *composer dump-autoload* if composer went wrong.
    ```
    composer dump-autoload
    ```
3. Publish vendor files of this package.
    ```
    php artisan vendor:publish --provider="CheweiHu\QuickadminLang\QuickadminLangServiceProvider"
    ```
4. Done.

