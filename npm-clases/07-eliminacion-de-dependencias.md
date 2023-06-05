Para eliminar una dependencia Ejemplo:

npm unistall webpack-dev-server
Otra forma es ir al archivo package.json y eliminar del listado de dependencia, dependencias de desarrollo o dependencias opcionales; una vez eliminado de la lista ejecutamos

rm -rf node_modules/
npm install
Para compilar el proyecto usamos

npm run build
Para compilar el proyecto y obtener mas informacion usamos


npm run build --dd
Para ver librerias deprecadas

npm ci