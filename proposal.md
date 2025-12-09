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
|CRUD dependiente|1. CRUD Evento depende de CRUD Categoria y CRUD Organizador<br>2. CRUD Entrada depende de CRUD Evento, CRUD Usuario y CRUD TipoEntrada|
|Listado<br>+<br>detalle| 1. Listado de eventos filtrado por categoría que muestra nombre, descripción, fecha, ubicación, cupo y categoría => detalle muestra toda la información del evento incluyendo foto y organizador<br> 2. Listado de categorías que muestra nombre y descripción => detalle muestra la cantidad de eventos de esa categoría y seguidores|
|CUU/Epic|1. Registrar organizador con validación de CUIT<br>2. Registrar usuario con validación de DNI<br>3. Crear evento con imagen, ubicación, fecha y categoría|


Adicionales para Aprobación
|Req|Detalle|
|:-|:-|
|CRUD |1. <br>2. |
|CUU/Epic|1. Comprar entrada para un evento (genera entrada con estado "ACTIVA")<br>2. Seguir/dejar de seguir categorías<br>3. Modificar perfil de usuario<br>4. Modificar perfil de organizador<br>5. Login unificado (usuario/organizador)|


### Alcance Adicional Voluntario

*Nota*: El Alcance Adicional Voluntario incluye funcionalidades implementadas que mejoran la experiencia del usuario.

|Req|Detalle|
|:-|:-|
|Listados |1. Listado de entradas por usuario que muestra evento, fecha de compra, estado y tipo de entrada<br>2. Listado de eventos por organizador<br>3. Listado de categorías seguidas por usuario<br>4. Visualización de eventos en mapa interactivo con geolocalización|
|CUU/Epic|1. Eliminar cuenta de usuario<br>2. Cancelar entrada (cambia estado de "ACTIVA" a "CANCELADA")<br>3. Carga de imagen de evento con integración de Cloudinary <br>4. Visualizar ubicación del evento en mapa interactivo|
|Otros|1. Moderación de contenido con IA para descripción de eventos y organizadores<br>2. Validaciones de formularios en frontend<br>3. Sistema de autenticación con tokens<br>4. Integración con API de mapas para visualización de ubicaciones|
