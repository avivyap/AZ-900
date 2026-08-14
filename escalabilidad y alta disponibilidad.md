-----
## Escalabilidad

La escalabilidad significa que una aplicación/sistema puede manejar mayores cargas adaptándose

Hay dos tipos de escalabilidad:

- Escalabilidad vertical 
- Escalabilidad horizontal 

### Escalado vertical

Desplegar la aplicación/base de datos en una instancia mayor:

- Un disco duro más grande
- Una CPU más rápida
- Más RAM,CPU o capacidades de red 

Es decir que podemos aumentar las características de la VM

Requiere de un periodo de inactividad

### Escalado horizontal

Despliegue de múltiples instancias de aplicación/base de datos

- Escalado vertical tiene limites, este no 
- Escalado vertical puede ser caro 
- Escalado horizontal aumenta la disponibilidad

En el escalado horizontal necesita infraestructura adicional:

- Conjuntos de escalado, balanceadores de cargar, etc.

**NO** requiere de un periodo de inactividad
### Escalabilidad vs Elasticidad vs Agilidad

Escalabilidad: capacidad de acomodar una mayor carga reforzando el hardware o añadiendo nodos

Elasticidad: una vez que el sistema es escalable, la elasticidad significa que habrá cierto "autoescalado" para que el sistema pueda escalar en función de la carga 

Agilidad: (no relacionado con escalabilidad) los nuevos recursos de IT están a un clic de distancia, lo que significa que se reduce el tiempo para poner esos recursos a disposición de los desarrolladores de semanas a sólo minutos

## Alta disponibilidad 

La alta disponibilidad suele ir de la mano del escalado horizontal 

Alta disponibilidad significa ejecutar la aplicación / sistema en al menos 2 zonas de disponibilidad 

El objetivo de la alta disponibilidad es sobrevivir a la pérdida del centro de datos 

**SLA** (Service Level Agreement) es el compromiso del proveedor sobre el tiempo que el servicio estará disponible

## Conjunto de disponibilidad

Un conjunto de disponibilidad (Availability Set) es un recurso de Azure que sirve para que varias máquinas virtuales no fallen al mismo tiempo cuando ocurre un problema dentro de un mismo centro de datos.

------
### Ejemplos 

Escalado vertical: Aumentar el tamaño de la instancia (= escalar hacia arriba)

- Desde 0.5G de RAM, 1 vCPU
- Hasta: 11.4TB de RAM, 416 vCPUs

Escalado horizontal: Aumentar el número de instancias (= escalado hacia fuera / hacia dentro)

- Conjuntos de escalado (VM Scale Sets)
- Balanceador de carga (Azure Load Balancer)

Alta disponibilidad: Ejecutar instancias para la misma aplicación a través de múltiples AZ 

 - Conjuntos de escalado (VM Scale Sets) Multi AZ
