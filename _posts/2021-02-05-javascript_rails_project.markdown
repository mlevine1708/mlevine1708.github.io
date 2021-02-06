---
layout: post
title:      "Javascript/Rails Project"
date:       2021-02-06 02:31:09 +0000
permalink:  javascript_rails_project
---


For the Javascript/Rails Project, I was tasked with creating a single-page application.  The frontend would consist of HTML, CSS, and Javascript, while the backend would be run with Ruby and Rails.  It took me a little while to comprehend what it meant to have a frontend and backend application running together, but once I "got" it, it was really cool to see.

In my previous project, which was Rails, I made a website that was meant as kind of a "contacts" database for parents to collect contact information for their children's friends.  I decided to re-use this as a basis for my new project.  From this, I came up with a "Student Contacts" website, so teachers can keep a running contact list of their students, both past and present.  As a teacher myself, I thought this was an interesting idea since we always have our students' contact information, but once they leave our classes, the database with that information is deleted.  If we want to get in touch with previous parents, etc., it is difficult to do.  So, I thought this might be a helpful tool for teachers.

The Javascript application was supposed to use Object Oriented Javascript (classes) and I created a "Students" class for this.  The domain models I included had a "teacher," who had many "students."  It also had "students," who belonged to "teachers."  

The really cool part about this project was having the Javascript side (frontend) talk to the Rails side (backend).  Of course, it was only cool once I figured out how to do it!  All data requests are handled asynchronously, also called AJAX, which means that the website does not need to refresh every time you add a new student, or change anything else.  The webpage used JSON as the communication format.

I incorporated three AJAX calls, using CRUD - create,  read, update, delete.  Users are able to "create" a new student, "update/edit" the student, and "delete" a student.  These tasks are all done without having to refresh the page, which I really liked.

This was a difficult project, of course, but I'm glad I persevered through it.  I learned quite a bit and feel much more confident in my abilities to program something in both the frontend and backend of an application.
