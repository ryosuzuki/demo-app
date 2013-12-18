# Instalation

This is Cumiki Demo App for http://cumiki.com/demo

```
git clone git@github.com:cumiki/demo-app.git

cd demo-app

bundle install

rake db:migrate
```

Then you can run server

```
rails s
```

# Setup Twitter Developer

To use Twitter API, please set up `ENV['TWITTER_KEY']` and `ENV['TWITTER_SECRET']`

```
cp config/application.yml.example config/application.yml
```

Then, modify your onw key and secret. You can get key and secret in https://dev.twitter.com

```
TWITTER_KEY: YOUR_TWITTER_KEY
TWITTER_SECRET: YOUR_TWITTER_SECRET
```

If you run in your local, don't forget to set *Twitter Developer Callback* setting to `http://0.0.0.0:3000/auth/twitter/callback`.