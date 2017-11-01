# Hebrew TL;DR Facebook Messenger Chatbot
To deploy new code you will need to install Heroku CLI [https://devcenter.heroku.com/articles/heroku-cli].
Clone repository, update the code and use deploy_code.bat script.
It will push the code to this repository, restart the web server and display a live log from the server, if the code is
buggy then all the issues will show on the log.

If you are running on a UNIX machine, you can deploy the server locally, cannot do that on Windows yet.



# Regarding Facebook Messenger Bot
This is a simple python template that uses Flask to build a webhook for Facebook's Messenger Bot API.

Read more in my [tutorial that uses this repository](https://blog.hartleybrody.com/fb-messenger-bot/).

*New:* [Check out my Facebook Messenger Bot Course](https://facebook-messenger-bot.teachable.com/p/facebook-messenger-bot/). It walks you through the process of getting this bot hosted on heroku step-by-step, and also unlocks all the content that's hidden in this repo's branches.

<<<<<<< HEAD
## "Callback verification failed" 
=======
## "Callback verification failed"
>>>>>>> fa6c337de72eabc188f09abf02b2be25f2b9d4a3

![Facebook Error](https://cloud.githubusercontent.com/assets/18402893/21538944/f96fcd1e-cdc7-11e6-83ee-a866190d9080.png)

The #1 error that gets reported in issues is that facebook returns an error message (like above) when trying to add the heroku endpoint to your facebook chat application.

Our flask application intentionally returns a 403 Forbidden error if the token that facebook sends doesn't match the token you set using the heroku configuration variables.

<<<<<<< HEAD
If you're getting this error, it likely means that you didn't set your heroku config values properly. Run `heroku config` from the command line within your application and verify that there's a key called `VERIFY_TOKEN` that has been set, and that it's set to the same value as what you've typed into the window on facebook.
=======
If you're getting this error, it likely means that you didn't set your heroku config values properly. Run `heroku config` from the command line within your application and verify that there's a key called `VERIFY_TOKEN` that has been set, and that it's set to the same value as what you've typed into the window on facebook.
>>>>>>> fa6c337de72eabc188f09abf02b2be25f2b9d4a3
