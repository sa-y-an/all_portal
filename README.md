# All Portal

A simple portal for posting and applying made possible by django.

## Use Cases 

<p>
Can be easily modified to be used in any place where one user group posts a project or job and another user group applies to it. 
</p>

<u>Common use cases - </u>
- College's Research portal where teacher can post a project and student can apply
- Jobs Portal - Companies posts jobs and user applies 

## Usage Guidelines

<p>
After Installation and setup (see below)
</p>

- Create a faculty account update your profile and post projects
- Create a students account and apply to them.


## Setup Guidelines 

- After sucessfull installation create a .env in the directory where ```settings.py``` is located 
- It must have the content as the .env.example file

### Important
- After installation (see below) Create two groups (student and teacher) from the admin panel or shell namely ```student``` and ```teacher```



## Installation Guidelines

1. Install and activate Virtual environment and install requirements by - 
```
pip install -r requirements.txt
```
2. Make the all migrations and run the server
```
python local.py makemigrations
python local.py migrate
python local.py runserver
```

> ### Note Important
> I created ```local.py``` to mirror django's ```manage.py``` and use it for development to know more about it see my <a href="https://stackoverflow.com/questions/68766668/django-best-practice-for-running-switching-dev-debug-product-mode/68766902#68766902"> stack overflow answer. </a>



## Contribution Guidelines 

Any changes are whole heartedly welcome, create an issue to report a bug. Or even better make a pr to fix it. 

> PS : If you use this for ypur project or work please consider starring it.
> Initially this was build to serve as the research portal of NIT Dgp which now is converted to serve as a rest api for an asynchronous frontend and can be found <a href="https://github.com/sa-y-an/rportal1"> here </a>. 

