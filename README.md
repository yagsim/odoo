# odoo
Repositorio de odoo con conexión a postgres

# Paso 1.Configuración de Postgres y pruebas:
- Para crear el docker-compose debemos acudir a la imagen de odoo en docker hub y copiar el docker-compose.yml para poder así recoger el servivio, también 
recogeremos el environment de postgres con el POSTGRES_DB,USER Y PASSWORD junto al puerto de creacion.
Puede haber un fallo si el puerto de postgres esta ocupado:

+ ¿Que ocurre si en el ordenador local el purto 5432 (postgres) esta ocupado? 
 '\n' Para ello tendremos que ir a la terminal y tendremos que usar el service postgres stop

# Paso 2 .Configuración de odoo:
- La creación de odoo sera igual que la de postgres recogiendo el compose en docker Hub donde recogeremos la imagen de la web, le daremos los puertos y el environment,
con esto ya se relacionara odoo y postgres.

# Paso 3.Enlazar PyCharm y DB.
- Para ello entramos en PyCharm ,debera ser el proffesional, en la parte de abajo habra un apartado llamada services, se abrira una ventana en la parte de abajo donde habra 
un + con una flecha para abajo , al darle ahi nos dara 4 opciones en la segunda donde pone "Docker Connections from Docker Contexts" ahi podremos enlazar Docker con PyCharm
Por otra parte esta el enlace con la base de datos en la parte derecha otro apartado llamado database ,se abrira otra solapa ,le daremos al mas y buscaremos postgreSql en DataSource
se abrira una ventana donde pondremos nuestro user ,password y los puertos,probaremos la conexión si da un fallo descargamos lo que manda ,comprobamos que la conexión este aceptada ,le daremos a apply 
y se realizara la conexión.






