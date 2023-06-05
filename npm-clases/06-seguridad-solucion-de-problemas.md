Seguridad y solución de problemas
Muchas veces algunas dependencias pueden llegar a comprometer nuestro proyecto y podemos verlos al momento de hacer el npm install, si nos muestra vulnerabilidades

Moderates: pueden dejarse pasar, pues no tendrán mayor efecto.
High: podemos considerarlas, esto puede volverse crítico.
Critical: son las que si o si hay que reparar.
npm audit veremos las vulnerabilidades, lo que está sucediendo y nos entrega una serie de información para tomar decisiones. Si continuaremos utilizando la librería o si la actualizamos.

npm audit fix puede ser usado si nos indica que están disponibles reparaciones de dependencias. Entonces a parte de ejecutar la auditoria, puede hacer una reparación.

npm audit --json mostrará la información de forma mas detallada en un formato json para analizarla mejor.

npm audit fix --force es sugerido para implementar la reparación de las demás vulnerabilidades y por fin ser reparadas.

npm install nombre@latest se usa para actualizar los paquetes a su última versión para que no esté causando vulnerabilidades.