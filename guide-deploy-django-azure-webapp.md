

## Running app locally

```bash

#Créez une valeur SECRET_KEY pour votre application en exécutant la commande suivante à l’invite du terminal : 
python -c 'import secrets; print(secrets.token_hex())'


# create virtual environment
python3.9 -m venv .envazurewebapp

# activate virtual environment
source .envazurewebapp/bin/activate

# copy environment variables from sample file to .env file
cp .env.sample .env






# Installez les dépendances :
pip install -r requirements.txt

# Run database migration
python manage.py migrate
# Run the app at http://127.0.0.1:8000
python manage.py runserver

