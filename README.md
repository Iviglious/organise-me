# Organise Me app

Easy and qick way to orginise your life.

## Functionality

- Sign In
    - via username & password
    - via email & password
    - via email or username & password
- Sign Up
- Log Out
- Profile Activation via Email
- Password Reset
- Re-send Activation Code
- Password Changing
- Email Changing
- Profile Data Changing
- Multilingual: Ukrainian, Russian, Spanish, French, Simplified Chinese, and German languages


## Installing

### Clone the project

```
git clone https://github.com/iviglious/organise-me
cd organise-me
```

### Install dependencies & activate virtualenv

```
pip install pipenv

pipenv install
pipenv shell
```

### Configure the settings (connection to the database, connection to an SMTP server, and other options)

1. Edit `source/app/conf/development/settings.py` if you want to develop the project.

2. Edit `source/app/conf/production/settings.py` if you want to run the project in production.

### Apply migrations

```
python source/manage.py migrate
```

### Collect static files (only on a production server)

```
python source/manage.py collectstatic
```

### Running

#### A development server

Just run this command:

```
python source/manage.py runserver
or
./start.sh
```

