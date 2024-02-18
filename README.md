  # Documentación Chat Buho

Repositorio de documentación de nuestro sistema omnicanal [Chat Buho](https://buho.la/chat/). Aquí encontrarás guías y tutoriales para maximizar el uso de nuestra plataforma. 

Tener en cuenta la estructura general del contenido que debe tener cada artículo:
- Título y Descripción
- Introducción
- Configuración inicial
- Funciones y uso básico
- Funciones avanzadas
- Casos de uso
- Problemas comunes y sus soluciones
- Preguntas frecuentes
- Recursos Adicionales

Si estas colaborando con nosotros usa los siguientes comandos:

### Instalación

```
$ npm install
```

### Iniciar entorno Local

```
$ npm start
```
Este comando inicia un servidor de desarrollo local y abre una ventana del navegador. La mayoría de los cambios se reflejan en vivo sin tener que reiniciar el servidor.

### Build

```
-- Usar npm run build. almenos en Windows 10
$ npm build
```
Este comando genera contenido estático en el directorio `build` y se puede usar en cualquier hosting. Esta carpeta es ignorado en el repositorio.

### Deployment

Usando SSH:

```
$ USE_SSH=true npm run deploy
```

Sin usar SSH:

```
$ GIT_USER=<Your GitHub username> npm run deploy
```
Este comando publica el contenido estatico a través de la rama `gh-pages`.

Instrucciones que Seguí:

Primero descargar la carpeta del repositorio, guardarla en nuetra pc , abrir VSCode, colocar npm install luego npm start
modificar la linea N° 66 que corresponde al "src:" etiqueta del logo. abrir el terminal y colocar npm run build luego npm run serve, luego crear el repositorio con el nombre de nuestro proyecto
en este caso "documentacion" luego en el terminal colocar -git init, -git add . , git commit -m "test" .
A continuacion cargamos nuestra carpeta local a nuestro repositorio con el comando:
git remote add origin https://github.com/JLBenYa/documentacion.git
git branch -M main
git push -u origin main

por ultimo creamos el git-hub page atravez del terminal:
PS C:\Users\BenJack\Documents\GitHub\documentacion> cmd /C 'set "GIT_USER=JLBenYa" && npm run deploy'  

Abrir el link https://jlbenya.github.io/documentacion/



