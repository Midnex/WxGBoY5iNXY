# Title: Creating a RESTFul API in Flask With JSON Web Token Authentication and 
Flask-SQLAlchemy
# Date: Jun 23rd, 2017
# Author: PrettyPrinted
# Youtube: WxGBoY5iNXY&t

I am not the author, only the code I am typed while learning the project. There 
are some notable changes in my code versus that of PrettyPrinted

# Changes
* Added a requirements.txt file, you can use this to setup a virtual environment 
that works with the original video.
* changed database location to sqlite:///todo.db as this will work for others 
who are not running WSL and whose usernames are different.
* Cleaned up some repeating code, by changing the login route to use a standard 
message for all login required messages.
* Added a check if username is already taken in create_user route. As this is a 
must for all user creation.
* Cleaned up formatting of code to be more consistent

# Requirements:
Flask==2.0.1
Flask-SQLAlchemy==2.5.1
PyJWT==1.7.1

# Setup
python -m venv venv
source venv/bin/Activate (Linux)
source venv/Scripts/Activate (Windows)
python -m pip install -r requirements.txt