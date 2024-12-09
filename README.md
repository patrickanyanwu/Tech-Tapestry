<h1>Blog Posting Site</h1>
<img src="https://github.com/user-attachments/assets/295b4775-134e-473a-9251-1e1f9ed9b2a1">
This project was made to display my skills with frontend and backend programming to construct a full stack web application.
I used flask as the server for the site and css, bootstrap and javascript for the styling and responsivity of the website.
<h3>Navigating the website</h3>

<p>Viewing and commenting on posts:</p>

https://github.com/user-attachments/assets/8fc0c637-bfd2-478c-8852-d9a2044a567b

<h3>User Authentication</h3>

I used flask login authenticator to authenticate users, when a user registers their email and name is stored in the SQLite database and their password is hashed and salted using the werkzeug security package. When a user then wants to login using their username and password, the password is hashed and salted again then compared with the corresponding email's password in the database and if they match then the user is authenticated. Any user that is registered and logged in can then comment on posts. 

<h3>Database</h3>

I used SQLite as my database and SQLAlchemy to create tables, read and write data, forms are used to read data that is input by users and this data is then read and written into the database. The html files then write the data from the database through flask, SQLAlchemy. Database relationships were used to keep track of what users made comments on posts, what users made posts and all comments that are made on a post, One to many relationships was used to do this.

<h3>Running the file</h3>

To run this file locally you will need to delete the current posts.db file so when the code is run a new empty database (with the tables) is automatically created in the "instance" folder, the first user to register is then the admin of the server and can make posts, delete posts and edit posts (only the admin can do so). Every other user can comment on post and their comment and name is displayed in the comment section.
