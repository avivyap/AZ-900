------
Conectar dos VNet, de forma privada utilizando la red de Azure 

![[Pasted image 20260712112837.png]]

Si entre dos VNet tenemos subredes que se superponen encima de la otra, estas dos VNet no vamos a poder emparejarlas con peering

![[Pasted image 20260712113007.png]]

------
### DEMO

Para poder emparejarlos lo que vamos a hacer es irnos a una de las redes y en "Configuración" darle a lo siguiente 

![[Pasted image 20260712113301.png]]

Y dentro de emparejamientos podremos realizar esta acción

![[Pasted image 20260712113435.png]]

Para que el emparejamiento se bidireccional hay que añadir esto

![[Pasted image 20260712113634.png]]

(Esta captura es dentro de lo de arriba, el proceso como tal solo se hace en una red)