Assignar Python/Django Tech Test
================================

This is a base project for technical tests we use in our hiring process.

The actual technical tasks and challenges are not included in this repo 
so that we are able to customise the tasks/challenges according to the 
roles we are looking for.    


Setup
-----

### Installation

This project is a very minimal Python setup. You are free to set 
it up locally in your own way (`virtualenv`, `venv`, `pyenv`, `poetry`, 
Docker, etc.). 

Here is an example:

```
python -m venv .venv
source .venv/bin/activate
pip install -r requirements.txt
```

### Database setup

Setup your initial database (SQLite).
    
    $ ./manage.py migrate
    
Create your first superuser.

    $ ./manage.py createsuperuser
    
Load initial seed data.

    $ ./manage.py loaddata images

Development
-----------

### Running the server

    $ ./manage.py runserver


Project Information
-------------------

This is a Django example project (`imagedb`) that includes one Django 
app called `images`.

The `images` app uses two models, `Image` and `ImageLabel`.

* `Image` - refers to an image that you can upload/download.
* `ImageLabel` - refers to a label of an object inside the image.

An `Image` can have multiple `ImageLabel`s. An `ImageLabel` belongs to 
only one `Image`.

A basic Django admin page is available at http://localhost:8000/admin. 
