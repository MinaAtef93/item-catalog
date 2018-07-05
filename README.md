about
-----
The Item Catalog project consists of developing an application that provides a list of items within a variety of categories, as well as provide a user registration and authentication system.

 RESTful web application utilizing the Flask framework which accesses a SQL database that populates restaurants and their menuitems. OAuth2 provides authentication for further CRUD functionality on the application. Currently OAuth2 is implemented for Google Accounts.



OAuth2.0
---------
Visit: http://console.developers.google.com for google setup

To get the Google login working there are a few additional steps:

1-Go to Google Dev Console
2-Sign up or Login if prompted
3-Go to Credentials
4-Select Create Crendentials > OAuth Client ID
5-Select Web application
6-Enter name 'web'
7-Authorized JavaScript origins = 'http://localhost:5000'
8-Authorized redirect URIs = 'http://localhost:5000/login' && 'http://localhost:5000/gconnect'
9-Select Create
10-Copy the Client ID and paste it into the data-client-id in login.html
12-On the Dev Console Select Download JSON
13-Rename JSON file to client_secrets.json
14-Place JSON file in folder build-item


JSON
---- 


1-get all  restaurants:localhost:5000/restaurant/JSON 

2-get specfic restaurant menus : localhost:5000/restaurant/<int:restaurant_id>/menu/JSON

3-get specfic menu:localhost:5000/restaurant/<int:restaurant_id>/menu/<int:menu_id>/JSON

Developing
--------
FrontEnd: 
html/css/jquery/json

Backend:
framework flask usning python version 2 and sql 



Install
-------
1-install vagrant and virtual box

2-open git bash terminal if u use windowes os 



3- load vagrant and authenticate it by using vagrant up and vagrant ssh

4- go to project folder

5- run  database_setup.py  follow this command:
	$ python database_setup.py
 
6- then lotsofmenus.py follow this command:
	$ python lotsofmenus.py
	
after step 5 and 6 u will see restaurant.db appear in folder 

7- finally run  main.py follow this command:
	$ python main.py

8- go to this link after run main.py localhost:5000

9- go to  login page by click button login or follow this link localhost:5000/login\

10- hover the restruant and click on it to see menu








License
--------


CopyRight By mina atef 



