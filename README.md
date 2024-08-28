# Get_Youtube_Subscribers (AlmaBetter__Capstone__Project)
 
## Introduction

* A backend project which includes specific routes in the URL .
* User can  do the following as below:
    - *access the number of subscribers*, 
    - *access subscribers by specific IDs and names*, 
    - *add subscribers*, &
    - *delete subscibers*

## Used in this project:

* Mongoose
* Express
* MongoDB (Atlas and Compass)
* Raw data
* Path module to join index.html
* Postman || Insomnia
* nodemon
* dotenv

## Steps :

- *Step 1*

Install npm dependencies of express and mongoose using " npm install " command.

- *Step 2*

Using MongoDB local (Compass) as well as MongoDB Cloud (Atlas), depends on you which you want to use 
Just uncomment and comment the codes vice versa in createDatabase.js and index.js<br/>
* - **note** : To demonstrate I am using deployed project over the onRender<br/>
<br/>

Start the backend server using nodemon or node index.js command.

- *Step 3*

- GET http://localhost:3000/ → The client will see an interface of the site.<br/>


- GET http://localhost:3000/subscribers → When the user hit this, endpoint /subscribers, the client will get an array of all subscribers in JSON format from the database where the data is stored in local or MongoDB cloud database. <br/>


- GET http://localhost:3000/subscribers/names →When the user hit this, endpoint /subscribers/names the client will to get an array of all subscribers in JSON format with only name and subscribed Channel fields from the database, where the data is stored in local or MongoDB cloud database.<br/>


- GET http://localhost:3000/subscribers/:id → When the user hit this, endpoint /subscribers/:id in ID, the user needs to enter the USER’S ID which is stored in the database to get a particular user’s details like name, subscribed Channel and subscribed Date from the database, where the data is stored in local or MongoDB cloud database.<br/>


- GET http://localhost:3000/invalid → when the user hit the unwanted route which is not mentioned above (which is used to handle all other requests), they will get an error message like Route not found in JSON format with an 404 error status code.<br/>


app.use() is used to handle all the unwanted requests. It will return 404 Not Found status code indicating that the requested resource could not be found but may be available in the future.


## Deployment

*__Use Json Viewer extension in Browser for better view__*

 *__live link__* <br/>
 https://get-youtube-subscribers-z118.onrender.com

 


      

