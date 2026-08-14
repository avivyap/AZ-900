---------
Microsoft Entra Domain Services proporciona servicios de dominio administrados ( unión a un dominio, directiva de grupo, LDAP y autenticación Kerberos/NTLM) sin necesidad de implementar o mantener controladores de dominio en la nube.
### ¿Como funciona?

Cuando cree un dominio administrado de Microsoft Entra Domain Services, defina un espacio de nombres único. 

Este 'namespace' es el nombre de dominio

No es necesario administrar, configurar ni actualizar estos controladores de dominio.

### ¿La información está sincronizada?

	Active Directory (local)
          │
          │ Microsoft Entra Connect
          ▼
	Microsoft Entra ID
	          │
          │ Sincronización automática
          ▼
	Microsoft Entra Domain Services


![[Pasted image 20260630113252.png]]