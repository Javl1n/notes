# Initial Setup after cloning
## without sail
**install composer dependencies**
```
composer update
composer install
```
**install NPM dependencies**
```
npm install
```
**copy .env file**
```
cp .env.example .env
```
**generate app encryption key**
```
php artisan key:generate
```
**migrate database**
```
php artisan migrate
```
**install reverb**
```
php artisan reverb:install
```

## with sail
**install composer dependencies**
```
composer install
```
**copy .env file**
```
cp .env.example .env
```
**install sail**
```
php artisan sail:install
```
**sail up**
```
sail up -d
```
**generate app encryption key**
```
sail artisan key:generate
```
**migrate database**
```
sail artisan migrate
```
**install NPM dependencies**
```
sail npm install
```

### optional installation
**install broadcasting**
```
sail artisan install:broadcasting
```
**expose**
```
sail share --subdomain [subdomain]
```
