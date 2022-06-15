# Práctica 1. Creación de una página web en Azure
## Creación de la página
En Azure Potal buscamos el Marketplace.

![p1p1](imagenes\p1p1copia.png)

Una vez en Marketplace, buscamos WordPress.

![p1p2](imagenes\p1p2.png)

Seleccionamos la primera opción.

![p1p3](imagenes\p1p3.png)

En Plan elegimos WordPress y damos click en crear.

![p1p4](imagenes\p1p4.png)

Para crea una instancia en Azure necesitaremos al menos 4 parámetros:
- Suscripción. Azure for Students en esta ocasión.
- Grupo de recursos. Seleccionamos un grupo de recursos o creamos uno nuevo; en este caso creamos per grupo de recursos sesion2-practica1.
- Región: Para tener una menor latencia, seleccionar una región cercana a nosotros es de mucha importancia. En este elegimos South Central US.
- Nombre: El nombre de la páginaweb, en este caso, deberá ser único.
Elegimmos el sistema operativo de preferencia. Por el momento dejaremos el sistema operativo de Windows.

![p1p5](imagenes\p1p5.png)

Podemos agragar etiquetas con las cuales podemos identificar cosotos, áreas y el impacto de la instancia.

![p1p6](imagenes\p1p6.png)

Podemos ver los recursos que se han creado:
- Plan de App Service (gratuito)
- App Service (gratuito)
- Servidos único de Azure Database fos MySQL (de pago)

![p1p16](imagenes\p1p16.png)

## Configuración de la prágina
En el recurso seleccionamos el link URL que nos llevará a nuestra página de WordPress. Una vez que nuestra página haya sido configurada, este URL nos servirá para compartir nuetra página.

![p1p8](imagenes\p1p8.png)

Serelccionamos el idioma de preferencia.

![p1p9](imagenes\p1p9.png)

LLenamos la información que de pide
- Título del sitio: Wizards
- Nombre de usuario: karicaracola
- Contraseña
- Correo electrónico 
- Visibilidad en los motores de búsqueda
Seleccionamos instalar WordPress

![p1p10](imagenes\p1p10.png)

Al crearse la página recibiremos un díalogo donde se nos da la bienvenida.

![p1p12](imagenes\p1p12.png)

Si al URL de agregamos al final de este "/wp-admin" nos dirigirá a la página de edición.

![p1p13](imagenes\p1p13.png)

Se nos pide el nombre de usuario y contraseñas solicitados en un inicio.

![p1p11](imagenes\p1p11.png)

Se nos redirige a la página de edición para nuestra página de WordPress.

![p1p14](imagenes\p1p14.png)

## Deshabilitación de la página para evitar el cobro
Como se mencioná antes, los recursos de Azure Database for MySQL cobrarán nuestro crédito incluso si no se usa la página. Para evitar que Azure consuma todo nuestro crédito eserá necesario detener este recurso.
En el grupo de recursos que ehemos creado para esta práctica seleccionamos el recurso de Azure Database for MySQL.

![p1p15](imagenes\p1p15.png)

Presionamos "Detener". Este paso dejará inhabilitada la página por lo que acceder a ella no será posible.

![p1p17](imagenes\p1p17.png)

Este recurso se detendrá, evitando que se continúe el cobro.
Si queremos que el recurso vuelva a ejecutarse, debe presionarse "Iniciar", de esta manera la página volverá a habilitarse.

![p1p18](imagenes\p1p18.png)

### Nota personal

- git add .
- git commit -m "README añadido"
- git push origin main
- git pull origin main (si algo falla)