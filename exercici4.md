# Exercici 4


## Creació i actualització de repositoris

## Part 1

**1. Crea una nova branca bibliografia i mostra les branques del repositori**

git branch bibliografia
git checkout bibliografia
git switch bibliografia
git branch

## Part 2


**1. Crear el fitxer capitols/capitol4.txt afegir el següent text**

git branch bibliografia
git checkout bibliografia
git switch bibliografia
git branch * master

**2.  Afegeix els canvis a la zona d’intercanvi temporal**

git add capitols/capitol4.txt

**3. Fer un commit amb el missatge «Afegit capitol 4»**

git commit -m «Afegit capitol 4»

**4. Mostrar la historia del repositori incloent totes les branques**

git log -all –graph –oneline


## Part 3


**1. Canvia a la branca bibliografia**

git checkout bibliografia

**2. Crea el fitxer bibliografia.txt i afegir la següent referencia**

git switch bibliografia

**3. Afegeix els canvis a la zona d’intercanvi temporal**

echo «text» > bibliografia.txt
git add bibliografia.txt

**4. Fes un commit amb el missatge «Afegida primera referència bibliogràfica»**

git commit -m «Afegida primera referència biliografica»

**5. Mostra la història del repositori incloent totes les branques**

git log –all –graph –oneline
 
## Part 4


**1. Fusiona la branca bibliografia amb la branca master**

# Assegura't d'estar a la branca master abans de fer la fusió
git checkout master

# Fusiona la branca bibliografia amb master
git merge bibliografia

**2. Mostra la historia del repositori incloent totes les branques**

git log --all --graph –oneline

**3. Elimina la branca bibliografia**

git branch -d bibliografia

**4. Mostra de nou la historia del repositori incloent totes les branques"**

git log --all --graph –oneline


## Part 5


**1. Crea la branca bibliografia**

git branch bibliografia

**2. Canvia a la branca bibliografia**

git checkout bibliografia

**3. Canvia el fitxer bibliografia.txt perquè continga les seguents referències**

git switch bibliografia

**4. Afegeix els canvis a la zona d’intercanvi temporal i fer un commit amb el missatge «Afegida nova referència bibliografica»**

echo «text» > bibliografia.txt
echo «text» > > bibliografia.txt
git add bibliografia.txt

**5. Canvia a la branca master**

git checkout master
git smitch master

**6. Canvia el fitxer bibliografia.txt per el següent:**

echo «text» > bibliografia.txt
echo «text» > > bibliografia.txt
 
**7. Afegeix els canvis a la zona d’intercanvi temporal i fer un commit amb el missatge «Afegida nova referència bibliogràfica»**

git add bibliografia.txt
git commit -m «Afegida nova referència bibliogràfica»

**8. Fusiona la branca bibliografia amb la branca master**

git merge bibliografia

**9. Resol el conflicte deixant el fitxer bibliografia.txt amb les referències**


**10. Afegeix els canvis a la zona d’intercanvi temporal i fes un commit amb el missatge «Resolt conflicte de bibliografia»**

git add bibliografia.txt
git commit -m «Resolt conflicte de bibliografia»

**11. Mostra la historia del repositori incloent totes les branques**

git log –all –graph –oneline




