# Python Tutorial for Flask

> This is a tutorial I went through while attending the Bottega course

## Start the Server
- Run the following commands in the terminal while in the 'hello_flask' folder/
```
$ pipenv shell
(hello_flask) python app.py
```

- If you get an error saying it doesnt know about a package, you might need to install the packages, or 
you may not be in your 'pipen shell'
```
$ pipenv shell
(hello_flask) pipenv install
(hello_flask) pipenv app.py
```

## Dependencies

- Flask
  - https://flask.palletsprojects.com/en/1.1.x/
- Flask SQLAlchemy
  - https://flask-sqlalchemy.palletsprojects.com/en/2.x/
- Flask Marshmallow
  - https://flask-marshmallow.readthedocs.io/en/latest/
- Marshmallow-sqlalchemy
  - https://marshmallow-sqlalchemy.readthedocs.io/en/latest/
