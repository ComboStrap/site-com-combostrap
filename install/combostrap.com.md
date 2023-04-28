# Server


## Symlinks

```bash
FQDN=combostrap.com
ln -s /opt/www/git/${FQDN}/pages /opt/www/bytle/farmer-animals/${FQDN}/data/pages
ln -s /opt/www/git/${FQDN}/media /opt/www/bytle/farmer-animals/${FQDN}/data/media
mkdir -p /opt/www/bytle/farmer-animals/${FQDN}/data/combo/theme/
ln -s /opt/www/git/${FQDN}/theme /opt/www/bytle/farmer-animals/${FQDN}/data/combo/theme/combo
```

## Configuration

Installation if changed in the repo
```
mv /opt/www/bytle/farmer-animals/${FQDN}/conf/local.php-$(date -u +"%Y-%m-%d.%H:%M")
ln -s /opt/www/git/${FQDN}/conf/${FQDN}/local.php /opt/www/bytle/farmer-animals/${FQDN}/conf/local.php
```

After each update on the server. Configuration is overwritten. After every configuration change
```
cp /opt/www/bytle/farmer-animals/${FQDN}/conf/local.php  /opt/www/git/${FQDN}/conf/${FQDN}/local.php
```
