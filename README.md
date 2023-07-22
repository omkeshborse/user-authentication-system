# user-authentication-system
user authentication system 

Tools use 
frontend : react , react-router-dom , Axios , 
back end : node js , express , nodemon ,cros , email-validator , bcyrpt , cookie -parser  , dotenv ,mongoose 

 install process : 
 
	 git clone git@github.com:omkeshborse/user-authentication-system.git 

 cd user-authentication-system 
	cd backend 
	npm  install 
 
 cd client 
	npm install 
	note : after installing  node modules in both frontend and backend need  to create   .env file as follow  : 

	in backend folder  : 
create  .env   file  
then add in .env  : 

PORT=8081
MONGODB_URL= mogoDB connection String (without quoted ) / mongodb atlas connetion string 
SECRET=SECRET
CLIENT_URL = http://localhost:3000

in frontend folder : 
create  .env   file  
then add in .env  : 

REACT_APP_URL = http://localhost:8081


















