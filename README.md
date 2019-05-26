# Twitter Clone
# Project Setup
The project backend has been implmented using Django-Rest-Framework and database used is RDBMS (MySQL). The code has been properly tested, and written in a generic manner.
Steps to setup the project on your machine- 
1) Create a virtual environment using command - 
>         virtualenv venv -p python3
2) Activate virtual environment using command - 
>         source venv/bin/activate
3) Install requirements using command -
>         pip install -r requirements.txt
4) Now make migrations of project using command - 
>         python manage.py makemigrations && python manage.py migrate
5) Run Django server using command - 
>         python manage.py runserver                   
All ready to go !

# List of APIs and their functionalities
API | Request Body | Method | Description | Response
|---|---|---|---|---|
| [/rest_auth/signup/] | (first_name, last_name, username, password, email, contact_number(in +91 format), country_code) | POST | User Sign up  | Authentication Token
| [/rest_auth/login/] | (username, password) | POST | User Login | Authentication Token
| [/rest_auth/logout/] | No | GET | Logout User | No
| [/tweets/tweet/] | (attachments[Multiple], description) | POST | Post tweet with attachments | Tweet
| [/tweets/tweet/[Tweet_id]/] | No | GET | Retrieve Tweet Info | Tweet
| [/tweets/tweet/[Tweet_id]/] | No | DELETE | Delete Tweet | No
| [/tweets/tweet/user/[User_id]/] | No | GET | Get list of user's tweets | [Tweets]
| [/tweets/attachment/[Attachment_id]/] | No | GET | Get attachment details | Attachment
| [/tweets/follow/[User_id]/] | (is_follow) | PUT | Follow/Unfollow a User | No
| [/tweets/tweet/like/[Tweet_id]/] | (is_like) | PUT | Like/Unlike a Tweet | No
| [/rest_auth/user/[User_id]/] | No | GET | Get user's details | User
| [/tweets/tweet/retweet/[Tweet_id]/] | (comment) | POST | Retweet a tweet | No
| [/tweets/tweet/retweet/user/[User_id]/] | No | GET | Get user's retweets | [Retweets]
