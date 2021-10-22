# OpenGraph

This is a fork of [hiroyukisato/mediawiki-extensions-OpenGraph](https://github.com/hiroyukisato/mediawiki-extensions-OpenGraph) with the [fix](https://github.com/hiroyukisato/mediawiki-extensions-OpenGraph/pull/2) by `bertrandgorge` applied and the README translated into English.
## Summary

Adds OGP and Twitter Card metadata to articles.

## Installation
This extension depends on [Extension:PageImages](https://www.mediawiki.org/wiki/Extension:PageImages) and [Extension:TextExtracts](https://www.mediawiki.org/wiki/Extension:TextExtracts).

LocalSettings.php
```php
 wfLoadExtension( 'OpenGraph' );
```

## Settings

```$ogpTwitter``` You can set the Twitter account (sets `twitter:site`).

```php
 $ogpTwitter = '@48pedia' //optional
```
