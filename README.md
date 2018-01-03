### First Steps

```sh
$ pyvenv-3.5 env
$ source env/bin/activate
$ pip install -r requirements.txt
```

### Set up Migrations

```sh
$ python manage.py db init
$ python manage.py db migrate
$ python manage.py db upgrade
```

### Run

Run each in a different terminal window...

```sh
# redis
$ redis server

# worker process
$ python worker.py

# the app
$ python app.py or python manage.py runserver
```


### Run-heroku
  swith to env
  export APP_SETTINGS="config.DevelopmentConfig"
  export DATABASE_URL="postgres://sid:sid12345@localhost:5432/test_dev"
