# ci-me-dice-on-demand
[![Build Status](https://app.travis-ci.com/santiagovj22/ci-me-dice-on-demand.svg?branch=main)](https://app.travis-ci.com/santiagovj22/ci-me-dice-on-demand)

Sample Python app for learning CI. You will get a flexible dice on demand! 

This application is written in Python and uses Flask as the web framework. It serves a single HTML page.  
Gunicorn is used for the production server.  
Continous Integration is managed using Travis-CI  
Continous Deployment is managed using Heroku  

# :page_with_curl: Instructions
1. Clone this repo
2. Navigate to the directory
3. Execute this:
```
# This will create and activate a virtualenv. Using a virtual environment allows you to manage your project’s dependencies without messing with system-level files shared by all applications.
python3 -m venv venv

source venv/bin/activate

# Install dependencies
pip install -r requirements.txt

# or if you're still using python 2
pip3 install -r requirements.txt
```

Now that all dependencies are installed, we can run the program!

4. To test the app:
```
python3 -m pytest -v tests/test_dice.py
```
5. To run the app:
```
flask run
```

6. Go to the URL provided by the app (i.e. `http://localhost:5000`)

# Usage

1. First off, enter the number of sides of your dice. (Some games might require you to use 20-sided dice)
2. Now, click on the `roll` button!
3. You should see a message on the screen - "You Rolled a ..."
4. That's it!
