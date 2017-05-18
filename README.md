# Skeleton rails-app

### This is the basic starter for all bloc projects

- Rails installed
- Basic landing page
- Basic config/gemfile settings
- Devise installed

This app should be compatible with any new Bloc.io project


---
### Setup cloud9 project
 
To pull this down into a new cloud9 project do the following:

First clone this repo into a new repo for your project.

Then create a new empty cloud9 project, (only the hidden file .c9 should exist)
in the console type:

```
git init
git remote add origin <https://github.com/mftaff/your-new-project.git> 
git pull -u origin master
bundle install
rake db:migrate
```
**Important!**
The first time you push up to github you need to add `-u` to the line: `git push -u origin master`

(To quickly launch the cloud9 localhost type: `ruby cloud9server.rb`) 


---
### Technical Details

In order to create environments.yml, you need to install the figaro gem: `figaro install`
confirm that this command creates a new `environments.yml` file, and appends it to `.gitignore`
(see `environments_placeholder.yml` for an idea of how the file should look)

To configure heroku run:
```
heroku login
heroku create <name-optional>
git push heroku master
```
After running this, add send-grid to your heroku app, and use the provided user_name/password as your environment variables in `environments.yml`
