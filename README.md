Installation de Django
créer un virtualenv appelé Nomenv :
python3 -m venv Nomenv
Démarrez votre environnement virtuel en exécutant :
source Nomenv/bin/activate
Maintenant que vous avez activé votre virtualenv, vous pouvez
installer Django
python -m pip install --upgrade pip
Après vous crée un fichier requirements.txt, dans ce
fichier vous copié < Django~=2.2.4 >
Maintenant, exécutez pip install -r requirements.txt pour
installer Django.
python -m pip install -U --force-reinstall pip
Pour création d’un Projet, N'oubliez pas le point .à la
fin ! Très important le point à la fin.
django-admin startproject mysite .
pour voir la hierarchie de django :
django-admin
Configuration de la base de données
python manage.py migrate
Notre nom d’hôte sur PythonAnywhere ne sera donc pas accepté
une fois que notre application sera déployée. Pour éviter cela, nous
allons changer le paramètre suivant :
mysite/settings.py
ALLOWED_HOSTS = ['127.0.0.1', '.pythonanywhere.com']
lancer le server
python manage.py runserver
http://127.0.0.1:8000/
