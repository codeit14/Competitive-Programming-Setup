# Twitter Clone
# Project Setup
The project backend has been implmented using Django-Rest-Framework and database used is RDBMS (MySQL). The code has been properly tested, and written in a generic manner.
Steps to setup the project on your machine- 
> 1) Create a virtual environment using command - 
        virtualenv venv -p python3
> 2) Activate virtual environment using command - 
        source venv/bin/activate
> 2) Install requirements using command -
        pip install -r requirements.txt
> 3) Now make migrations of project using command - 
        python manage.py makemigrations && python manage.py migrate
> 4) Run Django server using command - 
        python manage.py runserver                   
All ready to go !
# List of APIs and their functionalities- 

# Dataset Used
The dataset we have used for our music genre classification is GTZAN[]. This dataset contains 1000 song files, each of which is 30 seconds long. These songs are classified into 8 genres, namely, blues, classical, country, disco, hip-hop, jazz, metal and pop respectively. The sampling rate we have used for our data files is 22050 Hz. All these files were in .au format which were converted to .wav using online converter. This is done since .wav format files are easily read by python modules.  We divided our dataset into training and testing data in the ratio 7.5 : 2.5. Spectogram of songs of different genres are depicted. 
The dataset is available at this link : [marsyasweb.appspot.com/download/data_sets/](marsyasweb.appspot.com/download/data_sets/)

We have uploaded a small video explanation of our machine learning code as well as the flask API along with the research papers referred and the research paper we are still working on this link - [https://drive.google.com/open?id=1oAtUAaVEIwL_rsgMMQ_lYtfMLpl-oPXr](https://drive.google.com/open?id=1oAtUAaVEIwL_rsgMMQ_lYtfMLpl-oPXr)
