Part I - Node Core Setup
# Update and Install node, npm, git and heroku
$ npm install -g n
$ sudo n latest
$ node -v
$ npm -v
$ express --version
$ git --version 
$ heroku --version
Part II - App Deploy
# App Deploy LOCALLY (https://expressjs.com/en/starter/generator.html)
$ express --view=ejs lastname-appname
$ cd lastname-appname
$ npm install
$ npm start
	# navigate to localhost:3000
$ git add .
$ git config user.name "github_username_here"
$ git config user.email "github_email_here"
$ git commit -m "message_here"
$ git push -u origin master


# App Deploy REMOTELY (https://devcenter.heroku.com/articles/getting-started-with-nodejs#set-up)
$ heroku login
$ heroku create lastname-appname
$ git push heroku master
$ heroku open
