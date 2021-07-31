Criminal Recognition

1. clone this repository

$ git clone https://github.com/kumarkaushal920/FRSASS.git


2. Install virtualenv.

$ pip install virtualenv


3. create virtual environment.

$ virtualenv venv


4. activate environment.

$ . venv/Scripts/activate


5. install requirements.

$ pip install -r requirements.txt


6. modify the database in the settings.py which is this part

DATABASES = 
            { 'default': 
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

7. Open XAMPP control panel > start Apache and MySQL 

8. Goto Chrome type localhost > goto phpMyadmin >Create a database with the name of your choice

9. import the sql crime_identify.sql from the root folder for the project you cloned

#you can also run a python migrate if you do not want the data populated in my database

10. Run the server. 

$ python manage.py runserver [7000]