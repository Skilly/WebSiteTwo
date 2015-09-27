Welcome to WebSiteTwo!
===================
For considering AgileVentures Future Directions

Ronin final project to implement an AgileVentures showcase

---

Getting the app up and running
---

> **Optional** (if you haven't yet added an ssh key to github)

> - Generate a public\private key on your local Linux box

>            $ ssh-keygen -t rsa -b 4096 -f ~/.ssh/id_rsa_github
> - Add the key to ssh-agent on your local linux box

>          $ ssh-add ~/.ssh/id_rsa_github
> - login to github
> - view profile
> - choose ssh keys
> - add new
> - copy contents of ~/.ssh/id_rsa_github.pub to dialogue box

1. Fork https://github.com/AgileVentures/WebSiteTwo on github
1. create an "agileventures" folder where you keep your rails projects and cd into it
1. $ git clone git@github.com:UserName/WebSiteTwo.git
1. Logon to postgres using PGAdminIII and create user "" (not superuser but "can create databases"), with password
1. edit config/database.yml file to amend config settings for postgres db (password, host, port)
1.  rem bundle install
1. $ export RAILS_ENV=development
1. $ export RACK_ENV=development
1. $ rake db:create
1. $ rake db:migrate
1. $ rails server
