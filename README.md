# Salesforce Switch
Salesforce.com application to enable and disable validation rules, workflows and Apex triggers

## Details
This application runs on Django and is designed to run on Heroku, but could run on any server with some changes

## Installation
- Deploy code to a Heroku instance
- Install a Heroku database and a Redis add-on
- Create a Connected App in Salesforce
- Set up environment variables in Heroku for the Connected App settings:
    - SALESFORCE_CONSUMER_KEY = your Salesforce consumer key from the connected app
    - SALESFORCE_CONSUMER_SECRET - your Salesforce consumer secret
    - SALESFORCE_REDIRECT_URI - set to the URL of your app + '/oauth_response'
    - SALESFORCE_API_VERSION - current WSDL is setup to use 34
- Run `heroku run python manage.py syncdb`
