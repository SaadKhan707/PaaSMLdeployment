Refer youtube video- https://youtu.be/OBGaCULCZzg?si=Gtun03udIpgl1fYE
		     https://youtu.be/mrExsjcvF4o?si=vBQ5jLY-GfvBjfHO

Before implementation on public url, test the model on localhost (personal pc)
--> open anaconda prompt- navigate to the folder where the files files are kept "cd <path>"
--> run- python app.py (copy the url and paste it on browser and see if the model is working properly)

1- Create all the files- app.py (flask code) , model pickle, index.html, 
requirements.txt (will contain all the required packages to be installed before implementation of model).
2- Create a repo on github and upload all the above files.
3- open render.com (PaaS/ platform as a service) - Go to web services --> create a new project --> link your github repo
--> while configuring the connectivity command must be "gunicorn app:app" :- "app" on LHS is the flask file code and on RHS "app" is the
flask instance initiated with command "app = Flask(__name__)" inside the code.
Note: Under env variable select the varibale name: PYTHON_VERSION and value: 3.7.10 -- to avoid any issues with compatibility
--> Click on deploy button and everything will be done on its own (check terminal to view logs)
4- Once build successfully deployed --> we can see the live button highlighted in green and a link will be avaliable on top.
Use this link and open on a browser, input the data and get predicted salary.