# OpenGraph

Adds OGP and Twitter Card metadata to articles.

This is a fork of [hiroyukisato/mediawiki-extensions-OpenGraph](https://github.com/hiroyukisato/mediawiki-extensions-OpenGraph) with the [fix](https://github.com/hiroyukisato/mediawiki-extensions-OpenGraph/pull/2) by Bertrand Gorge applied, the README translated into English, and some further tweaks made:
1. Fix the description in Special:Version
1. Use `$wgLogos['1x']` (instead of deprecated`$wgLogo`) by default if there is no image identified by [Extension:PageImages](https://www.mediawiki.org/wiki/Extension:PageImages)
   * Also fixed to use fully-qualified URL
1. Add `twitter:title`, `twitter:description`, `twitter:image` meta tags in addition to `og:title`, `og:description`, and `og:image`

I do not know what I am doing, use at your own risk :-)

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
