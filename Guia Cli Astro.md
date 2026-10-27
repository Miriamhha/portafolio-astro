**Guía del CLI de Astro**

**1. Iniciar el servidor en el puerto 3000 y abrir el navegador**

Ejecutar:

![](comando.png)

**¿Qué hace cada opción?**

- npx: ejecuta el CLI de Astro disponible en el proyecto.
- astro: identifica la herramienta de línea de comandos.
- dev: inicia el servidor de desarrollo.
- --port 3000: establece el puerto 3000.
- --open: abre automáticamente el sitio en el navegador predeterminado.

Aspose.Words.6c74796c-2370-41d3-b8d4-4827c0d8c65f.002.png

![](Aspose.Words.6c74796c-2370-41d3-b8d4-4827c0d8c65f.003.png)


















**2. Acceder al sitio desde el celular usando Wi-Fi**

**IP WIFI PC:** 10.96.12.221

**En terminal**

![](Aspose.Words.6c74796c-2370-41d3-b8d4-4827c0d8c65f.004.png)

**Vista Celular:**

![](Aspose.Words.6c74796c-2370-41d3-b8d4-4827c0d8c65f.005.png)

**3. Ejecutar npx astro info y explicar cada línea**

![](Aspose.Words.6c74796c-2370-41d3-b8d4-4827c0d8c65f.006.png)

|**Línea**|**¿Qué significa?**|
| :-: | :-: |
|Astro |Versión del framework Astro instalado en el proyecto. En nuestro caso 7.4.2|
|Vite|Versión de Vite (8.3.5), herramienta que participa en el servidor de desarrollo y el proceso de compilación.|
|Node|Versión de Node.js (24.22.1) que ejecuta las herramientas del proyecto.|
|System|Sistema operativo y arquitectura del equipo (Windows de 64 bits).|
|Package Manager|Administrador de paquetes utilizado npm|
|Output|Tipo de salida configurado para la compilación, en este caso static|
|Adapter|<p>Adaptador de despliegue configurado, si corresponde. </p><p>La máquina no tiene configurado por eso se muestra none.</p>|
|Integrations|<p>Integraciones instaladas, como React, Tailwind CSS o Starlight, según la configuración del proyecto.</p><p>Este proyecto aun no tiene integrado nada, por eso se muestra none.</p>|

**4. Prueba npx astro dev --background, status, logs y stop.**

**4.1. Iniciar en segundo plano**

![](Aspose.Words.6c74796c-2370-41d3-b8d4-4827c0d8c65f.007.png)

**Propósito:** inicia el servidor de desarrollo como un proceso independiente, permitiendo seguir utilizando la terminal. Astro registra información del servidor para facilitar su administración.

**4.2. Consultar el estado**

- ![](Aspose.Words.6c74796c-2370-41d3-b8d4-4827c0d8c65f.008.png)

**Propósito:** comprueba si el servidor en segundo plano está activo. Puede mostrar su dirección URL, el identificador del proceso (PID) y el tiempo de funcionamiento.

**4.3. Consultar los registros**

![](Aspose.Words.6c74796c-2370-41d3-b8d4-4827c0d8c65f.009.png)

**Propósito:** muestra los registros del servidor, útiles para identificar errores y comprobar solicitudes.

**4.4. Detener el servidor**

![](Aspose.Words.6c74796c-2370-41d3-b8d4-4827c0d8c65f.010.png)

**Propósito:** detiene el servidor de desarrollo que se inició en segundo plano.

**5. Provocar y corregir un error de compilación (build)**

**- Provocar el error**

En la ruta src/pages/index.astro, y se agregara temporalmente una etiqueta la etiqueta <p> sin cerrar:

![](Aspose.Words.6c74796c-2370-41d3-b8d4-4827c0d8c65f.011.png)

Al ejecutar la compilación en la terminal

![](Aspose.Words.6c74796c-2370-41d3-b8d4-4827c0d8c65f.012.png)

**Error** 

![](Aspose.Words.6c74796c-2370-41d3-b8d4-4827c0d8c65f.013.png)

![](Aspose.Words.6c74796c-2370-41d3-b8d4-4827c0d8c65f.014.png)

- **Corregir el error**

  Cerramos la etiqueta p con </p>:

  ![](Aspose.Words.6c74796c-2370-41d3-b8d4-4827c0d8c65f.015.png)

  Se corrige el error en la compilación automáticamente y se muestra la pagina

  ![](Aspose.Words.6c74796c-2370-41d3-b8d4-4827c0d8c65f.016.png)
