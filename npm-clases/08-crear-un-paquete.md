Mis apuntes 🤓

. Crear un repositorio

Verificar que el nombre del repositorio sea igual al nombre que tendrá en npm
Verificar que el nombre no esta en npm (https://www.npmjs.com/) y que no hayan dependencias que hagan lo mismo que nosotros estamos a punto de publicar.
Clonar el repositorio en mi local
En el proyecto crearemos un archivo index.js (dentro de src) que tendrá la lógica del proyecto.

const messages = [
  "This is where it all begins...",
  "Commit committed",
  "Version control is awful",
  "COMMIT ALL THE FILES!",
  "The same thing we do every night, Pinky - try to take over the world!",
  "Lock S-foils in attack position",
  "This commit is a lie",
  "I'll explain when you're older!",
  "Here be Dragons",
  "Reinventing the wheel. Again.",
  "This is not the commit message you are looking for",
  "Batman! (this commit has no parents)",
];

const funnyCommit = () => {
  const message = messages[Math.floor(Math.random() * messages.length)];
  console.log(`\x1b[34m${message}\x1b[89m`);
}

module.exports = {
  funnyCommit
};
Se crea una carpeta bin y dentro de ella el archivo global.js

#!/usr/bin/env node
let random = require('../src/index.js');

random.funnyCommit();
Dentro del archivo package.json añadir

"homepage": "https://github.com/gndx/random-str-msg#readme",
  "bin": {
    "random-str-msg": "./bin/global.js"
  },
  "preferGlobal": true,
  "dependencies": {
    "g": "^2.0.1"
  }