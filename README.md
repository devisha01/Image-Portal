Cloud_Project_2
===============

This is an image portal application.
It shows picture in reverse chronological order, along with a caption and hashtags.
Users can upload their own images, with a caption and hashtags, or search the images using the hashtags.
Users can also invite their friends to join in.
Application Link : http://cloudprojecttest1-1252.appspot.com/   
Users can login through the main page and upload, caption and search images. The users have an option of giving captions and adding hashtags for the image while uploading. The addition of hashtags provide a searchable query for finding the photos. The user can enter one #hashtag and click on search, this displays all the images with that hashtag. As the user uploads images, an image pool of all images is displayed at the top. The user also has an option of sending an invite to a friend's email address. 
The services used in this project are as follows:
* ndb
* users
* images
* mail
* app_identity
* search

The NDB API provides persistent storage in a schemaless object datastore. NDB saves data objects, known as entities. An entity has one or more properties like string, an integer, datetime, key or a reference to another entity. 
Users is used for authentication. While a user is signed in to the application, the app can access the user's email address , as well as a unique user ID. The app can also detect whether the current user is an administrator, making it easy to implement admin-only areas of the app.
The Images sevice is used for uploading the image and properties like image resize, image data, author, etc.
The Mail  service is used for sending friend invite to other email addresses. The app sends messages using the Mail service and receive messages in the form of HTTP requests initiated by App Engine and posted to the app.
The app_identity service is used for generating project id of the app so that it can be used for sending friend invite to other email addresses.
The search service is used for searching the images by #hashtag.