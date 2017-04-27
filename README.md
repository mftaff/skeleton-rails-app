# Skeleton rails-app

### This is the basic starter for all bloc projects

- Rails installed
- Basic landing page
- Basic config/gemfile settings
- Devise installed

This app should be compatible with any new Bloc.io project

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
