heroku-node
===========


How to creat simply node.js app in 10 minutes and skip ssh problem on Windows 7 :D



Create directory 

mkdir heroku
npm init
npm install express --save

Edit files

subl app.js
mkdir public
subl index.html



Create repository

git init
git status
echo "node_modules" > .gitignore
git add .
git commit -m "my new static site"

Create proc file

echo "web: node app.js" > Procfile
git add . 
git commit -m "proc file"

Create heroku app

heroku create hs-static
get push heroku master


SSH problem in Windows Solution :D

Download msysGit and instal it on C:\
The in Git bash generate ssh by:

ssh-keygen -t rsa

Then copy this key to ssh keys on accoutn in heroku and then copyfiles from
username/.ssh folder do C:\msysGit and in cmd bash hit command

get push heroku master

you apps in on name-app.heroku.com  RUNNING

Thats it folks !!!


