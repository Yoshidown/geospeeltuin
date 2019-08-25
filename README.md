# geospeeltuin
Hobbyprojectje 


Dit is nieuw

Installeren:

pip install virtualenvwrapper
nano ~/.bashrc
In je bashrc file voeg het volgende onderaan toe: 
export WORKON_HOME=$HOME/.virtualenvs                                      
export PROJECT_HOME=$HOME/Devel                                                
source /home/USER/.local/bin/virtualenvwrapper.sh                                       

mkvirtualenv geospeeltuin                                             
workon (als het goed is staat geospeeltuin nu in de lijst)                        
(voor de zekerheid sluit je terminal en open een nieuwe en probeer nu workon geospeeltuin, je zit nu in je virtualenv)


sudo apt install python3-pip python3-dev libpq-dev postgresql postgresql-contrib nginx curl

sudo su postgres 
psql
(vervang username met je usernaam)
\connect template1;
CREATE EXTENSION postgis;
CREATE EXTENSION hstore;
CREATE DATABASE geospeeltuin_development;
CREATE ROLE username WITH LOGIN;
ALTER USER username CREATEDB;
\connect geospeeltuin_development;
CREATE EXTENSION postgis;
CREATE EXTENSION hstore;
ALTER DATABASE geospeeltuin_development OWNER TO username;
\q
