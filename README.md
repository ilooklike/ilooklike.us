# ilooklike.us

Web App for ilooklike.us

A location-based story sharing application that will encourage community-building.

## Getting up and running

### With rvm

1. Install postgresql
2. Install [ruby version manager](https://rvm.io/rvm/install)
3. Clone project repository

  ```
  git clone git@github.com:ilooklike/ilooklike.us.git
  ```

4. Switch to repository folder

  ```
  cd /path/to/application
  ```

5. Install required ruby version. Right now it's `2.2.3`, but it might be changed soon. So you find relevant verion in `.ruby-version` file

  ```
  rvm install 2.2.3
  ```

6. Install [bundler](http://bundler.io/) - ruby packege manager

  ```
  gem install bundler
  ```

7. Install all gems with bundler

  ```
  bundle install
  ```

8. Create database config file from template

  ```
  cp config/database.yml.example config/database.yml
  ```

9. Fill database.yml with creadentials for your local db. It might require you to configure postgresql first
10. Create project database with rake

  ```
  bundle exec rake db:create
  ```

11. Run server

  ```
  rails s
  ```

The end! Now you can access application with [localhost:3000](http://localhost:3000) in your browser
