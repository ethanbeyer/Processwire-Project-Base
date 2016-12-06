# Some Dependencies
1. [Virtualbox](https://www.virtualbox.org)
2. [Vagrant](https://www.vagrantup.com/downloads.html)
3. [Ghost](https://github.com/bjeanes/ghost)


# Startup
1. Edit `SITENAME` and `XXX.XXX` in `./Vagrantfile`
2. From within the project, run `$ vagrant up`
3. After running `$ vagrant up`, a command to add the site's IP to your hostfile will be printed. Copy/Paste that into the terminal to add the box's IP to your Hostfile.


# Packages
1. Run `$ vagrant ssh`. After that logs in to the box...
  - run `$ cd /var/www/public`
  - then `$ composer update`
  - then `$ logout`
2. Run `$ yarn install` to install all NPM packages.


# Install ProcessWire
1. Navigate to the `http://your-sitename` in your browser, and follow instructions to install PW.
  - DBNAME: scotchbox
  - DBUSER: root
  - DBPASS: root


# Lastly...
1. Run `$ gulp` from within the project
2. Log in to ProcessWire at `http://your-sitename/admin`
3. Click on "Refresh" under *Modules*
