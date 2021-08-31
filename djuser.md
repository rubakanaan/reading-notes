# Django Custum User Model

* Django ships with a built-in User model for authentication, however the official Django documentation highly recommends using a custom user model for new projects. The reason is if you want to make any changes to the User model down the road--for example adding a date of birth field--using a custom user model from the beginning makes this quite easy. But if you do not, updating the default User model in an existing Django project is very, very challenging.

**always use a custom user model for all new Django projects**

* To start, create a new Django project from the command line. We need to do several things:

    * create and navigate into a dedicated directory called accounts for our code
    * install Django
    * make a new Django project called config
    * make a new app accounts
    * start the local web server

### AbstractUser vs AbstractBaseUser

* There are two modern ways to create a custom user model in Django: AbstractUser and AbstractBaseUser. In both cases we can subclass them to extend existing functionality however AbstractBaseUser requires much, much more work. Seriously, don't mess with it unless you really know what you're doing. And if you did, you wouldn't be reading this tutorial, would you?


### Custom User Model

* Creating our initial custom user model requires four steps:

    * update config/settings.py
    * create a new CustomUser model
    * create new UserCreation and UserChangeForm
    * update the admin

### Superuser
* It's helpful to create a superuser that we can use to log in to the admin and test out log in/log out. On the command line type the following command and go through the prompts.

* **DjangoX**,is an open-source Django starter framework that includes a custom user model, email/password by default instead of username/email/password, social authentication, and more.