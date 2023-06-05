Comandos en NPM (Scripts)
En Node, existen comando por defecto como lo son npm start, npm build. Pero también podremos crear comandos personalizados.
Comandos personalizados
Para crear comandos personalizados, haremos uso de nuestra sección de “scripts” agregando los comandos que necesites, creando como alias. Por ejemplo:
  "scripts": {
    "start":"node src/index.js"
  },

Para ejecutar el comando tendremos que estar dentro de la carpeta raíz y ejecutamos el comando >npm run start

También podremos concatenar varios comandos en un solo script utilizando && para unirlos. Ejemplo:

    "concat": "node src/index.js && node src/index.js"
NOTA: si se rompe el primer comando, no funcionará el siguiente.
Comandos con NPX
Node Package Execute, nos permite ejecutar acciones particulares sin instalarlos. Lo ejecutamos y realizamos una tarea en particular. Ejemplo:

npx create-react-app my-app
Aquí crearemos un Proyecto nuevo de react, el cual contendrá su package.json y sus dependencias correspondientes.
Para ejecutar la apliación utilizamos npm start