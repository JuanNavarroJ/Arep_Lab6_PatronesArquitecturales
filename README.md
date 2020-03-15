# Patrones Arquitecturales

## Problema:

Una empresa lo ha contratado para capacitar a sus ingenieros en la construcción de sitios web dinámicos sobre Amazon Web Services. Para esto usted decidió construir un tutorial y un video que permita a los ingenieros hacer lo siguiente:

### 1. Desplegar un sitio estático usando S3

Primero ingresamos a nuestra cuenta de AWS educate e ingresamos a la consola y buscamos el servicio S3.
![1](https://user-images.githubusercontent.com/44879884/76563044-a37bb980-6474-11ea-9f43-6e62784a7267.PNG)

Damos en la opción de “Crear bucket”.
![2](https://user-images.githubusercontent.com/44879884/76563045-a37bb980-6474-11ea-98a7-99314b46fa54.PNG)

Ponemos el nombre del Bucket y la región donde se encontrará.
![3](https://user-images.githubusercontent.com/44879884/76563046-a37bb980-6474-11ea-95c9-e8e570e6c179.PNG)

Dejamos la configuración que nos da por defecto.
![4](https://user-images.githubusercontent.com/44879884/76563047-a4145000-6474-11ea-8326-4b70efd8944d.PNG)

Deshabilitamos la opción que nos dice que bloqueamos el acceso público, es decir así permitimos el acceso a nuestro bucket de forma pública.
![5](https://user-images.githubusercontent.com/44879884/76563049-a4145000-6474-11ea-84e5-8abc50de62c3.PNG)

Nos mostrara la configuración final del bucket y damos en “Create bucket”.
![6](https://user-images.githubusercontent.com/44879884/76563050-a4145000-6474-11ea-8069-8dfb86648fcb.PNG)

Luego podremos ver nuestro bucket en este caso lo llamamos arep e ingresamos a él.
![7](https://user-images.githubusercontent.com/44879884/76563051-a4ace680-6474-11ea-872f-3560cf108c4b.PNG)

Damos en la opción de “Upload”.
![8](https://user-images.githubusercontent.com/44879884/76563053-a4ace680-6474-11ea-931f-98bfde7563ee.PNG)

Nos abrirá una ventana emergente la cual nos pedirá que seleccionemos los archivos que vamos a almacenar en el bucket.
![9](https://user-images.githubusercontent.com/44879884/76563028-a1195f80-6474-11ea-8f16-29e1788eb9fa.PNG)

Una vez cargado el archivo damos en siguiente.
![10](https://user-images.githubusercontent.com/44879884/76563030-a1b1f600-6474-11ea-9db2-c1053ce07346.PNG)

Luego nos mostrará la configuración de los permisos que tendrá los archivos subidos.
![11](https://user-images.githubusercontent.com/44879884/76563031-a1b1f600-6474-11ea-8a47-13bb43a0623b.PNG)

También nos mostrará algunas opciones de configuración como la cantidad de zonas donde estará disponible, tiempo de duración etc…
![12](https://user-images.githubusercontent.com/44879884/76563033-a24a8c80-6474-11ea-9000-5f56a1abdf4d.PNG)

Luego nos mostrara un resumen de los archivos subidos.
![13](https://user-images.githubusercontent.com/44879884/76563037-a24a8c80-6474-11ea-8c5e-92af089fcfc9.PNG)

Ahora podremos ver un listado de los archivos subidos.
![14](https://user-images.githubusercontent.com/44879884/76563038-a24a8c80-6474-11ea-9a88-35668a96535f.PNG)

Hacemos que el archivo sea publico para que pueda ser solicitado por cualquiera ya que por defecto es privado. 
![15](https://user-images.githubusercontent.com/44879884/76563039-a2e32300-6474-11ea-9c6f-0685612e3b26.PNG)

Ahora vemos que nos dan una URL donde se encuentra alojado el recurso.
![16](https://user-images.githubusercontent.com/44879884/76563040-a2e32300-6474-11ea-8cad-8d8b0cbd94b6.PNG)

Y vemos el resultado de solicitar el recurso a la página web.
![17](https://user-images.githubusercontent.com/44879884/76563041-a2e32300-6474-11ea-890c-970af3209118.PNG)


### 2. Desplegar un formulario dinámico usando EC2

Ahora en el servicio de AWS vamos a crear una instancia EC2 para esto buscamos el servicio EC2 y damos en él.
![Captura6](https://user-images.githubusercontent.com/44879884/76691889-c1d0e900-661d-11ea-9361-be6bedfd1234.PNG)

Luego damos en el botón de lanzar una instancia.
![Captura7](https://user-images.githubusercontent.com/44879884/76691890-c3021600-661d-11ea-9c9a-4f2e1f34ec8d.PNG)

Escogemos la imagen de la maquina la cual queremos montar que tenga los programas mínimos para funcionar nuestro laboratorio en este caso necesitamos una máquina que tenga java.
![Captura8](https://user-images.githubusercontent.com/44879884/76691891-c3021600-661d-11ea-9458-174a81a1da78.PNG)

Dejamos la instancia que nos da por defecto ya que esta es suficiente y damos en “Review and Launch”.
![Captura9](https://user-images.githubusercontent.com/44879884/76691892-c4cbd980-661d-11ea-8965-3489de3e1387.PNG)

En este paso nos mostrara la información general sobre la instancia que vamos a lanzar, damos en el botón “Launch”.
![Captura10](https://user-images.githubusercontent.com/44879884/76691894-c5647000-661d-11ea-8485-3c3b392e2e65.PNG)

En este paso como no teníamos ningún par de llaves configurado escogemos la opción de crear un nuevo par de llaves.
![Captura11](https://user-images.githubusercontent.com/44879884/76691895-c5647000-661d-11ea-9451-451bb1d99548.PNG)

Descargamos el par de llaves y lanzamos la instancia.
![Captura12](https://user-images.githubusercontent.com/44879884/76691896-c5fd0680-661d-11ea-83ba-d3da29046077.PNG)

Finalmente ponemos a correr la instancia.
![Captura13](https://user-images.githubusercontent.com/44879884/76691898-c6959d00-661d-11ea-9d9a-a2484bd05770.PNG)

### 3. Enlazar el formulario a una base de datos relacional o no-relacional, para almacenar y traer los datos almacenados. Use servicios de base de datos de AWS.

Para crear una base de datos creamos el servicio RDS el cual es el administrador de base de datos relacionales de AWS.
![1](https://user-images.githubusercontent.com/44879884/76692401-170ff900-6624-11ea-8ee1-df00ec314326.PNG)

Damos en crear database la cual nos abrirá toda la posible configuración que podemos hacer para crearla.
![2](https://user-images.githubusercontent.com/44879884/76692402-17a88f80-6624-11ea-9e48-2f6ccda0be38.PNG)

Escogemos la opción de crear fácil ya que esta opción nos simplificara cierta configuración que para el desarrollo del laboratorio no generara problemas.
![3](https://user-images.githubusercontent.com/44879884/76692403-18412600-6624-11ea-8f5e-9e618884c44a.PNG)

Ahora elegimos el motor de base datos el cual queremos crear en nuestro caso elegimos una base de datos Postgres también escogemos la configuración gratis ya que esta es suficiente para el desarrollo del laboratorio y no genera mucho costo.
![4](https://user-images.githubusercontent.com/44879884/76692404-18412600-6624-11ea-801d-dbc52bdae340.PNG)

También deberemos poner el nombre de la base de datos y una clave para el máster de la base de datos.
![5](https://user-images.githubusercontent.com/44879884/76692405-18d9bc80-6624-11ea-8af5-9ff2f7c776a2.PNG)

Esperamos unos minutos que la base de datos se monte y se cree y deberíamos ver que su estado es disponible y se creó correctamente.
![6](https://user-images.githubusercontent.com/44879884/76692399-15decc00-6624-11ea-8e9a-d0317860978e.PNG)

Si ingresamos en ella podemos ver la configuración de la máquina.
![7](https://user-images.githubusercontent.com/44879884/76692400-170ff900-6624-11ea-8b12-c64f4511b3f2.PNG)


### 4. Configurar un VPC para gestionar la seguridad y los permisos de acceso a sus servidores.

Ahora vamos a configurar la seguridad de la instancia EC2 para que pueda tener abierto el puerto 5432 que es de Postgres para enviar y recibir información por este puerto.

Ingresamos a nuestra instancia EC2 creada en el paso 2 y damos en la configuración de la seguridad.
![50](https://user-images.githubusercontent.com/44879884/76692639-34929200-6627-11ea-9702-5b210fecefd1.PNG)

Damos en editar las reglas de entrada.
![52](https://user-images.githubusercontent.com/44879884/76692641-352b2880-6627-11ea-8d17-e1f140eef5d7.PNG)


Agregamos una nueva regla.
![53](https://user-images.githubusercontent.com/44879884/76692643-352b2880-6627-11ea-92f9-5822cad97205.PNG)


Configuramos que la nueva entrada es PostgreSQL y guardamos las reglas.
![54](https://user-images.githubusercontent.com/44879884/76692636-32c8ce80-6627-11ea-9aae-772acaff209d.PNG)


Ahora configuramos las reglas de salida y también agregamos el puerto de PostgreSQL.
![56](https://user-images.githubusercontent.com/44879884/76692638-33f9fb80-6627-11ea-8150-ef560b854884.PNG)

## Desarrollo

Construido con:

-   [Maven](https://maven.apache.org/)  - Control de dependencias

-	 [CircleCI](https://circleci.com/)  - Despliegue continuo

-	 [Amazon Web Services](https://aws.amazon.com/) - Plataforma Web

## Autor

-   **Juan David Navarro Jimenez**    -  [JuanNavarroJ](https://github.com/JuanNavarroJ)

## License

This project is licensed under the GNU General Public License v3.0 - see the [LICENSE.md](https://github.com/JuanNavarroJ/Arep_Lab4_ServerWeb/blob/master/LICENSE.txt) file for details.
