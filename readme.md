## Client Folder Proceedings

My whole Project have 7 features

1. Navigation bar with SignIn/SignUp button.
2. Account  verification.
3. Creating new travel post.
4. Editing the existing post.(but the user can only edit their own post which is achieved by Adding the post creator variable in the post storage in database)
5. Deletion of post. (user can only delete their own post which is also achieved by the account verification and the post creator verification).
6. Liking the travel post.(one post can be liked by one user only one time.) 
7. Handling of the token expiry. User authorization token will expire in one hour and after that the user will be logged out automatically.



### First we create a react application with the command in the client folder:

***
npx create-react-app ./
***

this command is placed in the client folder in the project document.
As this project will have two section first we will have work on client section to create a layout of the home page.


Since my project is in a different  folder  iam just installing all the dependencies all at once using the code
***
npm install
***

## but there are 2 dependencies which i have to install forcefully using the code 

***
npm install @material-ui/icons --force
***
npm install @material-ui/styles --force
***

I am using the material-ui components as it don't take more  modification to modify the looks of the page.

## i am using the jwt token for the Authorization of the user. To get the token I need to decrypt the token for that I'm using the jwt-decode which was installed using the command

***
npm install jwt-decode
***

## To process the authorization we need to use a middleware and to use the middleware we need to use the reactor dom which is installed using the command

***
npm install react-router-dom
***




## This is The server Section

### First we create a react application with the command in the server folder:

***
npm init -y
***

this command is placed in the server folder in the project document.
As this project will have two section first we will have work on server section to create the backbone of the project.

Since my project is in a different  folder  iam just installing all the dependencies all at once using the code
***
npm install
***

I will be following the  functionality of the routes and controllers and modules as it was the best way i understood. rest was too complex for me understand.

We are using quit a few dependencies
1. cors
2. dotenv
3. express
4. mongoose
5. nodemon


### Now we will do the nex process of Authentication

To Add the functionality of Authentication we need to install two dependencies

1. bcrypts
2. jsonwebtoken

to install this Dependencies we will run the command

***
 npm install bcryptjs jsonwebtoken
***

 To  accommodate the feature of authorization We are using the method of router Dom Where we will be using the middleware to create the authorization.Account verification is done for creating the new post along with editing and deleting which can only be done by verifying the account jsonwebtoken.
