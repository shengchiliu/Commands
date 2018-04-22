# Basic Heroku Commands

```sh
# Log in Heroku account
$ heroku login              # Enter your Heroku credentials.

# Clone Heroku App
$ https://git.heroku.com/YOUR-APP-NAME.git

# Create an app on Heroku
$ heroku create

# Deploy your code
git push heroku master

# Ensure that at least one instance of the app is running
$ heroku open

# View logs
$ heroku logs --tail        # Control+C to stop streaming the logs

# Visit the app at the URL
$ heroku open

# Define a Procfile
$ echo "web: gunicorn gettingstarted.wsgi --log-file -" >> Procfile     # Procfile file in the root directory of your application

# Scale the app
$ heroku ps
$ heroku ps:scale web=0
$ heroku ps:scale web=1
```
