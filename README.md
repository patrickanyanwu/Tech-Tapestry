<h1 align="center">Tech Tapestry</h1>

<img src="https://github.com/user-attachments/assets/f652c670-ae8f-49e8-b141-2a078e88a0b2">

This blog posting site project was made to display my skills with frontend and backend programming to construct a full stack web application.
I used flask as the server for the site and css, bootstrap and javascript for the styling and responsivity of the website. This project was made as part of my completion of Angela Yu's Python Course <a href="https://www.udemy.com/certificate/UC-345341ce-5be6-432e-8b5b-2301eac2b023/">100 Days of Code</a>
<h3>Navigating the website</h3>

<p>Viewing and commenting on posts:</p>

https://github.com/user-attachments/assets/8fc0c637-bfd2-478c-8852-d9a2044a567b
<p>When authenticated the delete button for posts will appear beside the date the post was made and the create post button will appear above the older posts button:</p>
<img src="https://github.com/user-attachments/assets/47934fb5-7e59-4d64-a737-ddf002340ee8">


<h3>User Authentication</h3>

I used flask login authenticator to authenticate users, when a user registers their email and name is stored in the SQLite database and their password is hashed and salted using the werkzeug security package. When a user then wants to login using their username and password, the password is hashed and salted again then compared with the corresponding email's password in the database and if they match then the user is authenticated. Any user that is registered and logged in can then comment on posts. 

<h3>Database</h3>

I used SQLite as my database and SQLAlchemy to hanfle CRUD operations such as create tables, reading and writing, updating and deleting data, forms are used to read data that is input by users and this data is then read and written into the database. The html files then write the data from the database through flask, SQLAlchemy. Database relationships were used to keep track of what users made comments on posts, what users made posts and all comments that are made on a post, One to many relationships was used to do this.
