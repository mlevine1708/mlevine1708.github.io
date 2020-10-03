---
layout: post
title:      "Rails Student Directory"
date:       2020-10-03 21:00:28 +0000
permalink:  rails_student_directory
---


It's hard to imagine that when I first started my Rails project back in March that I would just be finishing it on October 3!  But that's where we are, for better or worse.  I am a middle school teacher and once COVID hit in March and I had to switch to online teaching, in addition to many responsibilities helping other teachers adjust as I am an instructional team leader, plus help my 7 year old with his new online learning for first grade, coding at Flatiron fell way behind on what I was able to handle in a given day.  So I took a long hiatus from coding.

Fast forward to the summer, where I obtained a long-sought after teaching job, teaching Computer Science to middle schoolers.  Very exciting and I was very happy to make this transition I had been looking forward to for a long time.  However, this delayed my work on my Rails project even more.

I finally got back to working on it consistently around September, but went through multiple different ideas for the app as I worked on relearning everything I had learned about Rails six months ago.  All this to really say that my app is simple, but I finally finished it and I believe it fits all the requirements!

I ended up creating a Student Directory app.  Basically it is for parents with younger children, who want to easily keep contact information for their children's friends.  This is helpful to set up play dates, parties, etc.

There are three models - user (which is the parent), student, and teacher.  The student model is used as the join table, and the student belongs to both the user and teacher.  The teacher has many students and has many users, through students.  The user has many students and has many teachers through students.  

Once the user is logged in to the app, they can view all of the students listed, along with their homeroom teacher and contact information.  They can also add new students and new teachers.  Users can view the database as a list of all the students, or look at individual teachers or students.  They may also delete or edit student data.

The app saves the information and so this is also available for the user to share with other parents to create a larger database of contact information, obviously making sure all parents agree to sharing it.

I understand this app is simple and not very robust, but I am very proud that I persevered and got to the end of it.  There were many moments where I almost just gave up and quit.  But I didn't and I am proud of myself and excited to move on to the next section of this program.
