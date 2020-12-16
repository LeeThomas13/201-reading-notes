[Django Custom User Model](https://learndjango.com/tutorials/django-custom-user-model)

Django ships with a built-in User model for authentication and if you'd like a basic tutorial on how to implement log in, log out, sign up and so on see the Django Login and Logout tutorial for more.

However, for a real-world project, the official Django documentation highly recommends using a custom user model instead. This provides far more flexibility down the line so, as a general rule, always use a custom user model for all new Django projects.

MAKE YOUR OWN CUSTOM USER MODEL!

When doing so, do NOT MIGRATE until we've created our new custom user model.

There are two modern ways to create a custom user model in Django: AbstractUser and AbstractBaseUser. In both cases we can subclass them to extend existing functionality however AbstractBaseUser requires much, much more work. Seriously, don't mess with it unless you really know what you're doing. And if you did, you wouldn't be reading this tutorial, would you?

Abstract Base User === MUCH MORE WORK

Creating initial custom user model:
update config/settings.py
create a new CustomUser model
create new UserCreation and UserChangeForm
update the admin


[Back To Homepage](https://leethomas13.github.io/201-reading-notes/)