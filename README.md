# heroku_test
To run this app in local environment , run `./setup.sh`

To run this application in Heroku
1. Create an app in Heroku
`heroku create name_of_your_app`
2. Obtain Heroku git url 
`git remote add heroku heroku_git_url`
3. Create a database in Heroku
`heroku addons:create heroku-postgresql:hobby-dev --app name_of_your_application`
4. Add the env variables in `setup.sh` in Heroku env configs in Heroku dashboard
5. Push the code to heroku git 
`git push heroku master`
6. run the db migrations
`heroku run python manage.py db upgrade --app name_of_your_application`
