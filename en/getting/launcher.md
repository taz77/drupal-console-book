# Install Drupal Console Launcher using the phar

```
curl https://drupalconsole.com/installer -L -o drupal.phar
mv drupal.phar /usr/local/bin/drupal
chmod +x /usr/local/bin/drupal
```
NOTE: If you don't have curl you can try
```
php -r "readfile('https://drupalconsole.com/installer');" > drupal.phar
```

## Update DrupalConsole Launcher 
```
drupal self-update
```

## Run Drupal Console using the Launcher
```
drupal
```

## Installing the Launcher using Composer 
Set Composer global `minimum-stability` and `prefer-stable` configurations.
```
composer global config minimum-stability dev
composer global config prefer-stable true
```
```
composer global require drupal/console-launcher:~1.0
```

You must execute the launcher within a drupal site directory or use `--root=/path/to/drupal8.dev
` to specify your drupal site path.

**NOTE:** The name `drupal` is just an alias you can name it anything you like.
