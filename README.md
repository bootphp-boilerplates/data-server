# dataserver
A data Server with MYSQL and Mongo Backed for read.


## MAC

#### MONGO
```
$ brew update
$ brew install mongodb
$ mkdir -p /data/db
$ mongod --dbpath /data/db
```

#### OpenSSL install
```
$ brew install openssl
$ brew install wget

$ cd /usr/local/include 
$ ln -s ../opt/openssl/include/openssl .
// REFERENCE : https://github.com/mongodb/mongo-php-driver/issues/523
```

#### Install Driver
```
$ brew install autoconf
$ sudo /Applications/XAMPP/xamppfiles/bin/pecl install mongodb
$ sudo echo "extension=mongodb.so" >> /Applications/XAMPP/xamppfiles/etc/php.ini
//Restarted Apache
```

#### If apache not start
```
$ sudo /Applications/XAMPP/xamppfiles/bin/httpd -E /Applications/XAMPP/xamppfiles/logs/error_log -D SSL -D PHP
// REFER ISSUE : https://github.com/mongodb/mongo-php-driver/issues/247
```


