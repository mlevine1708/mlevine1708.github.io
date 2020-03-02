---
layout: post
title:      "My Sinatra App"
date:       2020-03-02 14:26:11 +0000
permalink:  my_sinatra_app
---


## Idea

For my Sinatra project, I wanted to create something that could actually turn out to be useful.  My current career is in elementary education, so I thought it'd be an interesting idea to make something for teachers.  As a teacher, one of the biggest issues, in elementary especially, is making sure all students have passed in their assignments.  So I decided to make an app that could keep track of a teacher's students and assignments.


## MVC
Getting everything coordinated and working in the MVC sections was of course the most difficult aspect of this project, in my opinion.  I had models for the user, students, and assignments.  A user has many students and many assignments.  A student belongs to a teacher and has many assignments.  An assignment belong to a user.  I created controllers for the each model, which ran through the Application Controller.  I implemented CRUD in my views for the students and assignments, so the user can create, read, update, and delete his/her entries.


## The Best Part For Me
The aspect I think I liked best about this is seeing how the user authentication worked.  Once I got it working, it was especially cool to see that when I was logged in to my app, I could edit or delete my entries.  But if I was logged in as someone else, I was not able to edit or delete the entries that that particular user did not create.


## Stretch Goals
One part I'd like to continue to work on is connecting the assignments with the students more.  Right now, it will list all of the students and assignments a teacher has, but I'd love for it to show which assignments each student has turned in, which was the original intent.  
