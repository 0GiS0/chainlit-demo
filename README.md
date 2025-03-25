# Demo de MCP Servers con Chainlit

¡Hola developer 👋🏻! En este repo puedes encontrar un entorno donde probar MCP Servers usando Chainlit. Lo único que debes hacer es añadir las credenciales de tu modelo en Azure Open AI en el archivo `.azure.env`:

Este repo funciona con Dev Containers así que no necesitas instalar nada en tu máquina local. Solo abre el repo en VSCode y selecciona la opción de abrir en contenedor.

Una vez que ya lo tengas ejecutandose, añade las credenciales de tu modelo en Azure Open AI en el archivo `.azure.env`:

```
AZURE_OPENAI_API_KEY=
AZURE_OPENAI_ENDPOINT=
OPENAI_API_VERSION=
AZURE_OPENAI_MODEL=
```

y ejecuta el siguiente comando para lanzar tu aplicación con Chainlit:


```bash
chainlit run app.py -w
```

Ahora verás que como parte del chat tienes un icono que te permite añadir servidores MCP:

![MCP Servers Icon](images/Añadir%20MCP%20servers%20en%20Chainlit.png)

Y puedes añadir algunos ejemplos, como el de filesystem;

![MCP Servers Icon](images/Configuración%20del%20MCP%20Server%20Filesystem.png)

Con el nombre Filesystem y este es el comando a ejecutar:

````
npx -y @modelcontextprotocol/server-filesystem /workspaces/chainlit-demo
````

Y la configuración quedaría algo así:

![MCP Servers Icon](images/MCP%20Server%20conectado.png)

Preguntarle algo as:

```
Puedes crearme un poema sobre la primavera en un archivo llamado poema.txt
```

Y el resultado sería como el siguiente:

¡Nos vemos 👋🏻!