
# Things I learned: 
STEPS: 
1. Had to create a form in my post.ejs with two params for my post id and user id. This would allow me to know who created the post and the id of post the user was commenting on
2. I proceeded to my routes folder went to my posts.js file to handle my request and added my endpoint with my two params. I also created a callback function which i will make in my controller folder specifically in posts.js file
3. In my controller folder in file posts.js created a comment to my Mongo DB and refreshing the pg w/ that comment 
4. Following with going to folder models and created a new comment.js file for my new comment schema which i reference in step 3
5. Then go and update my getPost in my controller folder in file posts.js. I updated it by finding the commments by post id and sorting it by date it was created. I then render it to my ejs file to display it 
6. I dynamically created cards with my for loop to display users comments and rendered it on pg


# Install

`npm install`

---

# Things to add

- Create a `.env` file in config folder and add the following as `key = value`
  - PORT = 2121 (can be any port example: 3000)
  - DB_STRING = `your database URI`
  - CLOUD_NAME = `your cloudinary cloud name`
  - API_KEY = `your cloudinary api key`
  - API_SECRET = `your cloudinary api secret`

---

# Run

`npm start`

