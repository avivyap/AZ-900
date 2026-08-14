-----
Azure Storage replica automáticamente los datos para garantizar la redundancia 

- Tres copias en una única región (por defecto)
- Seis copias distribuidas en dos regiones emparejadas (opcional)
	- Tres en cada región

Las opciones de redundancia varían según la disponibilidad y el coste

- Zona única
- Varias zonas en una única región
- A través de regiones

### Opciones de redundancia de almacenamiento

Región única

- Almacenamiento con redundancia local (LRS)
- Almacenamiento con redundancia de zona (ZRS)

Múltiples regiones

- Almacenamiento con redundancia geográfica (GRS)
- Almacenamiento con redundancia de zona geográfica (GZRS)

Todas las opciones incluyen:

- Tres copias en la región primaria

- Tres copias en la región secundaria (para opciones de múltiples regiones)

#### LRS

Podemos crear automáticamente tres copias en la región primaria para garantizar su durabilidad

Todo el almacenamiento y replicación se realiza dentro de una única región, sin distribución geográfica

Al ser local, no ofrece protección contra interrupciones de zona o regionales

![[Pasted image 20260707120536.png]]


#### ZRS

A diferencia del LRS, el ZRS replica datos en diferentes zonas de disponibilidad dentro de una misma región, aumentando la durabilidad y disponibilidad

Al igual que el LRS, mantiene tres copias de los datos, pero están distribuidas en diferentes zonas

Esta diseñado para salvaguardar los datos incluso si una zona completa enfrenta problemas, lo que lo hace mas resistente a interrupciones que el LRS

ZRS es mas caro que el LRS, por la replicación entre zonas

ZRS no protege contra eventos catastróficos que puedan afectar a una región completa 

![[Pasted image 20260707120521.png]]

#### GRS

GRS replica datos en diferentes centros de datos en regiones geográficamente separadas, protegiendo contra desastres regionales 

Mientras tres copias en la región primaria y tres copias adicionales en una región secundaria 

En caso de un fallo o desastre en la región primaria, los datos pueden ser accedidos desde la región secundaria, garantizando una alta disponibilidad 

GRS tiene un coste mayor a ZRS y LRS

![[Pasted image 20260707120506.png]]

#### GZRS 

Combina características de ZRS y GRS 

- Tres copias de datos distribuidas en diferentes zonas de disponibilidad en la región primaria (ZRS)

- Tres copias adicionales en una región secundaria (LRS)

Diseñado para garantizar la disponibilidad de datos incluso si una zona completa o incluso una región entera enfrenta problemas 

GZRS es mas caro que las opciones ZRS y GRS por separado 

![[Pasted image 20260707120548.png]]

### DEMO

Vamos a ver como podemos de forma practica elegir la opción que queramos de redundancia 

![[Pasted image 20260707122942.png]]


