1. fork https://github.com/AgileVentures/WebSiteTwo on github
2. $ ssh-keygen -t rsa -b 4096 -f ~/.ssh/id_rsa_github
3. $ ssh-add ~/.ssh/id_rsa_github
4. logon to github, view profile, ssh keys, add new, copy contents of ~/.ssh/id_rsa_github.pub to dialogue box
5. create an "agileventures" folder where you keep your rails projects and cd into it
6. $ git clone git@github.com:UserName/WebSiteTwo.git
7. Logon to postgres using PGAdminIII and create user "" (not superuser but "can create databases"), with password
8. edit config/database.yml file to amend config settings for postgres db (password, host, port)
9.  rem bundle install
10. $ export RAILS_ENV=development
11. $ export RACK_ENV=development
12. $ rake db:create
13. $ rake db:migrate
14. $ rails server
