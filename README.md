# Prueba Tecnica Ilumno

* Se crea un modulo llamado **example_users_rest**
* Se crea un recurso rest en el modulo para obtener y actualizar la información que se almacena en la tabla que el modulo **example_module** inserta
* Se implementa el metodo **GET** para obtener la información de la tabla **example_users**
* Se implementa el metodo PATCH para actualizar la información de un registro de la tabla **example_users**

## Rutas

* example-crud/data/{id}

## Evidencia grafica del modulo

* Se degenera dependencia del modulo **example_module** y del modulo **rest**
  
  ![image](https://user-images.githubusercontent.com/84405166/151637416-c3c21ef3-cba0-4d05-bf04-4c9f676e28cf.png)
  
* Se implementa autenticación basica para el Rest, lo que indica que si se desea consumir desde un agente externo, como **postman** se debe incluir las credenciales del usuario administrador de drupal en una autenticación Basica

  ![image](https://user-images.githubusercontent.com/84405166/151637558-1eeda272-0554-4618-8c4d-dcbdf8a91d2b.png)
  
* Se establecen los permisos para los dos recursos implementados, GET y PATCH

  ![image](https://user-images.githubusercontent.com/84405166/151637723-c143ef27-c9d7-4f90-9907-3352fcfeaa92.png)
  
* Se adjunta evidencia de consumo de recurso en **Postman** para metodo GET que trae un solo registro
  
  ![image](https://user-images.githubusercontent.com/84405166/151637821-7dd5ad8e-ca6c-4262-83d2-c300ff8a1cb0.png)
  
* Se adjunta evidencia de consumo de recurso en **Postman** para metodo GET que tra todos los usuarios (Se utiliza la palabra 'all')
  
  ![image](https://user-images.githubusercontent.com/84405166/151637976-56e62330-8b31-429f-99de-5657454ba63f.png)
  
* Se adjunta evidencia del consumo del metodo PATCH, para actualizar el registro 

  ![image](https://user-images.githubusercontent.com/84405166/151638058-4351ec02-62e4-4ebb-90cd-fc6ae03dca06.png)
  
## Apoyo tecnico

* Este modulo depende completamente del modulo **example_module** y del modulo **rest** y **restui** razon por la cual es necesario tener estos modulos instalados previamente
* Se utilizo drupal console para la generación de un nueveo recurso rest, en su versión de estructura base

## Checklist Prueba
1. **(REALIZADO)** Crear un segundo modulo que exponga un CRUD de servicios Restful que
permita alterar la información de la tabla generada, el path debe ser /example-crud/data.
 



