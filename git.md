
# Ordres git

**git clone <URL_o_RUTA_repositori>**

Permet clonar un repositori remot a partir de la seua URL o ruta.
Per defecte se mostra la rama principal del repositori remot.
Quan clonen un repositori remot apareix un remot en
el repositori local amb el nom d'origin.


**git remote -v**

Permet vore tots els remots configurats al repositori local.


**git remote add <NOM_REMOT> <URL_o_RUTA_repositori>**

Permet afegir un repositori remot


**git remote rm <NOM_REMOT>**

Esborrar un repositori remot


**git remote rename <NOM_REMOT> <NOU_NOM>**

Renombrar un repositori remot


**git fetch <NOM_REMOT>**

Permet actualitzar la informació dels repositoris remots.
git es connecta, comprova que hi ha canvis, els descarrega i actualitza
els punters de les branques remotes però no actualitza les branques locals. 

Per incorporar els canvis cal fer un git merge.
Les branques remotes són sempre de lectura i fan referència
a la informació que té git al repositori.


**git pull <NOM_REMOT> <NOM_BRANCA>**

Esta acció és equivalent a fer un fetch i un merge al mateix temps.
És una de les operacions més habituals quan es sincronitzen
canvis amb el repositori. Normalment les branques locals i
remotes tindran el mateix nom, encara que podrem
referenciar a una branca concreta amb <NOM_REMOT>/<NOM_BRANCA>


**git push <NOM_REMOT> <NOM_BRANCA>**

Esta acció envia els canvis locals d'una branca al repositori remot.
És l'acció inversa al pull. Normalment les branques locals
i remotes tindran el mateix nom. Si no fiquem el paràmetre
del nom de la branca el que fa és utilitzar la branca activa
i la sincronitza amb la del mateix nom al repositori remot.


**git checkout <NOM_BRANCA>**

Per defecte l'única branca que es descarrega del repositori és
la principal (normalment master o main). Si volem descarregar en
local altra branca només hem de fer un checkout a la branca remota
i git s'encarregarà de fer la descarrega.


**git push -u <NOM_REMOT> <NOM_BRANCA>**

Si hem creat una branca que no existeix al repositori remot i volem
sincronitzar-la al repositori hem d'utilitzar el git push amb el
paràmetre -u. Recorda que la branca activa ha de ser la branca a sincronitzar.


