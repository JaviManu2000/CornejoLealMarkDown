# Exercici 2


## Creació i actualització de repositoris

## Part 1

**1. Mostra l’historial de canvis del repositori**

git log

**2. Crea la carpeta capitols i dins d’ella crea el fitxer capitol1.txt amb el següent text:**

mkdir capitols
echo "Git es un sistema de control de versions ideat per Linus Torvalds" > capitols/capitol1.txt

**3. Afegeix els canvis a la zona d'intercanvi i temporal.**

git add capitols/capitol1.txt

**4. Fes un commit dels canvis amb el missatge "Afegit capitol 1"**

git commit -m "Afegit capitol 1."

**5. Torna a mostrar l'historial de canvis del repositori.**

git log

## Part 2


**1. Crea el fitxer capitol2.txt a la carpeta capitols amb el seguent text**

git commit -m "capitol2/capitol.txt"

**2. Afegeix els canvis a la carpeta capitols amb el seguent text**

git add capitols/capitol2.txt

**3. Fes un commit dels canvis amb el missatge "Afegit capitol 2"**

git commit -m "Afegit capitol 2."

**4. Mostra les diferencies entre l'ultima versio i les dues versions anteriors**

git diff HEAD HEAD~1
git diff HEAD~1 HEAD~2

## Part 3


**1. Crea el fitxer capitol3.txt a la carpeta capitols amb el seguent text**

echo «text a posar» > capitols/capitol3.txt

**2. Afegeix els canvis a la zona d’intercanvi temporal**

git add capitols/capitol3.txt

**3. Fes un commit dels canvis amb el missatge "Afegit capitol 3"**

git commit -m «Afegit capitol 3.»

**4. Mostra les diferencies entre la primera i l'ultima versio del repositori**

git diff $(git rev-list –max-parents=0 HEAD) HEAD
 
## Part 4


**1. Afegir al final del fitxer index.txt la següent linia**

echo "Capitol 5: Conceptes avançats" >> index.txt

**2. Afegir els canvis a la zona d’intercanvi temporal**

git add index.txt

**3. Fer un commit dels canvis amb el missatge "Afegit capitol 5 a l’index"**

git commit -m «Afegit captol 5 a l’index»

**4. Mostrar qui ha fet canvis sobre el fitxer index.txt"**

git blame index.txt

**4. Mostrar qui ha fet canvis sobre el fitxer index.txt**



