# Strapi application

A quick description of your strapi application




# Upload to strapi to heroku

https://strapi.io/documentation/developer-docs/latest/setup-deployment-guides/deployment/hosting-guides/heroku.html


# heroku create
heroku create dj-events-backend1231423
heroku git:remote -a dj-events-backend1231423
heroku addons:create heroku-postgresql:hobby-dev --app dj-events-backend1231423
heroku config
npm i pg-connection-string pg
heroku config:set NODE_ENV=production
heroku config:set MY_HEROKU_URL=$(heroku info -s | grep web_url | cut -d= -f2)
git push heroku HEAD:main
heroku open




# My Url backend on heroku
https://djeventsbackend83457.herokuapp.com/


# Heroku logs
heroku logs
-- to se errors if uploading

# Push heroku 
git push heroku HEAD:main
heroku open


