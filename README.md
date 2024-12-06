Jobsito Egg

Este egg está diseñado para ejecutar aplicaciones Node.js, específicamente el bot Jobsito, en un servidor de Pterodactyl. Permite ejecutar bots con estructuras personalizadas, como tener el archivo principal ubicado en src/index.js.

Requisitos

Panel Pterodactyl versión 1.0 o superior.

Un nodo configurado con Docker compatible.

Imagen de Docker: ghcr.io/parkervcp/yolks:nodejs_21.



---

Configuración

1. Variables

Este egg utiliza las siguientes variables para configurar el servidor:


---

2. Comandos de Inicio

El comando de inicio predeterminado es:

node {{BOT_JS_FILE}}

Esto ejecutará el archivo especificado en la variable BOT_JS_FILE (por defecto, src/index.js).


---

3. Instalación

Durante la instalación, este egg realiza las siguientes tareas:

1. Descarga las dependencias especificadas en package.json utilizando npm install.


2. Si se proporciona un repositorio GitHub en GIT_REPO, clona el proyecto y utiliza la rama especificada en BRANCH.




---

Pasos para Configurar el Egg

Paso 1: Importar el Egg

1. Ve al panel de administración de Pterodactyl.


2. Navega a Nests > Import Egg.


3. Sube el archivo JSON proporcionado (Jobsito-egg.json).



Paso 2: Crear un Servidor

1. Ve a la sección de Servers y selecciona el nest donde importaste el egg.


2. Llena las variables requeridas:

Archivo principal: src/index.js (u otro si aplica).

URL del repositorio y rama (si usas GitHub).

Token de Discord del bot.




Paso 3: Iniciar el Servidor

1. Inicia el servidor desde el panel de Pterodactyl.


2. Verifica los registros de inicio para confirmar que el bot se ejecuta correctamente.




---

Problemas Comunes


---

Créditos

Autor: Austin Morales.

Docker Image: ghcr.io/parkervcp/yolks.

Contacto: undefine.

