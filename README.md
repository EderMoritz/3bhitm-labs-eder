# 3bhitm-labs-eder

# hallo edit

# Hallo


Neuen Ordner für das Repo erstellen

mkdir 3bhitm-labs-eder
cd 3bhitm-labs-eder/

Befehle von Github ausführen:

Readme wird erstellt
echo "# 3bhitm-labs-eder" >> README.md

Repo wird initialisiert
git init

Readme kommt von der woking copy in die staging area
git add README.md

Readme wird von der staging area auf das lokale Repo commited
git commit -m "first commit"

Main Branch wird erstellt
git branch -M main

Repo wird hinzugefügt
git remote add origin https://github.com/EderMoritz/3bhitm-labs-eder.git

Alles vom lokalen Repo kommt nun auf das richtige Repo
git push origin main

Im Homeverzeichnis wird im .ssh Ordner zwei Files erstellt: id_rsa, id_rsa.pub
cd 
ssh-keygen -t rsa
cd .ssh 
gedit id_rsa.pub *public key kopieren*

Auf dem Github Repo rechts oben klicken -> Settings -> SSH and GPG keys -> new SSH key -> title: moritz, key: *public key einfügen* -> add SSH key

Einen playground Ordner erstellen für eine bessere Übersicht und für kein Durcheinander bei den Repos
cd
cd ITP
mkdir playground
cd playground/

Zurück auf Github Repo unter grüne Code Box SSH key kopieren und klonen -> yes eingeben (enter funktioniert nicht!)
git clone git@github.com:EderMoritz/3bhitm-labs-eder.git

Zu Settings auf dem Repo -> Manage Acces -> Collaborator hinzufügen
Collaborator muss auch den git clone ... Befehl ausführen

Readme verändern
cd 3bhitm-labs-eder/
gedit README.md 

Git Status nachsehen und wieder auf Repo pushen
git status
git add README.md 
git commit -m "update readme"
git push

Git pull wenn Collaborator etwas am Readme geändert hat
git pull
