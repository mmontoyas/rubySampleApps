# rubySampleApps for Mac 10.10 OS X
TemplateApps.
Follow the Instructions: 

Ruby On the Rails Set-up:

https://gorails.com/setup/osx/10.10-yosemite

Demo : https://www.youtube.com/watch?v=J6r_l3cAS9s

MYSQL
=====
We've installed your MySQL database without a root password. To secure it run:
    mysql_secure_installation

To connect run:
    mysql -uroot

To have launchd start mysql at login:
  ln -sfv /usr/local/opt/mysql/*.plist ~/Library/LaunchAgents
Then to load mysql now:
  launchctl load ~/Library/LaunchAgents/homebrew.mxcl.mysql.plist
Or, if you don't want/need launchctl, you can just run:
  mysql.server start
==> Summary
🍺  /usr/local/Cellar/mysql/5.7.10: 12677 files, 465M


Note: If errors are related with mysql2 gem, probably missing:
sudo  bundle install or bundle install
POSTGRESS SQL
=============

If builds of PostgreSQL 9 are failing and you have version 8.x installed,
you may need to remove the previous version first. See:
  https://github.com/Homebrew/homebrew/issues/2510

To migrate existing data from a previous major version (pre-9.4) of PostgreSQL, see:
  https://www.postgresql.org/docs/9.4/static/upgrading.html

To have launchd start postgresql at login:
  ln -sfv /usr/local/opt/postgresql/*.plist ~/Library/LaunchAgents
Then to load postgresql now:
  launchctl load ~/Library/LaunchAgents/homebrew.mxcl.postgresql.plist
Or, if you don't want/need launchctl, you can just run:
  postgres -D /usr/local/var/postgres
==> Summary
🍺  /usr/local/Cellar/postgresql/9.4.5_2: 3021 files, 40M

