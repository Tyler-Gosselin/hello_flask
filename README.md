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
## Database Setup

- If you need to setup your database do the following inside python repl while in your pipenv shell
- You will get a warning but it is ok as long as there is no Error

```
>>> from fileName import db
>>> db.create_all()

```

## Routes

### GET ALL GUIDES
- url: localhost:5000/guides

### GET SINGLE GUIDE
- url: localhost:5000/guides/ID

### POST
- url: localhost:5000/guide
```json
body: {
	"title": "New York Pizza",
	"content": "$12"
}
```

### PUT
- url: localhost:5000/guide/ID
```json
body: {
	"title": "New York Pizza",
	"content": "$12"
}
```

### DELETE
- url: localhost:5000/guide/ID

## Dependencies

- Flask
  - https://flask.palletsprojects.com/en/1.1.x/
- Flask SQLAlchemy
  - https://flask-sqlalchemy.palletsprojects.com/en/2.x/
- Flask Marshmallow
  - https://flask-marshmallow.readthedocs.io/en/latest/
- Marshmallow-sqlalchemy
  - https://marshmallow-sqlalchemy.readthedocs.io/en/latest/


## Fix Import Warnings
> With `VSCode` and `Pylance` you might need the following settings in order to let your `linter` and `code editor` know about your environment.
> Easiest way is to make sure you have `vscode` open into the current projects root directory.  For instance this projects `root` is `hello_flask`.  Once you have that open click on the `python` button on the bottom left of `vscode`.  This should pull up a menu that lets you choose which `python` you want to use, pick the one that is located in your `virtualenvironment`.  This should make a `.vscode/settings.json` file.
>If the first portion didn't work you can try this.  Hop into your `pipenv shell` and copy the `path` where your `virtualenv` is located and apply it to a `.vscode/settings.json` file in the root of the project.
```json
{
  "python.pythonPath": "/YOUR_VIRTUALENV_PATH/bin/python3"
}
```

