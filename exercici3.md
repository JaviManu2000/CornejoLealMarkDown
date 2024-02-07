# Exercici 3


## Creació i actualització de repositoris

## Part 1

**1. Elimina l'ultima linea del fitxer index.txt i guarda-ho**

Podem utilitzar un editor de text com vim, nano o l’editor que es preferisca
Només eliminem l’ultima linea i ho guardem
Ho faré amb nano:
nano index.txt
Guardem amb l’editor apretant Control + O
I després sortim de l’editor amb Control + X

**2. Comprova l’estat del repositori**

git status

**3. Desfés els canvis realitzats al fitxer index.txt per tornar a la versió anterior del fitxer**

git checkout – index.txt

**4. Torna a comprovar l’estat del repositori**

git status

A pesar d’aquest missatge, entram a l’index retorna la línia ques es va borrar abans, i o comprovent utilitzant una altra vegada el commandament nano, per obrir l’editor i on podrem vorer com apareix l’ultima linea.

## Part 2


**1. Elimina l’ultima linea del fitxer index.txt i guarda-ho**



**2.  Afegeix els canvis a la zona d’intercanvi temporal**

git add capitols/capitol2.txt

**3. Comprova de nou l’estat del repositori**

git commit -m "Afegit capitol 2."

**4. Treu els canvis de la zona d’intercanvi temporal, però mantin-los al directori de treball**

git diff HEAD HEAD~1
git diff HEAD~1 HEAD~2

**5. Desfes els canvis realitzats al fitxer index.txt per tornar a la versió anterior del fitxer**

git checkout –index.txt

**6. Torna a comprovar l’estat del repositori**

git status


## Part 3


**1. Elimina l’ultima linia del fitxer index.txt i guarda-ho**

Fem el mateix que els 2 exercicis abans

**2. Elimina el fitxer capitols/capitol3.txt**

rm capitols/capitol3.txt

**3. Afegeix un fitxer nou capitols/capitol4.txt que estiga buit**

touch capitols/capitol4.txt

**4. Afegeix els canvis a la zona d’intercanvi temporal**

git add index.txt capitols/capitol4.txt

**5. Comprova de nou l’estat del repositori**

git status

**6. Treu els canvis de la zona d’intercanvi temporal, però mantin-los al directori de treball**

git reset HEAD index.txt capitols/capitol4.txt

**7. Comprova de nou l’estat del repositori**

git status

**8. Desfes els canvis realitzats per tornar a la versio del repositori**

git checkout – index.txt capitols/capitol4.txt

**9. Torna a comprovar l’estat del repositori**

git status
 
## Part 4


**1. Elimina l’ultima linia del fitxer index.txt i guarda-ho**

fes el mateix que amb les 3 activitats anteriors

**2. Elimina el fitxer capitols/capitol3.txt**

rm capitols/capitol3.txt

**3. Afegeix els canvis a la zona d’intercanvi temporal i fer un commit amb el missatge «Borra accidental»**

git add index.txt capitols/capitol3.txt
git commit -m «Borrat accidental.»

**4. Comprova l’historial del repositori"**

git log

**5. Desfes l’ultim commit, però mantin els canvis anterios al directori de treball i a la zona d’intercanvi temporal**

git reset HEAD

**6. Comprova l’historial i l’estat de repositori**

git log
git status

**7. Torna a fer el commit amb el mateix missatge que abans**

git commit -c ORIG_HEAD

**8. Desfes l’ultim commit i els canvis anterior al directori de treball, tornant a la versio anterior del repositori**

git reset –hard HEAD


**9. Comprova el nou historial i estat del repositori**

git log
git status
