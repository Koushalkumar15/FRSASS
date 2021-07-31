Criminal Recognition

# clone this repository
$ git clone https://github.com/kumarkaushal920/FRSASS.git

#do a pip install
$ pip install virtualenv

# create virtual environment
$ virtualenv [name of your new virtual environment]

## activate environment.
$ . envName/Scripts/activate

## install requirements.
pip install -r requirements.txt

## setup db.
#modify the database in the settings.py which is this part 
DATABASES = { 'default': 
                { 
                    'NAME': 'crime_identify',
                    'ENGINE': 'mysql.connector.django',
                    'USER': 'root', 
                    'PASSWORD': 'koushal',
                    'HOST' : '127.0.0.1', 
                    'PORT': '3306',
                    'OPTIONS': { 'autocommit': True, },
                }
            }

#create a database with the name of your choice

#import the sql crime_identify.sql in the root folder for the project you cloned

#you can also run a python migrate if you do not want the data populated in my database

python manage.py runserver [7000]