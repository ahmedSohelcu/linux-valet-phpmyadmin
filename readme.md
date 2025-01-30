
### This Documentation's main purpose is to make easy a laravel developer's daily life.
####

# Index

> 1. Install Valet in fresh linux machine
####
> 
> 2. Install mysql, create root user and set privileges
####

> 3. Install PHP, composer, php extension, phpmyadmin as database tools
####

> 4. Add valet path dynamically
####

> 5. Generate and add Github ssh key for linux
####

> 6. Valet command list
####

> 7. Add alias in linux machine to create a command short
####

> 8. Install vim, vim  plugin and vim shortcut
####

> 9. Linux important command
####


> 10. Laravel scripts install or update for codecanyone
####

--------------------------------
vs code plugin 
--------------------------------
####  IntelliJ IDEA Keybindings – for phpstorm keybinding


---------------------------
 Valet setup
---------------------------
Install composer
------------------- 
```
1.sudo apt update
```
```
2.sudo apt install php-cli unzip
```
```
sudo apt install curl
```
```
php composer.phar global require friendsofphp/php-cs-fixer
```

```
sudo apt install composer
```

-------------------------------------------------
install valet 
-------------------------------------------------
```composer global require cpriego/valet-linux -W```

---------------------------
Add valet path dynamically
---------------------------
``` 
echo "export PATH=$PATH:$HOME/.config/composer/vendor/bin" >> ~/.zshrc
source ~/.zshrc 
```

---------------------------
valet dependency
---------------------------
```sudo apt-get install network-manager libnss3-tools jq xsel```

---------------------------
3.Install php extension
---------------------------
```
sudo apt install openssl php-bcmath php-curl php-json php-mbstring php-mysql php-tokenizer php-xml php-zip
```

---------------------------
valet command
---------------------------
```
Valet install

Valet park

Valet run

Valet restart

Valet stop

Valet start

sudo service apache2 stop -- t stop apache2 in create conflict with valet
```



https://cpriego.github.io/valet-linux/

https://cpriego.github.io/valet-linux/
https://www.digitalocean.com/community/tutorials/how-to-install-and-use-composer-on-ubuntu-20-04


---------------------------
Generate ssh key linux
---------------------------
```ssh-keygen -t rsa```
Go to -> home/ahmed/.ssh/id_rsa
Copy code-> and set in github

---------------------------
Copy the SSH public key to your clipboard. ...
---------------------------
```
In the upper-right corner of any page on GitHub, click your profile photo, then click Settings.
In the "Access" section of the sidebar, click SSH and GPG keys.
Click New SSH key or Add SSH key.
```


---------------------------
Phpmyadmin for valet
---------------------------
Download phpmyadmin (https://www.phpmyadmin.net/donate/)
Extract and copy to project directory

---------------------------
Install mysql client and server
---------------------------
```
sudo apt-get install mysql-client
```
```
sudo apt-get install mysql-server
```

---------------------------
Create root user and password
And set previledge
---------------------------
```
sudo mysql -u root -p
```

---------------------------
create user and password
---------------------------
```CREATE USER 'username'@'localhost' IDENTIFIED BY 'password';```

---------------------------
Give previleges
---------------------------

```GRANT ALL PRIVILEGES ON *.* TO 'username'@'localhost';```

---------------------------
flush previleges
---------------------------
```
FLUSH PRIVILEGES;
```

--------------------------------
Create Alias for a command to make short
--------------------------------

Open bashrc file to add alias

```
nano ~/.bashrc
```

Add Alias like and finally save and restart the terminal to get changes.
```
alias pa='php artisan'
alias pam='php artisan migrate'
alias pads='php artisan db:seed'
alias pakg='php artisan key:generate'
alias paoc='php artisan optimize:clear'
```

# Vim

--------------------------------
Install vim 
--------------------------------
#####
```json
sudo apt-get install vim
```

### Create .vimrc File to Install Plugin
```json
    vim ~/.vimrc
```

#### Add some plugin in .vimrc file

```
set number

set relativenumber

set tabstop=4

set shiftwidth=4

set autoindent

set mouse=a

set colorscheme slate (to change terminal color like state / delek etc)
```

---------------------------
valet dependency
---------------------------
```sudo apt-get install network-manager libnss3-tools jq xsel```

---------------------------
3.Install php extension
---------------------------
```
sudo apt install openssl php-bcmath php-curl php-json php-mbstring php-mysql php-tokenizer php-xml php-zip
```

---------------------------
Linux important command
---------------------------
```
LS - Lists files and directories in the current directory.
```
```
MV - Moves or renames files and directories.
```
```
SSH - Connects to a remote machine using SSH protocol.
```
```
CD - Changes the current directory.
```
```
CAT - Concatenates and displays file content.
```
```
SUDO - Executes a command with root/admin privileges.
```
```
PWD - Prints the current working directory.
```
```
GREP - Searches for a specified pattern in files.
```
```
TOP - Displays system resource usage and running processes.
```
```
MKDIR - Creates a new directory.
```
```
FIND - Searches for files and directories.
```
```
WGET - Downloads files from the web.
```
```
RM - Removes files and directories.
```
```
CHMOD - Changes the permissions of files and directories.
```

```
TAR - Archives files and directories into a single file.
```
```
CP - Copies files and directories.
```
```
CHOWN - Changes the ownership of files.
```
```
GZIP - Compresses files using the gzip algorithm.
```



---------------------------------------------------
Laravel scripts install or update for codecanyone 
--------------------------------------------------
```
	Main logic is initially commented all except setup route from
	RouteServiceprovider and load setup / update file from RouteServiceProvider
	and finally copy RouteServiecProvider from setupServiceProvider(all route will open for project and commented route for   setup and update)
```



	



