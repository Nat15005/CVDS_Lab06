# Integrantes
#### Cristian Javier Alvarez

#### Laura Natalia Rojas

# Despliega mi primera aplicación en Azure
## Mi primer despliegue en la nube
# Parte I - Despliegue app React (frontend) en Azure
1. Busca Azure for Students en tu buscador de preferencias e ingresa con el correo institucional.
 
     ![image](https://github.com/Nat15005/CVDS_Lab06/assets/111907712/37803e99-8fff-43b9-9ef5-e2d456b114b9)

2. Crea un budget de 1 dólar para la cuenta

    - Nos aseguramos de tener un crédito disponible
      
    ![image](https://github.com/Nat15005/CVDS_Lab06/assets/111907712/8c7e27b2-c8f8-4521-ae0c-7ce51a06f071)

    - Una vez verificado nuestro crédito, agregamos un presupuesto
     
      ![image](https://github.com/Nat15005/CVDS_Lab06/assets/111907712/44c4d57d-ffb2-4ac2-9f74-709d762a59ca)

    - Lo creamos con los datos correspondientes:
        
      ![image](https://github.com/Nat15005/CVDS_Lab06/assets/111907712/ec2c3830-e1dc-495d-81a9-251bcbc0f28c)

    - Establecemos las condiciones de alerta y lo creamos:
      
      ![image](https://github.com/Nat15005/CVDS_Lab06/assets/111907712/82780983-c867-42e0-931b-a6cac1dabaaf)

    - Verificamos que se haya creado correctamente:

      ![image](https://github.com/Nat15005/CVDS_Lab06/assets/111907712/2e555b5c-72d4-4636-9b01-f8e6663b411c)

 
3. El profesor guía el resto de pasos

   #### Despliegue Manual:

    - Ahora vamos a subir la aplicación manualmente, para esto, creamos un nuevo recurso:
  
      ![image](https://github.com/Nat15005/CVDS_Lab06/assets/111907712/54c81d0f-7722-4814-a697-f0e85f9cc12d)

    - Creamos una aplicación web estática, agregando un nuevo grupo recursos CVDS
  
      ![image](https://github.com/Nat15005/CVDS_Lab06/assets/111907712/8c73268a-7c25-41f7-921c-00011b25c3a5)

    - Especificamos los detalles:

      ![image](https://github.com/Nat15005/CVDS_Lab06/assets/111907712/fb13bee0-4136-40ab-b8b9-38b1d504ea62)

    - Creamos el recurso:
  
      ![image](https://github.com/Nat15005/CVDS_Lab06/assets/111907712/f7eeb98f-090d-4ee3-9cfd-2d7d2a207abf)

    - Verificamos que se haya completado la implementación

      ![image](https://github.com/Nat15005/CVDS_Lab06/assets/111907712/b4c1a54f-e2fd-4d8b-a009-557ac0962736)

    - Compilamos el proyecto con NODE_OPTIONS=--openssl-legacy-provider npm run start
      Una vez compilado prendemos docker, y ejecutamos el siguiente comando en la ruta build que se generó después de compilar:

      ![image](https://github.com/Nat15005/CVDS_Lab06/assets/111907712/05ff8ad8-3be9-464b-a632-8ae3e25d3bfc)

    - Entramos a la carpeta bin/staticsites/
    
      ![image](https://github.com/Nat15005/CVDS_Lab06/assets/111907712/14eb97b6-57bf-42c7-9f4b-9094da99b12e)

    - Ahora en Azure, buscamos el token de implementación y lo copiamos:
    
      ![image](https://github.com/Nat15005/CVDS_Lab06/assets/111907712/a6b5da6e-99ed-45c1-8e13-6396b3da5ebf)


    - Ahora cargamos el recurso con el siguiente comando
    
      ![image](https://github.com/Nat15005/CVDS_Lab06/assets/111907712/d0f96d91-6db2-447d-8b41-cce7c25bc034)

    - Si se subió correctamente, se debería ver algo así:
    
      ![image](https://github.com/Nat15005/CVDS_Lab06/assets/111907712/eaab1844-3bb8-444e-b8db-e7d70fb72e4d)

    - Verificamos usando el link https://red-mushroom-0666ddd10.5.azurestaticapps.net :
    
      ![image](https://github.com/Nat15005/CVDS_Lab06/assets/111907712/c7baced0-722d-475d-83c6-c6f26f0e5ad9)

   #### Despliegue Automático:

    - Ahora vamos a subir la aplicación automáticamente, para esto, creamos un nuevo recurso estático:

      ![image](https://github.com/Nat15005/CVDS_Lab06/assets/111907712/a1bc8745-c26e-45f3-979b-af0c5b11a469)

    - Creamos la aplicación web estática con los siguientes datos:
    
      ![image](https://github.com/Nat15005/CVDS_Lab06/assets/111907712/6f364b1a-9edb-423e-afa9-b55d94e09c80)
  
    - Enlazamos los siguientes datos con el gitHub correspondiente:      

      ![image](https://github.com/Nat15005/CVDS_Lab06/assets/111907712/7e751f1a-6f82-4ff5-b42c-8a9aecd4ddab)
      
    - Revisamos y creamos:
      
      ![image](https://github.com/Nat15005/CVDS_Lab06/assets/111907712/330bb2f1-b179-4c66-bb78-01a246a0d264)

    - Ahora modificamos esta parte del código:
    
      ![image](https://github.com/Nat15005/CVDS_Lab06/assets/111907712/242b1550-4090-4471-befe-b43600888244)
    
      ![image](https://github.com/Nat15005/CVDS_Lab06/assets/111907712/57f01ab1-d96f-42b6-993a-547b5308a4d2)

    - Ahora en gitHub nos vamos a la sección de Action para compilar y hacer el despliegue
      
      ![image](https://github.com/Nat15005/CVDS_Lab06/assets/111907712/aae83b88-aa59-4c29-977d-dca0074e6935)

    - Ahora, en azure buscamos el link, y probamos que el despliegue se haya ejecutado correctamente:
    
      ![image](https://github.com/Nat15005/CVDS_Lab06/assets/111907712/af6c7ea6-45d6-48df-821a-3eb697b541b5)
    
    - Probamos en el navegador con el link que copiamos https://wonderful-moss-03055d310.5.azurestaticapps.net :
    
      ![image](https://github.com/Nat15005/CVDS_Lab06/assets/111907712/ad2be27f-332b-4d47-914a-8d74a5693486)

# Parte II - Despliegue app web spring MVC (o spring-boot backend)

1. Inicie Azure Cloud Shell desde el portal. Para implementar en un grupo de recursos, ingrese el siguiente comando

    ![image](https://github.com/Nat15005/CVDS_Lab06/assets/111907712/9d64f6ca-f72e-40a7-9ddd-f067ba047f3d)

2. Para crear un plan de servicio de aplicaciones (App service plan)

    ![image](https://github.com/Nat15005/CVDS_Lab06/assets/111907712/323e150c-1678-40a2-a0db-fe51c434bcd5)

3. Finalmente, cree el servidor MySQL con un nombre de servidor único.
  
    ![image](https://github.com/Nat15005/CVDS_Lab06/assets/111907712/a92b862a-0acb-4a9b-ab0f-825630b2737f)

    ![image](https://github.com/Nat15005/CVDS_Lab06/assets/111907712/59cb79eb-e23a-4a47-be86-cc587c11991e)

    ![image](https://github.com/Nat15005/CVDS_Lab06/assets/111907712/3d77c61d-eb8c-4617-ab3b-ec2d5b91fecc)

4. Miramos que se haya creado correctamente

   ![image](https://github.com/Nat15005/CVDS_Lab06/assets/111907712/2ce55b7c-3c80-48e3-8c1b-0b611dbfc87c)

5. Ahora dentro del servidor, vamos al apartado de redes y habilitamos la siguiente opción:

   ![image](https://github.com/Nat15005/CVDS_Lab06/assets/111907712/50711c40-0534-4932-95f1-814cf3bfff61)


### Ejercicio 2: actualización de la configuración de la aplicación web

1. Ahora, creamos un nuevo recurso con los siguientes datos

   ![image](https://github.com/Nat15005/CVDS_Lab06/assets/111907712/bffb8195-5e26-48c8-9d29-87fed97d671d)

   ![image](https://github.com/Nat15005/CVDS_Lab06/assets/111907712/e7d30a77-c4be-45ec-9e62-67b1a1c4de43)

2. Después de haber llenado todos los campos, le damos en crear

   ![image](https://github.com/Nat15005/CVDS_Lab06/assets/111907712/2e958fc0-b345-428b-83ae-c9ab840fdb15)

3. Comprobamos que la implementación se haya completado correctamente

   ![image](https://github.com/Nat15005/CVDS_Lab06/assets/111907712/28edcb2b-0d99-4ab9-b636-28dac626e93e)

4. Abrimos el link del dominio predeterminado del recurso:

   ![image](https://github.com/Nat15005/CVDS_Lab06/assets/111907712/5e92a96f-160c-4061-ac23-bb36bea421ea)

5. La página web se verá como la imagen a continuación

   ![image](https://github.com/Nat15005/CVDS_Lab06/assets/111907712/7dbd8739-14d8-45d5-91d3-05f10e107be0)

6. Ahora, actualizamos las cadenas de conexión para que la aplicación web se conecte correctamente a la base de datos, desde azure vamos a configuraciones y damos click en el recuadro resaltado

   ![image](https://github.com/Nat15005/CVDS_Lab06/assets/111907712/4c42918b-904c-4e15-9da5-f9469564879f)

7. Añadimos una nueva cadena de conexión, teniendo en cuenta que en valor debe ir el jdbc reemplazando los valores correspondientes de :MySQL Server Name, your user name, your password
   jdbc:mysql://{MySQL Server Name}:3306/alm?useSSL=true&requireSSL=false&autoReconnect=true&user={your user name}&password={your password}

   ![image](https://github.com/Nat15005/CVDS_Lab06/assets/111907712/eeb6d797-3177-42ae-a38d-c275b469f7d2)

8. Ahora, en la ruta src/main/resources/application.properties agregamos lo siguiente:

   ![image](https://github.com/Nat15005/CVDS_Lab06/assets/111907712/d0a41937-1938-4882-ab72-3af858b395dc)

9. También en el archivo Lab7Application.java agregamos la siguiente importación:

    ![image](https://github.com/Nat15005/CVDS_Lab06/assets/111907712/4aac5e60-a354-4841-8cf1-bc43d3074bff)

10. Una vez hecho esto, hacemos $mvn package para generar el .jar

    ![image](https://github.com/Nat15005/CVDS_Lab06/assets/111907712/463d66bf-600e-424d-ac9b-82757e4d737c)

    ![image](https://github.com/Nat15005/CVDS_Lab06/assets/111907712/be2ab602-54ca-462f-9cea-43d56170c167)

11. Ahora en el recurso de nuestra aplicación, en el apartado de configuración, configuramos el servicio ftp como se muestra a continuación:

    ![image](https://github.com/Nat15005/CVDS_Lab06/assets/111907712/ca568dc3-11e3-49f4-af4a-6d418a304ffd)

12. Revisamos las credenciales de FTPS para establecer la conexión

    ![image](https://github.com/Nat15005/CVDS_Lab06/assets/111907712/6744cffc-ddbb-4bf5-b4bd-f4a7992b8228)

13. Ingresamos las credenciales anteriores en el cliente ftp (fileZilla en este caso) para establecer la conexión, luego ubicamos el .jar que generamos (debemos cambiarle el nombre 'app.jar')

    ![image](https://github.com/Nat15005/CVDS_Lab06/assets/111907712/3d28263d-d088-4ea7-bd67-f181fef3a89a)

14. Arrastramos el app.jar al sitio remoto

    ![image](https://github.com/Nat15005/CVDS_Lab06/assets/111907712/ed0d0bdc-6942-4517-9144-ba2c37a15b69)

15. Ahora, en la configuración de la aplicación configuramos el comando de inicio, como se muestra:

    ![image](https://github.com/Nat15005/CVDS_Lab06/assets/111907712/12bbef9a-7be0-407e-bdb0-86b7ce37263d)

16. Copiamos el link de nuestra aplicación

    ![image](https://github.com/Nat15005/CVDS_Lab06/assets/111907712/de29ce05-27e0-4678-a953-e04717b5f9b4)

17. Probamos el funcionamiento de la aplicación con el link que copiamos https://cvdsappwebmvc.azurewebsites.net :

    ![image](https://github.com/Nat15005/CVDS_Lab06/assets/111907712/48a48506-b9dc-40d6-bea8-4d768955e3b4)

    



    

  

