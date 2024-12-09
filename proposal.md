# Propuesta TP DSW

## Grupo
### Integrantes
* 51418 - San Pedro, Lucas
* 50939 - Seffino, Mateo
* 51190 - Giménez, Joaquín
* 50449 - Orsi, Dante

### Repositorios
* [Backend App](https://github.com/LucasSanPedro18/DSW-TP)
* [Frontend App](https://github.com/JoaquinGZ1/DSW-TP-FE)

## Tema
### Descripción
Sistema para la publicación y divulgación de eventos creados por distintos perfiles organizadores. Los organizadores se registran en la aplicación y cuentan con funciones para crear distintos eventos, en ubicaciones anteriormente cargadas y pertenecientes a distintas categorias.<br>
Los perfiles de usuario son avisados de los eventos mediante la página principal o son notificados de eventos creados por organizadores que sigan. Los mismos pueden acceder al evento con la compra de una entrada.

### Modelo
* [Modelo de dominio](https://drive.google.com/file/d/16xYhbJUnDa4sdpdbVt6X3xEIybnITIP2/view?usp=sharing)

## Alcance Funcional 

### Alcance Mínimo

Regularidad:
|Req|Detalle|
|:-|:-|
|CRUD simple|1. CRUD Usuario<br>2. CRUD Organizador<br>3. CRUD Evento<br>4. CRUD Categoria|
|CRUD dependiente|1. CRUD Evento depende de CRUD Categoria|
|Listado<br>+<br>detalle| 1. Listado de eventos ordenado por fecha o categorías muestra nombre, descripción, categoría, fecha, cupo y categorias<br> 2. Listado de categorias ordenado por cantidad de eventos muestra nombre, descripción y cantidad de eventos creados|
|CUU/Epic|1. Crear organizador<br>2. Crear usuario<br>3. Crear evento|


Adicionales para Aprobación
|Req|Detalle|
|:-|:-|
|CRUD |1. CRUD Pais<br>2. CRUD Localidad<br>3. CRUD Ubicación<br>4. CRUD Entrada<br>5. CRUD TipoEntrada<br>6. CRUD Valoración|
|CUU/Epic|1. Crear categoria<br>2. Comprar entrada<br>3. Subir valoración<br>|


### Alcance Adicional Voluntario

*Nota*: El Alcance Adicional Voluntario es opcional, pero ayuda a que la funcionalidad del sistema esté completa y será considerado en la nota en función de su complejidad y esfuerzo.

|Req|Detalle|
|:-|:-|
|Listados |1. Eventos a los que asisten amigos del usuario muestra nombre de amigo, foto de perfil de amigo, nombre de evento, fecha de evento, foto de evento y ubicación de evento => detalle CRUD Evento<br> 2. Listado de usuario filtrado por nombre de usuario muestra nombre de usuario, foto de perfil => detalle CRUD Usuario|
|CUU/Epic|1. Cancelación de entrada<br>2. Crear ubicación<br>3. Hacer valoración<br>4. Asistir a evento<br>5. Editar perfil<br>6. Agregar amigo<br>7. Interactuar en un grupo de evento<br>8. Comunicarse via mensaje directo con otra Cuenta|
|Otros|1. Envío de recordatorio de eventos<br>2. Envio de eventos que puedan interesar al usuario|
