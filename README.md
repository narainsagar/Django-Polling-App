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

Then navigate to http://127.0.0.1:5000 in your browser.

## License

Please read over at [LICENSE](./LICENSE) file.