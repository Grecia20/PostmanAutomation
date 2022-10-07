## **Automatizacion pruebas de servicios Restful-booker**

QA Grecia Ponce

### 📝 Acerca
----
Este es un desafío para crear un proyecto de automatización API. ✨


### 🔧 Instalación de herramientas
----
#### Postman
![](https://i0.wp.com/www.hoclabs.com/wp-content/uploads/2017/02/postman.png?fit=837%2C500&ssl=1)


1. Descargar la herramienta Postman [Download](https://www.postman.com/downloads/)   
2. Instalar la herramienta Postman en su máquina
3. Abrir la herramienta


#### Newman
![](https://ull-esit-dsi-1617.github.io/primeros-pasos-en-nodejs-carlos-david-35l2-2/assets/nodejs-npm_logos.png)

1. Descargar primero el node.js [Download](https://nodejs.org/en/download/current/)    
2. Instalar la herramienta node.js
3. Verificar desde la consola ingresando  `$ node -v `
4. Una vez verificado la instalación del node, se procede con la instalación de Newman ingresando la línea de comando `$ npm install -g newman ` 
5. Si se desea obtener una repostería mejor en visibilidad y en extensión html, ingresar la línea de comando `$ npm install -g newman-reporter-html` 
 y `$ npm install -g newman-reporter-htmlextra`

### ⚙ Configurando script
                
----
1. Una vez abierto Postman, procedemos dando clic en menú y seleccionamos la opción "Import" y clic en la opción File// OpenAPI, buscamos la ruta donde se ubica la colección y el environment damos clic en el botón "Import".
2. Ya importado el paquete de los servicios automatizado, procedemos a dar clic izquierdo en la colección y clic en la opción "Run collection", se mostrará la lista de servicios y configuramos a criterio propio como se desea el recorrido de la colección, damos clic en el boton "Run ApiAutomation-Restful-booking", lo siguiente es que mostrará el reporte de la ejecución en Postman.
3. Si se quiere visualizar desde consola el reporte Newman, debemos ejecutar el servicio desde consola, ingresamos a la consola en la ruta donde se encuentra alojado la colección y environment, y 
ejecutamos el siguiente comando: ` $ newman run ApiAutomation-Restful-booker.postman_collection.json -e Environment-Restful-booker.postman_environment.json` , cuando termine de ejecutar todo el servicio, se mostrará el reporte con detalle de los test case ya se executed o failed.
4. Para obtener la reporteria en html ejecutar el comando en consola lo siguiente `$ newman run ApiAutomation-Restful-booker.postman_collection.json -e Environment-Restful-booker.postman_environment.json -r htmlextra` , nos
vamos en la carpeta ubicada la colección y se visualizará una carpeta creada automáticamente, ingresamos y visualizaremos el reporte con extensión .html y lo abrimos en nuestro navegador preferido.


