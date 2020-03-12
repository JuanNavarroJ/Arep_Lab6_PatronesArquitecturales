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

### 3. Enlazar el formulario a una base de datos relacional o no-relacional, para almacenar y traer los datos almacenados. Use servicios de base de datos de AWS.

### 4. Configurar un VPC para gestionar la seguridad y los permisos de acceso a sus servidores.


## Despliegue continuo

[![CircleCI](https://circleci.com/gh/JuanNavarroJ/Arep_Lab4_ServerWeb.svg?style=svg)](https://circleci.com/gh/JuanNavarroJ/Arep_Lab4_ServerWeb)

## Desarrollo

Construido con:

-   [Maven](https://maven.apache.org/)  - Control de dependencias

-	 [CircleCI](https://circleci.com/)  - Despliegue continuo

-	 [Heroku](https://dashboard.heroku.com/apps) - Plataforma Web

## Autor

-   **Juan David Navarro Jimenez**    -  [JuanNavarroJ](https://github.com/JuanNavarroJ)

## License

This project is licensed under the GNU General Public License v3.0 - see the [LICENSE.md](https://github.com/JuanNavarroJ/Arep_Lab4_ServerWeb/blob/master/LICENSE.txt) file for details.
