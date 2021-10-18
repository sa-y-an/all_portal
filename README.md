# All Portal

A simple portal for posting and applying made possible by django. Supports all databases supported by django. 
Currently uses - 
1. postgress in deployment (```manage.py```)
2. sqlite in development (```local.py```)

## Use Cases 

<p>
Can be easily modified to be used in any place where one user group posts a project or job and another user group applies to it. 
</p>

<u>Common use cases - </u>
- College's **Research portal** where teacher can post a project and student can apply
- **Jobs Portal** - Companies posts jobs and user applies 
- **e-commerce app** - Vendors Posts about items and prices and customer buys them ( in that case a payment gateway needs to be integrated )

### Live Demo

A live demo can be seen at <a href="https://allportal.herokuapp.com/">https://allportal.herokuapp.com/</a>
> PS: Give some time for the site to load ( The Heroku containers might be restarting after a long hibernation XD )

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
> I know it creates some duplicate code and can be a bad practise, but since it simplifies things i go with it XD.
> Furthermore, currently I make a third file where I store the common code and inhereit from there, I will update this repo as well wherever I get time.


## License 

- This is a starware ⭐, which means you can use this code as long as you star this repo.
