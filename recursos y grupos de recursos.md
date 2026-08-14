--------
Un recurso es el bloque de construcción básico de Azure. Todo lo que cree, aprovisione o implemente es un recurso. Las máquinas virtuales, las redes virtuales, las bases de datos y los servicios de Azure AI son ejemplos de recursos.

##### Jerarquía de azure 

	Grupo de administración
        ↓
	Suscripción
        ↓
	Grupo de recursos
        ↓
	Recurso

#### ¿Que es una suscripción?

Una **suscripción** sirve para dos cosas:

- 💰 **Facturación** (quién paga).
- 🔐 **Control de acceso** (quién puede administrar los recursos).

Piensa en ella como un **contenedor administrativo**.

#### ¿Que hace un Grupo de Administración?

Es un nivel **por encima de las suscripciones**.

Sirve para aplicar políticas a muchas suscripciones de golpe.

Si prohíbes crear VMs fuera de Europa en el grupo de administración...

➡️ **Todas las suscripciones heredan esa política automáticamente.**