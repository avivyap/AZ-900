-----
Controla tráfico entrante/saliente a recursos Azure mediante reglar permitir/denegar tráfico

Cuando creas una maquina virtual se le crea y asigna automáticamente a su interfaz de red un grupo de seguridad

Un NSG solamente se puede asociar a una subred y a una interfaz de red 

Para poder ver los que tienes disponibles, puedes hacerlo aquí 

![[Pasted image 20260715105023.png]]

### Configuración de reglas

Origen: Define las direcciones IP de origen que están sujetas a esta regla

Intervalo de puertos de origen: Especifica los puertos de origen para el tráfico entrante

Destino: Identifica el recurso de destino 

Servicio: Especifica el protocolo de destino y el intervalo de puertos para esta regla 

Intervalos de puertos de destino: Especifica los puertos de salida para el tráfico saliente 

Protocolo: Protocolo de tráfico (TCP,UDP,ICMP,etc.)

Acción: Determina si el tráfico seleccionado será permitido o denegado 

Prioridad: Número que determina el orden en qué se aplican las reglas ( los números mas bajos tienen una prioridad mas alta )

![[Pasted image 20260712115912.png|509]]


