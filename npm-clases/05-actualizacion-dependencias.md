

Actualización de dependencias
Muchas veces tenemos proyectos o tenemos que trabajar con proyectos que hace mucho tiempo han estado sin actualizarse

Babel es un Transpilador para entender javascript moderno y lo pasa al último estándar de ECMAScript.
Eslintrc Analizan nuestro código para dar mejorar que debemos implementar.
.gitignore Listamos archivos, que no queremos en nuestro repositorio.
.prettierrc estandat para manejar sintaxis
Package.lock.json y package.json nuestros archivos estándares.
Package.json
Este archivo base contiene la información de nuestra aplicación, algo muy parecido a un manual de lo que necesita la aplicación para funcionar de la forma correcta.

Actualización de paquetes
npm list nos muestra todos los elementos que son parte del proyecto y los errores correspondientes si es el caso y no están instalados.

npm install procederá a instalar todas las dependencias del proyecto y podremos tener mensajes como dependencias vulneradas, de forma moderadas, altas o criticas (deben ser atendidas inmediatamente)

npm outdate nos mostrará cuales son las dependencias que necesitan o que pueden ser actualizadas porque han tenido alguna mejora.

npm install react@latest si esta dependencia usa otras y también están desactualizadas, nos informará y podemos proceder a realizar la actualización de la otra >npm i react-dom@latest