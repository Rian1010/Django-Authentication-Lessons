## Acivating a Virtual Environment
- python3 -m venv myvenv
- virtualenv venv
- virtualenv venv --system-site-packages
- source venv/bin/activate

## Deactivation a Virtual Environment
- deactivate

## Reactivating a Virtual Environment 
- source venv/bin/activate

## Uninstall Packages
- sudo pip3 uninstall ______packagename______

## Starting Off With Django
- sudo pip3 install django==1.11.24
- django-admin startproject django_auth .
- django-admin startapp accounts
- python3 manage.py runserver


## If Migration Is Required:
- python manage.py makemigrations
- python manage.py migrate

## Get Aliases (Not important, so it is okay, if it does not work)
- nano ~/.bashrc (to get to the bashrc on VSCode, but for this part use settings.json on VSCodeas shown at the very bottom of the README.md file)
- alias run = "python3 manage.py runserver" (does not apply for vscode)
- Then press "Ctrl + X" to save, "Y" for yes, and then press the <enter> button
- Run the page using 'run' in the terminal

## Extra Notes:

### Reset git add
- git reset
### Get all in the venv
- pip3 list

## Next Step
- In settings.py, add "accounts" in INSTALLED_APPS 
- In settings.py, add:
```python
 ALLOWED_HOSTS = ['localhost', '127.0.0.1',
                os.environ.get('HOSTNAME')]
```
- python manage.py migrate
- python3 manage.py createsuperuser

- Make a templates folder with the index.html content
- views.py (return render(request, "todo-list.html"))
- urls.py

## Admin

### SQLite3
- sqlite db.sqlite3

### Check content
- select * from django_migrations;
- .quit