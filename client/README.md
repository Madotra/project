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
