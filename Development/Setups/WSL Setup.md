# Initial Installations
## Update APT
```
sudo apt update && sudo apt-get full-upgrade
```

## Install PHP
```
sudo apt-get install -y php php-cli php-common php-fpm php-mysql php-zip php-gd php-mbstring php-curl php-xml php-bcmath openssl php-json php-tokenizer
```

## Setup Github
**profile**
```
git config --global user.name 'Javl1n'
git config --global user.email 'farmodia@gmail.com'
```
**ssh key**
```
ssh-keygen -t ed25519 -C "Javl1n@pc"
cat ~/.ssh/id_ed25519.pub
```

## Install Composer
**Initial install**
```
php -r "copy('https://getcomposer.org/installer', 'composer-setup.php');"
php -r "if (hash_file('sha384', 'composer-setup.php') === 'dac665fdc30fdd8ec78b38b9800061b4150413ff2e3b6f88543c636f7cd84f6db9189d43a81e5503cda447da73c7e5b6') { echo 'Installer verified'.PHP_EOL; } else { echo 'Installer corrupt'.PHP_EOL; unlink('composer-setup.php'); exit(1); }"
php composer-setup.php
php -r "unlink('composer-setup.php');"
```
**Move to global**
```
sudo mv composer.phar /usr/local/bin/composer
```

## Install Node
**install node**
```
sudo apt install nodejs
```
**install npm**
```
sudo apt install npm
```

## Install MySQL
```
sudo apt install mysql-server
```

## Initialize Laravel Project
**clone repository**
```
git clone https://github.com/organization/project.git project-directory
```
**install composer dependencies**
```
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

## WSL Networking
link: https://www.youtube.com/watch?v=yCK3easuYm4
**On powershell**
```
netsh interface portproxy add v4tov4 listenport=5173 listenaddress=0.0.0.0 connectport=5173 connectaddress=172.29.106.143
```