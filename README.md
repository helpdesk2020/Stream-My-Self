# heroku general guide for future refrence 
1- change the port to: process.env.PORT
2- create Procfile with: web: node index.js
3- make sure in package json the npm start command points to "node index.js" 
4- if you have requests from front end use the root path
5- make sure code runs locally
6 - deploy using the following comands

git remote -v 
git remote rm heroku 
heroku create 
git push heroku master 
heroku ps:scale web=1 
heroku open 
heroku logs --tail 
heroku run bash
