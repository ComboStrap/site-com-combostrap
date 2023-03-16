# WebSite - Installation


## Steps

  * Copy the `pages` and `media` directory to the `data` directory of Dokuwiki
  * Copy the [interwiki.local.conf](./interwiki.local.conf) file to the `conf` directory of Dokuwiki
  * Copy the `interwiki` icon [combo.png] to the `lib\images\interwiki`


## In a dev environment

Create Symlink

```cmd
mklink /D "D:\dokuwiki\website\theme" "D:\dokuwiki\website\theme"
```