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
[Reference](https://stackoverflow.com/questions/30204938/how-to-install-php-mongodb-driver-for-xampp-on-osx)

#### OpenSSL install
```
$ brew install openssl
$ brew install wget

$ cd /usr/local/include 
$ ln -s ../opt/openssl/include/openssl .
```
[Reference](https://github.com/mongodb/mongo-php-driver/issues/523)

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
```
[Reference](https://github.com/mongodb/mongo-php-driver/issues/247)


