## GIT
**Setup GIT**
1. setup .gitignore
1. `git init`
1. `git add .`
1. `git commit -m "Initial Commit"`
1. `git remote add origin {url_of rpro}`
1. `git push -u origin master`

**Setup GIT from existing project**
1. `git remote add origin {url_of rpro}`
1. `git pull {url_of rpro}`
1. `git branch --set-upstream-to=origin/master master`

**git commands**
- `git rm --cached` // remove item from git repository with out deleting
- `git commit`
- `git pull`
- `git status`

**git resources**
- https://github.com/github/gitignore // gitignorefiles

**global .gitignore**

Mac
- `touch ~/.gitignore_global` // Create file 
- `git config --global core.excludesfile ~/.gitignore_global` // Declare the global .gitignore 
- `vim .gitignore_global` // Open and add items as needed
  - .DS_Store
  - .DS_Store?
  - .idea
  - *~
  - log/
  - *.log
  - node_modules/

Windows
- [See this article](https://gist.github.com/subfuzion/db7f57fff2fb6998a16c)

## General Commands

**Folder and files**
- `mv * .[^.]* ../` // Move all files up a level
- `sed -i 's/original/new/g'` {filename} //Find and replace
- `rm -rf {directoryname}` //delete directory and all sub directories
- `mkdir` {filename} //make directory
- `vim {filename}` //open file to edit
- esc `:wq {filename}` //save and quit vim
- esc `:q {filename}` // quit vim

**SSH**
- Generate key `ssh-keygen`
- Copy public key `cat .ssh/id_rsa.pub`

**Project setup**

{php project with npn}
- `git clone`
- `npm install`
- `composer install`
- Create .env file at project root
- `npm run watch`
- `php artisan serve`

**Update project configuration**
- `php artisan optimize`
- `php artisan cache:clear`

## Other
**Server Updates**
1. `sudo apt-get update`
1. `sudo apt-get dist-upgrade`
1. `sudo reboot`
1. `sudo poweroff`

**Vagrant**
- `vagrant up`
- `vagrant provision`
- `vagrant ssh`

**Magento**
- `php shell/indexer.php --reindexall //reindexall in magento`

**Directory Listings**
/var/php-fpm // error logs on server
