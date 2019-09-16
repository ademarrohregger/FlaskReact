# FlaskReact

A To Do app made in React (JavaScript) and Flask (Python)

## Commands

### Server

Install [Python](https://wiki.python.org/moin/BeginnersGuide/Download)\
Run `pip install -r server/requirements.txt` to install dependencies.\
You'll need to run `pip freeze > requirements.txt` whenever a new dependency is added\
Run `export FLASK_APP=server/src`and `export FLASK_ENV=development` to set up Flask\
You may run `export FLASK_DEBUG=1` to enable auto reloading\
To initialize the database as configured in `schema.sql`, run `flask init-db`\
Start flask by running `flask run` or `python -m flask run` in case of virtualenv

To Do: change pip to pipenv

### To deploy

`heroku create`\
`git init`\
`git remote add heroku <git>`
`git add .`\
`git commit -m "updating deploy"`\
`git push heroku master`\

(pipenv install ?)\
`pipenv lock`\
Procfile `web: flask init-db & gunicorn app:app`

## References

- [Building a Todo App with Flask in Python](https://stackabuse.com/building-a-todo-app-with-flask-in-python/)
- [Flask's Tutorial](https://flask.palletsprojects.com/en/1.0.x/tutorial/)
