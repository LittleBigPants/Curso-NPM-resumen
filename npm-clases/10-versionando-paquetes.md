Pasos 📌
 

• Se recomienda tener buen estructurado el archivo README.md para tener un mejor control de los cambios que se realizan al proyecto.
 
• Si cambiamos elementos del paquete, bien sea en la lógica, en los datos, etc, lo recomendable es tener varias versiones de la publicación del paquete.
 
• Una vez hecho un cambio, se debe actualizar a git con:
git add .
git commit -m “mensaje-del-cambio”

 

• Luego se hace un cambio de versión ejecutado:
up main
 

• Se agrega la nueva versión, por ejemplo si tenemos la versión 0.0.0 se puede actualizar a:
npm version 1.1.0
 

• Con git status se verifica si todo está correcto.
 
• Se vuelve a publicar pero con la nueva versión:
npm publish
 

• Se revisa en la página de npm para ver los cambios de la versión.