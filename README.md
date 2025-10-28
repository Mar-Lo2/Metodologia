# Metodologia

En base a las metodologías vistas de los frameworks (NIST,PTES), deberéis hacer un framework de trabajo, con las herramientas que usareis para cada fase, que tipo de información buscar, intentar crear herramientas para algunos casos específicos (automatizar la recepción de información, normalizar información).

**************
*************
# Metodología PTES (Penetration Testing Execution Standard)
- ##### Es un estándar que define un marco de trabajo estructurado en siete fases, centrado en realizar pruebas de penetración, para la evaluación de sistemas informáticos.


# Metodología NIST (National Institute of Standards an Technology)
- ##### Son una Serie de Macros y directrices para la gestión dela ciberseguridad y seguridad de la información.

- ###### Fases PTES ↔ NIST 2.0
	- ### 1. Interacciones Iniciales ↔ Gobernar
		- **Objetivo:** 
			- Definir los objetivos, reglas de compromiso, alcance y permisos de la prueba
		- **Información a buscar:**
			- En esta parte no es tanto la información que se va a buscar sino la información/pasos a seguir que se establece con la empresa.
				- ¿Cuál es el objetivo?
				- ¿Qué tipos de actividades se pueden realizar dependiendo de la infraestructura?
				- ¿Hay alguna infraestructura critica sobre la que no se pueda realizar ninguna operación?
				- Horarios disponibles para la intervención y tiempos establecidos para las investigaciones.
				- Firma de contratos.
		- **Entregables:**
			- Alcance de la Investigación.
			- Estructura de reportes según necesidad.
			- Contratos.
		- **Herramientas:**
			- **Adobe Acrobat**, para mandar contratos y estructura de reportes.
			- **Excel**, para la organización de horarios.
			- **Power Point / Canvas / Derivados** Para mostrar mas intuitivamente la explicación del alcance.
			- **Proton Mail:** Para la comunicación con el cliente sin involucrar correos empresariales.
	- ### 2. Recopilación de información ↔ Identificar
		- **Objetivo:** 
			- Recopilar la máxima cantidad de información sobre el objetivo, existen dos tipos de recopilación en esta fase.
				- Activa
				- Pasiva
		- **Información a buscar:**
			- Activos de la empresa
				- Dispositivos
				- Usuarios
					- Locales
					- Dominio
				- Correos
				- Aplicaciones utilizadas y versiones
			- Estructura de red
				- Número de dispositivos reconocidos
				- Marcas Utilizadas
			- Contraseñas que se mandan en texto plano
		- **Entregables:**
			- Lista de Activos
			- Lista de correos, cuentas apps.
			- División de Superficies de ataque según criterios establecidos
		- **Herramientas:**
			- Recon-NG
			- Shodan
			- Burpsuite
			- OWASP ZAP
			- Nuclei
			- The Harvester
	- ### 3. Modelado de amenazas ↔ Proteger & Identificar
		- **Objetivo:** 
			- Se analiza la información para identificar activos críticos y posibles amenazas.
		- **Información a buscar:**
			- Amenazas en activos
			- Malas optimizaciones que puedan suponer amenazas
			- Exploits de aplicaciones en la empresa con versiones antiguas.
		- **Entregables:**
			- Diagrama e Informe de Amenazas identificadas.
		- **Herramientas:**
			- MITRE ATT&CK Navigator
			- Metasploit
			- OWASP ZAP
	- ### 4. Análisis de vulnerabilidades ↔ Detectar
		- **Objetivo:** 
			- Se analiza la información recopilada y se localizan vulnerabilidades, vectores y posibles puntos de entrada a los activos críticos.
		- **Información a buscar:**
			- A partir de la información analizada en el anterior paso, localizar técnicas, que muestren esa vulnerabilidad y como explotarla. 
		- **Entregables:**
			- Informe con las Vulnerabilidades, sus respectivos exploits y la amenaza que suponen
		- **Herramientas:**
			- Qualys
			- Nmap
			- OpenVAS
			- Nessus
	- ### 5. Explotación ↔ Detectar & Responder
		- **Objetivo:** 
			- Se procede a probar técnicas de explotación en las vulnerabilidades identificadas en el sistema para ver que tipos de accesos se pueden obtener
		- **Ejecución:**
			- Después de haber, analizado toda la información anterior, realizar pruebas para verificar que la información analizada es una vulnerabilidad y se pueden realizar las técnicas de explotación realizadas. 
		- **Entregables:**
			- Lista de las vulnerabilidades detectadas anteriormente.
			- Respectivo informe de cada una de las vulnerabilidades que se han logrado explotar
		- **Herramientas:**
			- Metasploit
			- Burp Suite
			- Sliver
			- Cobalt Strike
			- CrackMapExec
	- ### 6. Post-explotación ↔ Responder
		- **Objetivo:**
			- Se intenta escalar un usuario normal hasta administrador y obtener persistencia. Posteriormente se evalúa el impacto del acceso obtenido, datos sensibles y movimientos laterales.
		- **Entregables:**
			- Análisis del impacto
			- Validación de persistencia
		- **Herramientas:**
			- Mimikatz
			- Pupy
			- winPEAS / linPEAS
			- BloodHound / SharpHound
	- ### 7. Generación de informe ↔ Recuperar
		- **Objetivo:**
			- Documentar hallazgos, vulnerabilidades, exploits exitosos, impacto y recomendaciones de mitigación.
		- **Información a buscar:**
			- Recopilar toda la información anterior y explicarla de forma extensa y clara.
				- Explicación del impacto que se podría haber causado en un ataque real.
				- Limitaciones o métodos de defensa que estén funcionando correctamente
			- Además hay que buscar y recomendar posibles soluciones a exploits que se hayan realizado exitosamente o a deficiencias en la estructura de seguridad de red..
		- **Entregables:**
			- Informe Final
			- Buenas prácticas
			- Defensas actuales que funcionan correctamente
			- Defensas actuales con deficiencias
		- **Herramientas:**
			- Reportes plantillas de Qualys
			- Power Bi
			- Grafana
			- Click Up
			- Share Point
			- Adobe/Word/Power Point
			- Elastic


MarLo
