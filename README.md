# The Pizza Place - Introduction

**The Pizza Pace** Restaurant delivery app created using the Django framework that allows for the creation, reading,
updating and deleting of data to a database. 

> It targets **tourist destinations** of India, where user can view the blog post of tourist destinations.
The user can view the blog post and comments. When the user is logged in, user can like/unlike a post, comment on a post and add a post from the user page.

You can view the live site here:- https://incredible-india.herokuapp.com/


![mockup](assets/mockup.jpg)

----

## [Content](#content)
- [Incredible India - Introduction](#incredible-india---introduction)
  - [User Experience - UX](#user-experience---ux)
    - [Site Aims](#site-aims)
    - [Agile Methodology](#agile-methodology)
      - [Epics and User Stories](#epics-and-user-stories)
      - [Tasks](#tasks)
  - [Design](#design)
    - [Colours](#colours)
    - [Typography](#typography)
    - [Imagery](#imagery)
    - [Wireframes](#wireframes)
  - [Database Diagram](#database-diagram)
  - [Features](#features)
    - [Home Page](#home-page)
      - [Navbar](#navbar)
      - [Hero Image](#hero-image)
      - [Destination Section](#destination-section)
      - [Footer](#footer)
    - [User Page](#user-page)
    - [About Page](#about-page)
    - [Blog Page](#blog-page)
      - [Blog Details](#blog-details)
      - [Blog Comments](#blog-comments)
    - [Register](#register)
    - [Login](#login)
    - [Logout](#logout)
    - [Destinations](#destinations)
    - [Search Button](#search-button)
    - [Alert Messages](#alert-messages)      
  - [Admin Panel/Superuser](#admin-panelsuperuser)
  - [Technologies Used](#technologies-used)
    - [Languages Used](#languages-used)
    - [Django Packages](#django-packages)
    - [Frameworks - Libraries - Programs Used](#frameworks---libraries---programs-used)
  - [Testing](#testing)
      - [Validation](#validation)
      - [Manual Testing](#manual-testing)
  - [Bugs](#bugs)
      - [Fixed Bugs](#fixed-bugs)
      - [Unfix Bugs](#unfix-bugs)
  - [Deployment](#deployment)
      - [Creating the Django project](#creating-the-django-project)
      - [Creating Heroku app](#creating-heroku-app)
      - [Set up Environment Variables](#set-up-environment-variables)
      - [Heroku deployment](#heroku-deployment)
      - [Final Deployment](#final-deployment)
  - [Credits](#credits)
    - [Content](#content)
    - [Information Sources / Resources](#information-sources--resources)
  - [Acknowledgement](#acknowledgement)

-----

# User Experience - UX

## Site Aims

* The pizza place is a website designed to allow customers to view the menu and order food. 
* The website navigation and appearance is designed to be simple and easy to use.
* This website allows the user add and remove items from their order as well as allowing the site admin to add and remove menu items.
* The site allows the admin to create, read update and delete data in the database.

## User Stories

User stories were utalised to create realisitic scenarios and appropriate features to delivery to the user's needs. 

<img src="./coderscafe/media/readme_files/user-story-one.png" width="800">
<img src="./coderscafe/media/readme_files/user-story-two.png" width="800">
<img src="./coderscafe/media/readme_files/user-story-three.png" width="800">

A common theme in the user stories is the need for convience when ordering food. For this reason the navigation of the website must remain simple to allow 
for quick and simple navigation. It should also always be possible for the user to make an order from any page of the website. A link placed in the footer and header will allow for this. The point here is to make the process of tranacting on the website as frictionless as possible

### Website UI
Epic Goals for User- 
* A simple and easy to navigate user interface.
* The uses and functions of the website are immediataly obvious to the user on the landing page.
* Have easy and quick asses to the menu and the corresponding menu items description.
* Search bar to allow for quicker on site navigation.

### Registration and Account Management
* Quick and simple account creation. 
* Allow admin to easily create, read, update and delete menu items from the data base.
* Allow admin accounts to be created and removed.

### Admin Management
* Create / Update / Read / Delete menu items, descriptions.
* View a history of admin actions taken.
* Add and remove user accounts.

[Back to top](#content)

## Design

### Typography

Italiana was used throughout with a backup of sans-serif. It was chosen because it relates tot he Italian selection of the restaurant.

### Imagery

All images were sources from pexels.com. They were seleted for their appealing and accurate representation of the menu items. 

### Wireframes
The wireframes were created using Figma.

<img src="./coderscafe/media/readme_files/homepage-wireframe.png" width="800">
<img src="./coderscafe/media/readme_files/description-wireframe.png" width="800">
<img src="./coderscafe/media/readme_files/menu-wireframe.png" width="800">

----

# Features

## Home Page

At the very first glimpse, user can see a Navigation menu with a search button and carousel-images on the homepage. Homepage provides the user with some quick information about the site and make use of all its features. User do not need to be registered to view a blog post. The responsive navigation bar is featured on all pages. 

<img src="./coderscafe/media/readme_files/homepage.png" width="800">

----

## About Page

The about page gives a simple description of the restaurant and the Italian theme of the menu.

<img src="./coderscafe/media/readme_files/about-page.png" width="800">

----

## Menu Page

The menu page shows all the menu items along with their description. 

<img src="./coderscafe/media/readme_files/menu-page.png" width="800">


## Navbar after loged in user

* If the user is logged in (username Mahi is provided as an example here), navbar will be shown with user name and logout options. On a desktop, the navigation menu will appear as shown below:

![logged-in-user-Navbar](assets/features/logged-in-user-navbar.jpg) 

## User Page

* This page will be only visible to logged-in user. Navbar will show this page with the username on it. When the user clicks on his/her name in the navbar, the user navigates to the User page. On this user page, the user can create new posts or view his old posts list to edit and delete any of his posts.

![logged-in-user-page](assets/features/logged-in-user-page.jpg) 

* When user clicks on the 'Add New Post' button, following form will be displayed.

![Add-post](assets/features/add-post-form.png)

* If the user does not provide an image, the following default image will be presented.

![Default-post-image](assets/features/default-post-image.jpg)


* User can access all his posts by clicking on 'View Old Post' button. User can see the list of posts in this page which he has posted till now. Here he/she can edit or delete any of his post.

![user-post-list](assets/features/user-post-list.jpg) 
![edit-delete-post](assets/features/edit-delete-post.jpg)

* If the user wants to edit his/her post, the following update form will be displayed with pre-filled content.

![update-post](assets/features/update-post-form.png)


* User can see the following message to make sure to delete his post.

![delete-post](assets/features/delete-post.jpg)


* If the user hasn't posted anything before, the user will be shown that there are no posts and they can create.

![no-user-post](assets/features/no-user-post.jpg) 

----

## Footer

- On the website footer, users can see basic information such as my social media, copyright, and a quote about Incredible India.

![Navbar](assets/features/footer.jpg)

----

## About Page

- The About Page gives, users information about the Incredible India with a brief discription of india and the travel options to reach there.

![About Us](assets/features/about-us-page1.jpg)
![About Us](assets/features/about-us2.jpg)

----

## Blog Page

This page enlists all the blog posts added so far to the website. The blog posts is paginated in a way that 9 posts are displayed. Further post can be accessed by clicking next button. Each blog post shows the image overlay with the destination type. The card body displays blog post title with specific fields and sliced post content along with the name of author, submitted date and shows the number of likes and comment icon in the card footer.

![Blog Page](assets/features/blog-page1.jpg)
![Blog Page](assets/features/blog-page2.jpg)

----

## Post-Detail Page

- When a user clicks on the image or title of the blog post, they are brought to the post details page for the selected blog post. Here the user is shown the complete details of the blog post with image, author name, created time, title, best time, ideal-duration, number of likes and comments along with full content.
- Underneath the post description the page displays all the approved comments on that blog post posted by signed-in users. 
- At the bottom of this page, the Comment box is visible to the users.

![Post-detail](assets/features/post-details1.jpg)
![Post detail](assets/features/post-details2.jpg)

- If user is signed-in, following comment box will appear. 

![Comment box](assets/features/comment-box-login-user.jpg)

- When User submit a comment or like/unlike a post, following messages/ alert displays respectively.

![Comment-alert](assets/features/comment-alert.jpg)
![Like post alert](assets/features/like-alert.jpg)
![Unlike-post-alert](assets/features/unlike-alert.jpg)

- Signed-in users can only edit/delete their own comments.

![Edit Delete Comment](assets/features/edit-delete-comment.jpg)

- When the user clicks on the delete button to remove his comment, following alert message pops up.

![Delete Comment Alert](assets/features/delete-comment-alert.jpg)


- User navigates to the edit-page when he clicks on the edit button. Here he can edit his comment text. 
![Edit Comment](assets/features/edit-comment.jpg)

- When user clicks on update button, a successful update alert message is displayed.

![Update Comment Alert](assets/features/update-comment-alert.jpg)

----

## Destination Page

User can select a specific destination blog posts either from destination section on home page or from the navbar dropdown which navigates to that specific destination blog posts.

![Dropdown destination](assets/features/dropdown-destination.jpg)

- For example, if user select a destination such as a hill station, the filtered blog posts will be displayed.
![Filter destination posts](assets/features/selected-destination-post.jpg)

- If there is no post for any selected destination, user will see the following message.
![No post message](assets/features/no-destination-post.jpg)

----

## Security
In order to properly interact with the website, the user needs to have an account and sign in. This ensures security of their comments and gives them rights to create, modify and delete them.

### Sign Up

- User is asked to enter username and password to sign up. User will be guided by validation messages if the username exists or password is too small which was created by modifying Django inbuilt templates.
![Signup page](assets/features/user-register-page.jpg)

- When users sign up to the website they will see a message at the top of the page saying "Successfully signed in as (username)".
![Sign Up alert](assets/features/user-registration-alert.jpg)

### Sign In

- User can enter username and password to sign in. User will be guided by validation messages if the username or password is not correct. This was created by modifying Django inbuilt templates.

![Sign In page](assets/features/user-login-page.jpg)

- When users sign in to the website they will see a message at the top of the page saying "Successfully signed in as (username)".

![Sign In alert](assets/features/signed-in-alert.jpg)

### Sign Out

- If the user is signed-in, then only they can see Logout nav-item in navbar. User will be taken to the Sign Out page. This was created by modifying Django inbuilt templates. When the user signs out, they are redirected to homepage.

![Sign out page](assets/features/logout-page.jpg)

- When users log out of the website they will see a message at the top of the page saying "You have signed out".

![Sign out alert](assets/features/signout-alert.jpg)

----

## Search Button 

On the top right corner, a search input field is provided along with a button to submit. This allows the user to try and find the post they are looking for.

![Search button](assets/features/search-button.jpg)

- On the search results page, users can see posts related to their search. If there are posts for the user's search input, the user can click on the card result to go to the post detail page.

![Search result](assets/features/search-result.jpg)

- On the search results page, users will see this message if nothing is found for the search.

![Search result](assets/features/no-search-result.jpg)

- On the search results page, users will see this message for empty input.

![Search result](assets/features/empty-input-for-search.jpg)

----

[Back to top ⇧](#content)

## Admin Panel/Superuser

- Admin accesses the project via logging into Django admin panel with a superuser id and password. The page appears as shown [here](assets/features/admin-panel-login.jpg).
- A superuser "admin" was created for this project to manage the admin panel.
- On the Admin Panel, as an admin I have full access to CRUD functionality so I can view, create, edit and delete the following ones:
  - Posts
  - Comments
  - Author
  - Destination
- As admin I can also approve comments, approve posts and change the status and give other permissions to the users.

### Admin 'Post' Model Management

- On selecting Blog "Post", a list of blog posts is displayed with its title, slug, status, created_on and author name. Admin can select the post and edit or delete its data.
- When a blog post is submitted by a user, its status is set to Draft by default.
- When the status is set to Publish on Admin Approval, the post starts appearing in the website.

The admin site for post model appears as shown [here](assets/features/admin-panel-post-model.jpg).

### Admin 'Comment' Model Management

- Upon selecting the Blog "Comment" model, a list of comments on a post is displayed with the username, comment body, post title, status and created_on. Admin can select the comment and edit or delete its data.
- When a comment is submitted by a user, it requires approval from an admin in order to publish it on the comments section.

The admin site for comment model appears as shown [here](assets/features/admin-panel-comment-model.jpg).

### Admin 'Destination' Model Management

- On selecting the Blog "Destination" model, a list of destinations for the blog post is displayed with title, slug and excerpt fields. Only Admin can add, edit or delete any destination data.

The admin site for destination model appears as shown [here](assets/features/admin-panel-destination-model.jpg).

----

## Technologies Used

### Languages Used

* [HTML 5](https://en.wikipedia.org/wiki/HTML/)- Used to structure all the templates on the site
* [CSS 3](https://en.wikipedia.org/wiki/CSS)- to provide extra styling to the site
* [JavaScript](https://www.javascript.com/)- Minimum javascript was used to fade out alerts after a few seconds.
* [Python](https://www.python.org/)- To provide the functionality to the site. Packages used in the project can be found in requirements.txt

### Django Packages

* [Gunicorn](https://gunicorn.org/)- As the server for Heroku.
* [Cloudinary](https://cloudinary.com/)- Was used to host the static files and media for the site.
* [Dj_database_url](https://pypi.org/project/dj-database-url/)- To parse the database URL from the environment variables in Heroku.
* [Psycopg2](https://pypi.org/project/psycopg2/)- As an adaptor for Python and PostgreSQL databases.
* [Summernote](https://summernote.org/)- As a text editor.
* [Allauth](https://django-allauth.readthedocs.io/en/latest/installation.html)- For authentication, registration, account management.
* [Crispy Forms](https://django-crispy-forms.readthedocs.io/en/latest/)- To style the forms.

### Frameworks - Libraries - Programs Used

* [Django](https://www.djangoproject.com/) was used as the framework for the back-end logic of the project. Django enables rapid and secure development.
* [Bootstrap](https://getbootstrap.com/)- Used to style the website, add responsiveness and interactivity.
* [Git](https://git-scm.com/)- Used for version control by utilizing the Gitpod terminal to commit to Git and push to GitHub.
* [GitHub](https://github.com/)- Used to store the project's code after being pushed from Git.
* [Heroku](https://id.heroku.com)- Used to deploy the live project.
* [PostgreSQL](https://www.postgresql.org/)- Database used through heroku.
* [Balsamiq](https://balsamiq.com/)- To build the wireframes for the project.
* [Google Chrome Developer Tools](https://developers.google.com/web/tools/chrome-devtools) was used to inspect page elements, debug, troubleshoot and test features and adjust property values. Using the Lighthouse extension installed in Chrome Browser, the performance report was generated.
* [Google Fonts:](https://fonts.google.com/) used for the Roboto font
* [Font Awesome:](https://fontawesome.com/) was used to add icons for aesthetic and UX purposes.

-----

[Back to top ⇧](#content)

## Testing

### Validation
I used the following validation tools to validate HTML, CSS, PYTHON codes. Below the link of TESTING.md file, which includes all validation results.  
- HTML using [W3C HTML validator](https://validator.w3.org/)
- CSS using [Jigsaw CSS validator](https://jigsaw.w3.org/css-validator/)
- Python via [PEP8 CI Python Linter](https://pep8ci.herokuapp.com/)

### Manual Testing
Testing has taken place continuously throughout the development of the project. Each view was tested regularly. When the outcome was not as expected, debugging took place at that point. An exhaustive list of features were checked on different devices and browsers. They were performed and their scrrenshots can be found in the features section on how the distinct features render. All clickable links redirect to the correct pages.

- Link for TESTING.md file:- [Testing Results Here](TESTING.md)

----

## Bugs

| **Bug** | **Fix** |
| ----------- | ----------- |
| In navbar, the menu item destination dropdown was not populating.| Create destination_list view that return context (destination_list) then add `'blog.views.destinations_list'` in templates section in settings.py file |
| Post image was not rendering on post_detail page(Issue only for mobile screens). | Remove class 'd-none' from post_detail page |
| Alert messages was not disappeare after setTimeOut(2000)<br><details><summary>Alert Code</summary><img src="assets/alert-js.jpg"></details> | Copy code from bootstrap alert and customize with forEach <br><details><summary>New Alert Code</summary><img src="assets/new-alert-js.jpg"></details>|
| Destination dropdown was again not populating. | Remove script scr 'bootstrap.min.js' because there is already 'bootstrap.bundle.min.js' |
| Automated test was not working because of postgres database | Connect with local db.sqlite3 while running unit test<br><details><summary>Override database for unit test</summary><img src="assets/local-bd-for-unittest.jpg"></details>  |


| **Unfix Bug** |
| ----------- | 
| When a logged in user adds a new post, the post slug should automatically be created from the post title. But the slug field is empty in the database. Slug is a required field when admin publishes a draft post, so here admin manually filled the slug field during publishing. Below is the screenshot from the post model in admin panel and view for Add Post.<br><details><summary>Empty slug screenshot</summary><img src="assets/empty-slug.jpg"></details><details><summary>Add Post View</summary><img src="assets/addPostView.jpg"></details> 

----

## Future Implementation

* Automated testing for views functions 
* Adding and displaying replies below corresponding comments on our blog

[Back to top ⇧](#content)


## Deployment

### 1. Creating the Django Project
* Go to the Code Institute Gitpod Full Template [Template](https://github.com/Code-Institute-Org/gitpod-full-template).
* Click on `Use This Template` button, then create new repository.
* Name our repository and click on `Create repository from template` button.
* Once the template is available in your repository click on `Gitpod` button.
* When the image for the template and the Gitpod are ready, open a new terminal to start a new Django App.
* Install Django and gunicorn: `pip3 install 'django<4' gunicorn`.
* Install supporting database libraries dj_database_url and psycopg2 library: `pip3 install dj_database_url==0.5.0 psycopg2`.
* Install Cloudinary libraries to manage static files: `pip install dj-3-cloudinary-storage`.
* Create file for requirements: `pip freeze --local > requirements.txt`.
* Create project:`django-admin startproject project_name .`.
* Create app: `python manage.py startapp app_name`.
* Add app to list of `installed apps` in settings.py file: `'app_name'`.
* Migrate changes: `python manage.py migrate`.
* Test server works locally: `python manage.py runserver`.
* If the app has been installed correctly the window will display- The install worked successfully! Congratulations!

### 2. Create your Heroku app
* Navigate to [Heroku](https://id.heroku.com).
* Create a Heroku account by entering your email address and a password (or login if you have one already).
* Activate the account through the authentication email sent to your email account.
* Click the **new button** on the top right corner of the screen and select create a new app from the dropdown menu.
* Enter a unique name for the application.
* Select the appropriate region for the application.
* Click create app.
* Click Reveal Config Vars and add a new record with `DATABASE_URL`.
* Click Reveal Config Vars and add a new record with `PORT`.
* Click Reveal Config Vars and add a new record with the `DISABLE_COLLECTSTATIC = 1`(note: this must be either removed or set to 0 for final deployment).
* Next, scroll down to the Buildpack section, click `Add Buildpack` select python and click Save Changes.

### 3. Set up Environment Variables
* In you IDE create a new env.py file in the top level directory.
* Add env.py to the .gitignore file.
* In env.py import the os library.
* In env.py add `os.environ["DATABASE_URL"]` = "Paste the link copied from Heroku DATABASE_URL".
* In env.py add `os.environ["SECRET_KEY"] = "Make up your own random secret key"`.
* In Heroku Settings tab Config Vars enter the same `SECRET_KEY` created in env.py by entering 'SECRET_KEY' in the box for 'KEY' and your randomly created secret key in the 'value' box.

### 4. Setting up settings.py
* In your Django 'settings.py' file type:

 ```
 from pathlib import Path
 import os
 import dj_database_url

 if os.path.isfile("env.py"):
  import env
 ```
* Remove the default insecure secret key in settings.py and replace with the link to the secret key variable in Heroku by typing: `SECRET_KEY = os.environ.get(SECRET_KEY)`
* Comment out the `DATABASES` section in settings.py and replace with:
```
DATABASES = {
  'default': 
  dj_database_url.parse(os.environ.get("DATABASE_URL"))
  }`
```
* Create a Cloudinary account and from the 'Dashboard' in Cloudinary copy your url into the env.py file by typing: `os.environ["CLOUDINARY_URL"] = "cloudinary://<insert-your-url>"`
* In Heroku, click Reveal Config Vars and add a new record with the `CLOUDINARY_URL`
* Add Cloudinary libraries to the installed apps section of settings.py file:
 ```
 'cloudinary_storage'
 'django.contrib.staticfiles''
 'cloudinary'
 ```
* Connect Cloudinary to the Django app in `settings.py`:
```
STATIC_URL = '/static'
STATICFILES_STORAGE = 'cloudinary_storage.storage.StaticHashedCloudinaryStorage'
STATICFILES_DIRS = [os.path.join(BASE_DIR, 'STATIC')]
STATIC_ROOT = os.path.join(BASE_DIR, 'staticfiles')
MEDIA_URL = '/media/'
DEFAULT_FILE_STORAGE =
'cloudinary_storage.storage.MediaCloudinaryStorage'
* Link file to the templates directory in Heroku 
* Place under the BASE_DIR: TEMPLATES_DIR = os.path.join(BASE_DIR,
'templates')
```
* Change the templates directory to TEMPLATES_DIR. Place within the TEMPLATES array: `'DIRS': [TEMPLATES_DIR]`
* Add Heroku Hostname to ALLOWED_HOSTS: 
```ALLOWED_HOSTS = ['<Heroku_app_name>.herokuapp.com', 'localhost']```
* Create Procfile at the top level of the file structure and insert the following:
    ``` web: gunicorn PROJECT_NAME.wsgi ```

* Commit and push the code to the GitHub Repository.

### 5. Heroku Deployment: 
* Click Deploy tab in Heroku.
* Select Github as the deployment method.
* Confirm you want to connect to GitHub.
* Search for the repository name and click the connect button to link the heroku app with the Github repository. The box will confirm that heroku is connected to the repository.
* Scroll to the bottom of the deploy page and select the preferred deployment type.
* Click either Enable Automatic Deploys for automatic deployment when you push updates to Github or To manually deploy click the button 'Deploy Branch'. The default 'main' option in the dropdown menu should be selected in both cases. When the app is deployed a message 'Your app was successfully deployed' will be shown. Click 'view' to see the deployed app in the browser.

### 6. Final Deployment
In the IDE:
* When development is complete change the debug setting to: `DEBUG = False` in `settings.py` 
* In Heroku settings config vars change the `DISABLE_COLLECTSTATIC` value to 0
* Because DEBUG must be switched to True for development and False for production it is recommended that only manual deployment is used in Heroku. 
* To manually deploy click the button 'Deploy Branch'. The default 'main' option in the dropdown menu should be selected in both cases. When the app is deployed a message 'Your app was successfully deployed' will be shown. Click 'view' to see the deployed app in the browser.

----

[Back to top](#content)

# Credits

## Code
- The basic set up of the website was done by strictly following the steps as described in Code Institue Full Stack Frameworks module - Django walkthrough project `"I Think Therefore I Blog"`.
- Followed the project of one of my friend who is also a CI student (Roshana Vakeel): https://github.com/RoshnaVakkeel/Little_Learners_Lab_Logs/blob/main/logs/forms.py 
- Another project link I found from Linkdin, also CI's student (Laura Mayock): https://github.com/LauraMayock/The-happy-reader
- [The Newsbox](https://github.com/rashdogg74/newsbox86)- One of the project shared by my cohort facilitator on Slack. 

## Learning Resources
- Code Institutes Full Stack Framework Module, mainly the 'blog' walkthrough project.
- Youtube videos by [Codemy](https://www.youtube.com/watch?v=6-XXvUENY_8&list=PLCC34OHNcOtr025c1kHSPrnP18YPB-NFi&index=5)
- [W3CSchool](https://www.w3schools.com/django/)
- [Django Documentation](https://docs.djangoproject.com/en/3.2/ref/models/fields/#field-types)(For different quaries while doing project. For example query about models, fields, form widgets, auth and many more)
- Other open source to understand and solve following types of error : UnboundedLocalError, MultivalueDictKeyError,  ProgrammingError, InvalidCursorName etc.
- Youtube videos [The Dumbfounds](https://www.youtube.com/playlist?list=PLbpAWbHbi5rMF2j5n6imm0enrSD9eQUaM) for automated testing.

## Content and Media

Mostly images and post content are taken from the website https://www.holidify.com/ and https://www.incredible-india.org/. Some images are taken from [Pexels](https://www.pexels.com/).

----

## Acknowledgement

Special thanks to my mentor Sandeep Aggarwal, My fellow student Roshna, Tutor support and Slack community for their assistance throughout this project.

[Back to top](<#content>)
   