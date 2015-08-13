  1. [![Deploy](https://www.herokucdn.com/deploy/button.png)](https://heroku.com/deploy)
  1. Run ```heroku addons:open postmark -a app-name```
  1. Select inbound mail from the webpage opened in the previous step
  1. Enter ```https://yourapp.herokuapp.com/hooks/postmark``` for the webhook URL
  1. Send an email to the address provided by Postmark
  1. Optionally, create an email rule to forward messages from anouther account to the Postmark address


You can always retrieve the email address to submit issue to by running

    heroku config:get POSTMARK_INBOUND_ADDRESS

It can also be helpful to create an easy to remember email address that forwards to the POSTMARK_INBOUND_ADDRESS.
