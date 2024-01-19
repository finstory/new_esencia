## ESENCIA DOCUMENTACIÓN

> [!IMPORTANT]
> ### ÍNDICE: <br/>
> ##### - ENTIDADES: <br/>
>- [Equipos](#equipos) <br/>
>- [Usuarios](#usuarios) <br/>
>- [Roles](#roles) <br/>
> ##### - FUNCIONALIDADES: <br/>
>- [Usuario - Común](#usuario-normal) <br/>
>- [Usuario - Scrum Master](#usuario-admin-scrum-master) <br/>
> ##### - VISTAS: <br/>
>- [Auth](#auth) <br/>
>- [New User](#new-user)
>- [Global](#global)
>- [Dashboard](#dashboard)
>- [Retrospective](#retrospective)
>- [Encuestas Diarias](#encuestas-diarias)
>- [Feedback](#feedback)

#

> ENTIDADES PRINCIPALES:

##### `Teams:`
```bash
- id
- name
- logo
- members
- description
```

##### `Users:`
```bash
- id
- photo
- first name
- last name
- email
- password
```

##### `Roles:`
```bash
- id
- role_type
- status
```

#

> FUNCIONALIDADES:

##### `Usuario Normal:`

```bash
- Pueden hacer encuestas & retros en el sitio a través de una invitación y/o ingresando a la plataforma.

- Ver datos no sensibles sobre el team.

- Puede registrarse, se le pedirá datos básicos.

- Puede cambiar su contraseña.

- Loguearse con Google o manual.

- A la hora de completar encuestas y retro se le respetara el anonimato.

- Sugerir añadir foto de perfil en caso de que no se haya logueado con Google.

```
> [!TIP]
> -- Actividad interactiva entre miembros (juego de trivia, por ejemplo).

##### `Usuario Admin (Scrum Master)`:

```bash
- Enviar, Administrar Retro y Encuestas.

- Acceso a las Análisis y Estadísticas del Team.

- Acceso al FeedBack.

- Poder dejar notas importantes del día para tu team y que sean visibles para todos los miembros.

- Gestionar teams y miembros del equipo (banear, agregar, eliminar, modificar).

```
> [!TIP]
> -- Posibilidad de descargar un reporte semanal, quincenal o mensual a PDF o via email.
#

> PÁGINAS DE LA WEB:


##### `AUTH:`
###### Página de entrada a la web, gestiona la autenticación del usuario.
```bash
- Registro con formulario ó google.

- Logueo con email & pass ó google.

- Recuperación de contraseña.
```

##### `NEW USER:`
###### Aquí si eres un usuario nuevo se te sugerirá datos adicionales para tu perfil. 
```bash
- Se mostrará una animación de entrada.
- Se te pedirá un Nombre y Apellido. Cómo opcional también Roles y Foto de Perfil.
``` 

##### `GLOBAL:`
###### Funcionalidades disponibles en todas las páginas.
```bash
- MIEMBROS & SCRUM MASTER:
    ○ Ver todos mis teams y sus miembros.
    ○ Opción para acceder a tu perfil.
    
- SOLO SCRUM MASTER DEL TEAM:
    ○ Menú para moverse entre páginas administrativas como las retrospectiva, encuestas diarias, feedback.
``` 

##### `DASHBOARD:` 
###### Sección donde se verán las funcionalidades principales.
```bash
- MIEMBROS & SCRUM MASTER:
    ○ Paneles que especifican la privacidad de tu usuario, qué datos son públicos y cuales son privados.
    ○ Tu actividad, es decir, las veces que asististe a las encuenstas y retros.
``` 
```bash
- SOLO SCRUM MASTER DEL TEAM:
    ○ Gestionar [agregar, editar o elimiar] caracteristicas de un team o miembros del mismo.
    ○ La proactividad individual de cada miembro en un team. 
    ○ Estádisitcas [gráficos] de la evolución general del team (con opciones adicionales, quitar gráficas, ajustar fecha, etc.) junto con las Key Team Indicators.
    ○ Panel de estadísticas númercias, como cantidades de retros hechas, etc.
    ○ Opciones rápidas de envío de retro o encuesta diaría.
    ○ [IA] Panel de sugerencias de mejoras para tu equipo (se puede mejorar aún).
``` 
> [!TIP]
> -- Chat solo para que el scrum master envié mensajes de notas del día o sugerencias para un team.

##### `RETROSPECTIVE:` 
###### Páginas donde se hacen y gestionan tus retrospecticas.
```bash
- Modo Miembro:
    ○ Cada miembro puede responder como maxímo 2 preguntas y solo podrá eliminar sus respuestas.
    ○ La actividad de las retro ocurrirán en tiempo real y será visible en ese momento para todos los miembros.
    ○ Por cada pregunta habrá una columna donde todas las respuestas se pondrán en filas.
``` 
```bash
- Modo Scrum Master:
    ○ Gestionar tus retrospectivas, esto implica poder editarla las cantidad de preguntas que quieras hacer.
    ○ Un historial para rever tus retros anteriores.
    ○ Opción para enviar tu retrospectiva a todos tus miembros del team.
``` 
> [!TIP]
> -- Lista de todas las preguntas de las retros anteriores, con la posibilidad de ver las más destacadas y las más negativas.

##### `ENCUESTAS DIARIAS:` 
###### Páginas donde se hacen y gestionan tus encuestas diarias.
```bash
- Modo Miembro:
    ○ Cada miembro deberá contestar una serie de preguntas con puntación del 1 al 10.
    ○ Si un miembro quiere añadir una comentario adicional, puede hacerlo.
    ○ Se le anunciará con una animación al usuario que su encuesta fue enviada.
``` 
> [!TIP]
> -- Estaría bueno aplicar otras actividades diarías, como por ejemplo la posiblidad de que cada miembro pueda hacer su propia pregunta de manera anonima y otro miembro deba contestarla.

```bash
- Modo Scrum Master:
    ○ La idea es gestionar de la misma manera que las retrospectivas, así que muchos puntos se repitan. Como poder editar tus preguntas y enviarlas a tus miembros, de manera automatica o manual.
``` 
##### `FEEDBACK:` 
###### Página para gestionar tus retrospecticas.
```bash
-[IA] Dar recomendaciones para mejorar aspectos del proyecto y comunicación entre los miembros. 
-[IA] Realizar un análisis diario de las encuestas [gráficas y estádisitcas generales] y dé una descripción del avance o retroceso que haya tenido el grupo. 
``` 
#
