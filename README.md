��#� �z�o�o�s�a�r�l�
�
�

Backend

Installer PostgreSQL
Configurer la source de donnees dans application.yml.
cd backend.
Run mvn install.
Run mvn spring-boot:run.
Spring Boot vas import automatiquement les donnees par defaut contenue dans import.sql .
Le server backend tourne sur localhost:8080.

Frontend
Installer Node.js , npm et Angular Cli
cd frontend.
Run npm install.
Run ng serve
Le frontend tourne  sur localhost:4200.

Flask
Installer Python3
cd flask
python3 -m pip install --user pipx
python3 -m pipx ensurepath
pipx install pipenv
pipenv install --dev
pipevn shell
pipenv graph
set FLASK_APP=app.py
set FLASK_ENV=development
set FLASK_RUN_PORT=9000
export FLASK_DEBUG=1
flask run
L'api flask tourne sur localhost:9000.

NB: L'API du backend en cas de changment d'url se configure dans le fichier src/environments/environment.ts du  frontend  a fin d'eviter les erreur de CORS du la security du content policy implenete au sein des navigateur web. La valeur par defaut de url de cette APi est  localhost:8080/api.
