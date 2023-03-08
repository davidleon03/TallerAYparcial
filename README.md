# Taller Docker | David Leon
## Objetivo
Aprender a desarrollar una aplicación web utilizando el micro-framework de Spark Java, aprender a crear y desplegar un contenedor Docker para la aplicación y configurarlo en una máquina local y en AWS. Además, aprender a utilizar DockerHub para almacenar imágenes de contenedores y poder desplegarlas en distintas máquinas.

## Herramientas utilizadas
 - Maven
 - Java 
 - Git 
 - Docker
 - Spark
 - Mongo
 
 ## Desarollo del Laboratorio y pruebas del mismo
- Empezamos creando la imagen de docker del mismo

![image](https://user-images.githubusercontent.com/98216838/223550686-874778e8-637d-4250-b7ae-8222091911e0.png)

- Verificamos la creacion

![image](https://user-images.githubusercontent.com/98216838/223550900-e791056e-2387-4dc6-b7d4-929c7baffe06.png)

- A partir de la imagen de docker crearemos 3 instancias del mismo 

![image](https://user-images.githubusercontent.com/98216838/223551431-ba5fdfdc-6b69-4b2d-bf3a-e50c7f213530.png)
- Verificamos que esten corriendo y realizamos las pruebas localmente desde esas instancias como se evidencia acontinuacion

![image](https://user-images.githubusercontent.com/98216838/223551736-3c695eda-1a8b-4120-92c9-3c38e721bfd4.png)
![image](https://user-images.githubusercontent.com/98216838/223551013-6d3db315-5d4a-45b6-9af5-6eae43fc084c.png)
![image](https://user-images.githubusercontent.com/98216838/223560474-89fd926c-c045-4c39-a822-bc501f207321.png)
- Procedemos a subir la imagen a Docker Hub 
![image](https://user-images.githubusercontent.com/98216838/223552621-db167a0c-3f48-4282-9465-e12732906ba1.png)

- Creamos una instancia en AWS EC2 y procedemos a lanzarla
![image](https://user-images.githubusercontent.com/98216838/223554419-d13c6477-77be-400f-ac84-ca17e58dbb33.png)
- Instalamos docker y corremos la imagen creada en docker hub
![image](https://user-images.githubusercontent.com/98216838/223555418-5d8c63aa-e553-4ade-baae-5eaadfd63d4d.png)
- Realizamos las pruebas desde la instancia de AWS y verificamos que funciona correctamente
![image](https://user-images.githubusercontent.com/98216838/223557824-e6a27499-0b73-45de-840a-3185be1b8d14.png)
- Verificamos que los datos si lleguen a la base de datos NoSql Mongo
![image](https://user-images.githubusercontent.com/98216838/223560139-26492299-c093-4159-a483-7977d8e7be06.png)

## Links de la maquina en AWS
- http://35.170.52.248/insert/aca se ingresa la cadena

## Documentacion

Para crear la documentación del proyecto se hace con el siguiente comando:
    
    mvn javadoc:javadoc
    

## Autor

* **David Leon**

