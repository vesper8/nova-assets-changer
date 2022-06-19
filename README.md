[![Stand With Ukraine](https://raw.githubusercontent.com/vshymanskyy/StandWithUkraine/main/banner2-direct.svg)](https://vshymanskyy.github.io/StandWithUkraine/)

# Nova Assets Changer

This package is for Nova 4 and swaps the resources from the `resources/Nova/Nova` folder with those in the `vendor/laravel/nova/resources/js` folder or use the `php artisan custom-assets:publish`
command.  
Then the assets are recompiled and published with the Force option.

This package creates a backup of each file and checks for changes

Attention. The original vendor files will be overwritten.

# IMPORTANT

You must run the `php artisan nova:custom-assets` after every composer update!

Tip: You can replace `@php artisan nova:publish` with `@php artisan nova:custom-assets` in Your `composer.json`

## Install

```
composer require norman-huth/nova-assets-changer --dev
```

### Running

For the full process run this command:

```
php artisan nova:custom-assets
```

### Optional

#### Publish Nova Assets Via Command

```
php artisan custom-assets:publish
```

Publish example resources

```
php artisan vendor:publish --provider="NormanHuth\NovaAssetsChanger\PackageServiceProvider"
```

## Notice

After a Nova update, you need to check your resource files to see if they are still compatible.

___

## Examples

I make not a release for every example. For all example resources take a look in the `resources` folder of the GitHub repository

---
[![More Laravel Nova Packages](https://raw.githubusercontent.com/Muetze42/asset-repo/main/svg/more-laravel-nova-packages.svg)](https://huth.it/nova-packages)
