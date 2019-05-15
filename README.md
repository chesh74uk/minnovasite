
POSTGRESQL
sudo apt-get update
sudo apt-get install postgresql postgresql-contrib
sudo service postgresql start
sudo apt-get install libpq-dev
sudo -u postgres createuser -s ubuntu
sudo -u postgres createdb ubuntu

RUBY
rvm install 2.5.3
gem install rails -v 5.2.2
rvm --default use 2.5.3
rails new minnova -d=postgresql


GEMS
https://github.com/comfy/comfortable-mexican-sofa

HEROKU
sudo snap install --classic heroku
heroku config:set AWS_ACCESS_KEY_ID=xxx AWS_SECRET_ACCESS_KEY=yyy
heroku login
heroku create mwaw --region eu
git push heroku master
heroku run rails db:migrate