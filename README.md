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
