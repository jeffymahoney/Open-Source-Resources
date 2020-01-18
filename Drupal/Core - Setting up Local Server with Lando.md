Lando sandbox for core work

Video: 
From Tandem
https://www.youtube.com/watch?v=jNAdsqQM3RA&feature=youtu.be


Setting up local for CORE contribution

```
cd ~
cd Sites/
git clone -b 8.8.x https://github.com/drupal/drupal.git d8core
cd d8core
lando init --recipe drupal8
```

From where should we get your app's codebase? `current working directory`


Where is your webroot relative to the init destination? `.`


What do you want to call this app? `d8core`


```
lando start
lando composer install
```

lando info (shows db creds amongst other things)

FOR NEW DB
DB_HOST=database
DB_USER=drupal8
DB_PASSWORD=drupal8
DB_NAME=drupal8
DB_PORT=3306

    "creds": {
      "user": "drupal8",
      "password": "drupal8",
      "database": "drupal8"
    },
    "internal_connection": {
      "host": "database",
      "port": 3306
      
      

TROUBLESHOOTING
https://docs.devwithlando.io/troubleshooting/logs.html