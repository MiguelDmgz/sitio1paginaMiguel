Cafeteria con reservaciones
Fácil personalización:

Archivos HTML y CSS bien organizados, lo que permite modificar colores, texto, y elementos visuales sin mucha dificultad.
Compatibilidad con navegadores:

Funciona correctamente en navegadores populares como Chrome, Firefox, Edge, y Safari.

Secciones destacadas:

Inicio: Una página principal con imágenes grandes y llamativas, ideal para mostrar la identidad visual de tu cafetería.
Sobre nosotros: Información sobre la historia, visión, y valores del negocio.
Menú: Una sección para listar productos (cafés, pasteles, bebidas) con descripciones y precios.
Galería: Espacio para mostrar fotos de alta calidad del local, productos, o eventos especiales.
Testimonios: Comentarios de clientes satisfechos para generar confianza.
Contacto: Formulario para recibir mensajes, junto con ubicación en Google Maps y redes sociales.


Para que otra máquina que tenga Docker pueda abrir tu imagen o sitio web, sigue estos pasos.
Compartir el comando para descargar y ejecutar la imagen
•	Comparte el siguiente comando con la persona que usará la imagen en otra máquina:

docker push migueldmgz/sitio1pagina:tagname

Esto descargará la imagen desde Docker Hub.
3. Ejecutar la imagen en la otra máquina
•	Después de descargar la imagen, pueden ejecutarla con:

docker run -d -p 80:80 migueldmgz/sitio1pagina:último

Explicación:
o	-d: Corre el contenedor en segundo plano.
o	-p 80:80: Mapea el puerto 80 de la máquina anfitriona al puerto 80 del contenedor. Cambia el puerto si es necesario.
4. Acceder al sitio web
•	Una vez que el contenedor esté corriendo, pueden acceder al sitio web a través del navegador de la otra máquina usando su dirección IP pública o localhost si está en la misma red:

http://<IP_de_la_máquina>:80

5. Validar el funcionamiento
•	Asegúrate de que el sitio web esté configurado correctamente en el contenedor, es decir, que el servidor (por ejemplo, Nginx, Apache) sirva tu aplicación en el puerto 80 o el que configuraste.

