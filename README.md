# WatchOutBlog 
Blog for watch enthusiasts created by watch enthusiast.

Please visit the blog in [here](https://watchoutblog.herokuapp.com/).

## Introduction and purpose

The WatchOutBlog has been developed as part of the Milestone project 4 for Code Institute Diploma in Software Development with eCommerce.
The WatchOutBlog is a website blog built in Django, incorporating Python, CSS and HTML.

The blog and its content, in terms of blog posts, is administered by WatchOutBlogger. The nature of the blog posts will be a mix of educational and brand review posts with the overall aim of creating engagement in the watch community across the globe.
The blog community may engage with the WatchOutBlogger as well as other blog users by creating comments under each blog post. Users may also like blog posts to express their interests in specific blog types. The engagement of the blog user is only possible post completion prior user registration process. 

![Multidevice view](static/multidevice/all-devices-black.png)

## Design 

The below section of the document outlines development journey of the blog starting from the concept to ultimate solution used to develop the blog.

### 1 Concept

The overall concept was to develop a blog, which would be administered by its owner. The purpose was to provide educational and brand review blog posts.
Blog users would be invited to register and post completion registration process would be allowed to engage in community through blog posts comments and likes.

In order to appeal to users the blog needed to be visual, therefore homepage is diveded into 4 sections allowing for a good quality picture to give sense to a user in relation to nature of each blog post. In additionl each blog post has blog title associated as well as the date and time as to when it was created.
In order to give a sense of community engagement for each of the blog posts, each blog post on the homepage will also reflect numbre of likes and number of comments.

### 2 Functional scope 

In terms of overall functional scope the following 4 key areas were needed to be developed in order for the blog to operate as required:

**Blog administration** - blog owner to be able to create, post and manage respective blog posts. Blog owner shoudl be also able to manage user comments through approval and where required a deletion process.

**User administration** - blog users to be able to register and login in order to interact with the blogger and other blog users.

**User comments** - registered and logged blog users should be in position to comment on individual blog posts. Users should be also allowed to update and delete their own comments.
   
**User blog likes** - registered and logged blog users should be in position to like individual blog posts. The functionality shoudl also allow for blog users to reverse "a like" previously given to a particular blog post.

### 3 Solution 

In order to develop a website based blog, and given the functional needs the following solutions were used:

**Languagues**
Given the fact that nature of the application indicates a need for a frequent content manipulation, a standard HTML solution will not work.
The solution needed to incorporate Python in order to make the solution more agile, in terms of development of relevant functions and in order for the user actions to be able to interact with the database in place. 
As part of the development the following languages were used:
- HTML
- CSS
- Python

**Database**
The blog application required a database structure, which would support managing blogger's blog posts, storing relavant content and images.
The database also needed to store users information and their interactions with the blog through comments and likes.
For the purpose of managing database related needs, Postgresql was selected as a solution for this project.

The below reflects database schema developed in order to support the needs of this project.

DATABASE SCHEMA PLACEHOLDER

**Development**
For the purpose of development of this project a number of technologies were used. 
- GitHub respository was used to store the project's code after being pushed from Gitpod.
- Gitpod IDE was used for version control by utilizing the Gitpod terminal to commit and Push to GitHub.
- Django framework was used to develop structure of the blog and also to use some of the already developed functions of Django such as user authorisation, admin portal and others.
- Bootstrap5 was used for construction of the blog application and responsivness.
- Cloudinary was used for a purpose of managing images required for running the application.
- Summernote for the purpose of enhanced text editing when managing blog posts.
- Crispy forms library 
- DrawSQL was used for drawing database schema.
- Balsamiq was used for creation of wireframes during the initial design process.
- Google

**Deployment and application hosting**
The application has been deployed and it is hosted on Heroku.
The deployment process has been outlined in a more detailed manner in the latter part of this document.

### 4 Wireframes 

As part of the design process for this process a set of wireframes have been created using Balsamiq application.
The purpose of the wireframes below was to visualise indicatively the user experience, which the blog user will get once the application was fully operation.

The wireframing has been completed for desktop and mobile users.

**Desktop**

Homepage

![desktophome](static/wireframes/desktophome.PNG)

Blog post, comment section and user comment form

![dekstopblogpost](static/wireframes/desktoppost.PNG)

User Sign up

![desktopsignup](static/wireframes/desktopsignup.PNG)

User Login

![desktopsignin](static/wireframes/desktoplogin.PNG)

Comment deletion

![desktopdeletecomment](static/wireframes/desktopdeletecomment.PNG)

Comment update

![desktopupdatecomment](static/wireframes/desktopupdatecomment.PNG)

**Mobile**

Homepage & Blog post, comment section and user comment form

![mobilehome](static/wireframes/mobilehome.PNG)                ![mobileblogpost](static/wireframes/mobilepost.PNG)

User Sign up & User Login 

![mobilesignup](static/wireframes/mobilesignup.PNG)            ![mobilesignin](static/wireframes/mobilelogin.PNG)

Comment deletion & Comment update

![mobiledeletecomment](static/wireframes/mobiledeletecomment.PNG) ![mobileupdatecomment](static/wireframes/mobileupdatecomment.PNG)


### 5 User stories

## User Experience

## Features 

The below illustrates features currently available to blog users.

### Blog navbar
User will find navigation bar, which features WatchOutBlog logo (acting as home buttom), Home, Register and Clock In (Sign in) buttons.

![navbar](static/images/navbar.PNG)

### Blog homepage
Homepage includes 4 blog posts, each of which can be clicked on in order to access entire blog post.

![homepage](static/images/Homepage.PNG)

### Blog individual posts
Individual blog posts will host blog image, content and also reflect number of likes and comments under the blog post.

![blogpost](static/images/blogpost.PNG)

### User comments 
User comment section, under individual blog post, will allow user to read through the comments posted by other users.
Logged in users will be able to use comment form and post their own comment.If a logged in user has already posted before, they will see Delete and Edit icons next to their own comments, allowing for further action on these. The option of deleting or editing comments is exclusively available to logged in users and only for their own comments. 

![usercomments](static/images/Usercomments.PNG)

### User comments deletion
Logged in users who have posted comments before, will be able to delete their own comments. Upon clicking Delete icon they user will be taken to a confirmation page to confirm deletion of their comment.

![commentdeletion](static/images/commentdeletion.PNG)

### User comments update
Logged in users who have posted comments before, will be able to update their own comments. Upon clicking Edit icon they user will be taken to a confirmation page to edit their own comment.

![commentedit](static/images/commentedit.PNG)

### User notification messages
There is set of user notifications available to blog users. Users who log in will receive a message confirming that they logged in. Similarily users who logout will receive a message that they are logged out. In addition user who post a comment under a blog post, will receive a message that their comment is subject to administrator's approval.

![usermessages](static/images/usermessages.PNG)

### Blog user sign up
New users will be able to register by creating their user name and also password.

![signup](static/images/usersignup.PNG)

### Blog user sign in 
Registered users are able to login in order to manage their comments and like posts.

![signin](static/images/usersignin.PNG)

### Blog administration
Blog administration in terms of blog posts, comments approval is managed by Django's admin portal.

![blogpostadmin](static/images/blogpostadmin.PNG)


## Future developments
The below outlines potential future developments in order to enhance user experience and to attract wider user base.

- **User blog collaboration** - complete development to allow registered users to create blog posts, subject to blog owner approval.
This would allow for a greater and more frequent content being added to the blog.

- **User comments with images** - complete development which would allow registered users to post comments along with images. This would allow a greater level of user engagement when discussing watch experiences.

- **Watch news** - complete development of additional page in the blog, which would pull watch related news from number of sources. This would further increase user engagement as the blog would become one stop for blog posts, discussion and also following on the latest watch news.

- **User emails** - create a email confirmation issued to newly registered users who opted to provide their email address.

- **Search option** - develop blog content search options which would allow users to search throughout the blog using keywords.


## Testing 
There has been an extenstive testing completed prior to final deployment.
The 3 key areas of testing were related to functional, resposive user experience and code validation.

**Functional**
The functional testing has been completed manually and the test scenarios, expected results, actual results and overall test results have been captured in the document below.

PLACEHOLDER FOR TEST RESULTS


**Responsive user experience**



**Code validation testing**
The code itself was validated using HTML - W3C HTML Validator,CSS - Jigsaw CSS Validator and Python - PEP8Online.
Results have been outlined below


**HTML code validation**

The code validation process in HTML - W3C HTML Validator has provided the below results.

Base.html

![base](static/testing/base.png)

Post_detail.html

The validation had highlighted bad value error, which upon further testing does not cause any functional or performance issues.
Due to time constraints the error will not be resolved prior to submission of this project.

![post](static/testing/postdetail.png)

Comment_confirm_delete.html

![delete](static/testing/commentdelete.png)

Comment_form.html

![update](static/testing/commentedit.png)

Login.html

![login](static/testing/login.png)

Logout.html

![logout](static/testing/logout.png)

Signup.html

![signup](static/testing/signup.png)

**Python code validation**

The code validation process in PEP8Online has not highlighted any code errors.
The screenshots confirming validation outcomes may include some details of the code however none of this is confidential or something, which could pose security concern.

Admin.py

![admin](static/testing/adminpy.png)

Apps.py

![apps](static/testing/appspy.png)

Forms.py

![forms](static/testing/formspy.png)

Model.py

![model](static/testing/modelpy.png)

Settings.py

![settings](static/testing/settingspy.png)

Urls.py

![urls](static/testing/urlspy.png)

Views.py

![views](static/testing/viewspy.png)

**CSS code validation**
The code validation process in Jigsaw CSS Validator has not highlighted code errors.

![css](static/testing/css.png)

**Lighthouse – Dev Tools**

Lighthouse testing has been also completed for both, desktop and mobile.

*Desktop*

![lighthousedesktop](static/testing/desktoplighthouse.PNG)

*Mobile* 

![lighthousemobile](static/testing/mobilelighthouse.PNG)


**Bugs**

  **Fixed Bugs**
  

  
  **Unfixed Busg**
  


 
## Deployment 


## Credits
















