# Exercici 1


## Creació i actualització de repositoris

## Part 1

**1. Crea un repositori nou amb el nom "llubre" i mostrar el seu contingut**


***Creem un repositori nou amb el nom "llibre"***

  git init llibre
  
***Entrem al directori del repositori***

cd llibre

***Mostrem el contigut del repositori***

ls

**2. Configura GIT  definint el nom d'usuari, correu electronic i activar l'eixida en color. Mostrar la configuració final.**

***Configurem Git: definim el nou usuari, correu electronic i activen els colors***

git config-global user.name "Javier Cornejo"
git config-global user.email "cornejolealjavier@gmail.com"
git config-global color.ui true

***Mostrem la configuració final***

fit config-list


## Part 2


**1. Comprova l'estat del repositori**

git status


**2. Crea un fitxer index.txt amb el següent**

echo "Contingut del fitxer" > index.txt

**3. Comprova de nou l'estat del repositori**

git status

**4. Afegeix el fitxer a la zona d'intercanvi temporal**

git add index.txt


**5. Tornar a comprovar una vegada més l'estat del repositori**

git status

## Part 3


**1. Realitza un commit dels ultims canvis amb el missatge "Afegit index del llibre". I veure l'estat del repositori**

git commit -m "Afegit index del llibre"

git status


## Part 4


**1. Canvia el fitxer index.txt perquè continga el següent**

echo "Nou contingut del fitxer" > index.txt

**2. Mostra els canvis respecte a l'ultima versió guardada al repositori**

git diff

**3. Fer un commit dels canvis amb el missatge "Afegit capitol 3 sobre gestió de branques"**

git commit -m "Afegit capitol 3 sobre gestió de branques"

## Part 5


**1. Mostrar els canvis de l'ultima versio del repositori respecte a l'anterior**

git log-p

**2. Canviar el missatge de l'ultim commit a "Afegit capitol 3 sobre gestio de branques a l'index"**

git commit-amend-m "Afegit capitol 3 sobre gestió de branques a l'index"

**3. Tornar a mostrar els ultims canvis del repositori**

git log -p

## Part 6


**1. Indica a git que vols ignorar tots els fitxer que comencen per "daw", tots els que tenen l'extensio out i les imatges (jpg,png,bmp i gif)**

***Crea o edita el ftxer .gitignore amb les regles d'ignorar***

echo "daw*" >> .gitignore
echo "*.out" >> .gitignore
echo "*.jpg" >> .gitignore
echo "*.png" >> .gitignore
echo "*.bmp" >> .gitignore
echo "*.gif" >> .gitignore

***Afegeix el fitxer .gitignore a la zona d'inercanvi temporal***

git add .gitignore


***Realitza un commit amb els canvis a l'arxiu .gitignore***


git commit-m "Afegit regles d'ignorar a .gitignore"





