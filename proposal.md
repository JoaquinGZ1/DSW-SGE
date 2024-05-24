# Propuesta TP DSW

## Grupo
### Integrantes
* 51418 - San Pedro, Lucas
* 50939 - Seffino, Mateo
* 51190 - Giménez, Joaquín
* 50449 - Orsi, Dante

### Repositorios

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
|CRUD simple|1. CRUD Categoría<br>2. CRUD Cuenta<br>3. CRUD Localidad|
|CRUD dependiente|1. CRUD Evento {depende de} CRUD Categoría,CRUD Organizador y CRUD Ubicación<br>2. CRUD Ubicación {depende de} CRUD Localidad|
|Listado<br>+<br>detalle| 1. Listado de eventos filtrado por rango de fecha, localidad y categoría muestra nombre, fecha, foto y ubicación => detalle CRUD Evento<br> 2. Listado de entradas filtrado por rango de fecha, muestra nombre de evento, fecha de evento, foto de evento => detalle muestra ubicación de evento y datos completos de entrada junto a su tipo de entrada|
|CUU/Epic|1. Crear Perfil<br>2. Crear evento|


Adicionales para Aprobación
|Req|Detalle|
|:-|:-|
|CRUD |1. CRUD Categoría<br>2. CRUD Cuenta<br>3. CRUD Localidad<br>4. CRUD Provincia<br>5. CRUD País<br>6. CRUD Valoración<br>7. CRUD TipoEntrada<br>8. CRUD Entrada|
|CUU/Epic|1. Crear Perfil<br>2. Crear evento<br>3. Comprar entrada<br>4. Crear tipo de entrada|


### Alcance Adicional Voluntario

*Nota*: El Alcance Adicional Voluntario es opcional, pero ayuda a que la funcionalidad del sistema esté completa y será considerado en la nota en función de su complejidad y esfuerzo.

|Req|Detalle|
|:-|:-|
|Listados |1. Eventos a los que asisten amigos del usuario muestra nombre de amigo, foto de perfil de amigo, nombre de evento, fecha de evento, foto de evento y ubicación de evento => detalle CRUD Evento<br> 2. Listado de usuario filtrado por nombre de usuario muestra nombre de usuario, foto de perfil => detalle CRUD Usuario|
|CUU/Epic|1. Crear Categoría<br>2. Cancelación de entrada<br>3. Crear ubicación<br>4. Hacer valoración<br>5. Asistir a evento<br>6. Editar perfil<br>7. Agregar amigo<br>8. Interactuar en un grupo de evento<br>9. Comunicarse via mensaje directo con otra Cuenta|
|Otros|1. Envío de recordatorio de eventos<br>2. Envio de eventos que puedan interesar al usuario|
