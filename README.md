# Django-pollio-app

`Django pollio app` is a full featured polling app. You have to register in this app to show the polls and to vote. If you already voted you can not vote again. Only the owner of a poll can add poll , edit poll, update poll, delete poll , add choice, update choice, delete choice and end a poll. If a poll is ended it can not be voted. Ended poll only shows user the final result of the poll. There is a search option for polls. Also user can filter polls by name, publish date, and by number of voted. Pagination will work even after applying filter.

## Getting Started

These instructions will get you a copy of the project up and running on your local machine for development and testing purposes.

## Prerequisites

<code>python== 3.9.1 or up and django==4.2.1 or up</code>

## Installing

> git clone or simply download this code:

```bash
https://github.com/narainsagar/Django-pollio-app.git
```

> following steps will setup the project on your machine.

```bash
### Create and Activate the Virtual enviornment
$ python -m venv .venv
$ source .venv/bin/activate

### install the project dependencies
$ pip install -r requirements.txt
```

> To migrate the database open terminal in project directory and type
```bash
$ python manage.py makemigrations
$ python manage.py migrate
```

> To use admin panel you need to create superuser using this command.

`$ python manage.py createsuperuser`

> To Create some dummy text data for your app follow the step below:

```bash
$ pip install faker
$ python manage.py shell
import seeder
seeder.seed_all(10) # Here 10 is a number of entry. You can use it as your own
```

> To run the program in local server use the following command.
```bash
$ python manage.py runserver 5000
```

Then navigate to http://127.0.0.1:5000 in your browser or checkout the Demo snapshots as below.

## Demo

<h2>Project snapshot</h2>
<h3>Home page</h3>
<div align="center">
    <img src="https://user-images.githubusercontent.com/19981097/51409444-0e40a600-1b8c-11e9-9ab0-27d759db8973.jpg" width="100%"</img> 
</div>

<h3>Login Page</h3>
<div align="center">
    <img src="https://user-images.githubusercontent.com/19981097/51409509-36c8a000-1b8c-11e9-845a-65b49262aa53.png" width="100%"</img> 
</div>

<h3>Registration Page</h3>
<div align="center">
    <img src="https://user-images.githubusercontent.com/19981097/51409562-5cee4000-1b8c-11e9-82f6-1aa2df159528.png" width="100%"</img> 
</div>

<h3>Poll List Page</h3>
<div align="center">
    <img src="https://user-images.githubusercontent.com/19981097/51409728-d423d400-1b8c-11e9-8903-4c08ba64512e.png" width="100%"</img> 
</div>

<h3>Poll Add Page</h3>
<div align="center">
    <img src="https://user-images.githubusercontent.com/19981097/51409796-fe759180-1b8c-11e9-941b-c1202956cca4.png" width="100%"</img> 
</div>

<h3>Polling page</h3>
<div align="center">
    <img src="https://user-images.githubusercontent.com/19981097/51409843-1e0cba00-1b8d-11e9-9109-cceb79a6a623.png" width="100%"</img> 
</div>

<h3>Poll Result Page</h3>
<div align="center">
    <img src="https://user-images.githubusercontent.com/19981097/51409932-60ce9200-1b8d-11e9-9c83-c59ba498ca8b.png" width="100%"</img> 
</div>

<h3>Poll Edit Page</h3>
<div align="center">
    <img src="https://user-images.githubusercontent.com/19981097/51410008-92dff400-1b8d-11e9-8172-c228e4b60e28.png" width="100%"</img> 
</div>

<h3>Choice Update Delete Page</h3>
<div align="center">
    <img src="https://user-images.githubusercontent.com/19981097/51410442-dc7d0e80-1b8e-11e9-8f8e-18e6d7bb70fb.png" width="100%"</img> 
</div>

## License

Please read over at [LICENSE](./LICENSE) file.