# HOSTING ON HEROKU GUIDES


# Before you can deploy your app to Heroku, initialize a local Git repository and commit your application code to it.

cd example-app
git init
Initialized empty Git repository in .git/
git add .
git commit -m "My first commit"


# Login to Heroku

heroku login


# Create a Heroku Remote

heroku create -a example-app


# You can use the git remote command to confirm that a remote named heroku has been set for your app

git remote -v

heroku  https://git.heroku.com/example-app.git (fetch)
heroku  https://git.heroku.com/example-app.git (push)


# For an Existing App

Add a remote to your local repository with the heroku git:remote command. All you need is your Heroku app’s name

heroku git:remote -a example-app

set git remote heroku to https://git.heroku.com/example-app.git


# Rename a Remote

By default, the Heroku CLI names all of the Heroku remotes it creates for your app heroku. You can rename your remotes with the git remote rename command. For example, rename heroku to heroku-staging

git remote rename heroku heroku-staging


# Deploy Your Code

git push heroku main
