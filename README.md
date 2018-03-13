
# Sistema de aprendizaje a través de las prácticas (praxi)

El sistema consiste en una página web que presenta múltiples materias y cada una ofrece un programa de ejercicios y referencias a los libros de Synergy Vision para desarrollar el conocimiento profundo y basado en prácticas desde lo más básico a lo más complejo.

El sitio web permite a los usuarios formar parte de una comunidad que propone problemas y estos se destacan semanalmente. Cada problema se clasifica por materia y por nivel de dificultad. Son 5 niveles de dificultad.

La solución de cada problema le genera puntos a los usuarios para subir en el ranking de conocimiento. Además por cada problema propuesto se genera reputación, así como por el tiempo que pertenece a la comunidad.

## Página principal

- La página principal presenta el contenido destacado:
    - Problemas de la semana para cada nivel
    - Libro o capítulo de la semana
    - Link de la semana (artículo o paper)
    - Curso en promoción
    - Artículo de la semana (Corpus)

## Cursos clasificados en áreas

- Se presentan las áreas en el menú lateral o superior
- Cada área contiene varias materias o cursos

## Destaca los cursos recientes (realizados por las personas)

- Los cursos iniciados se presentan con sus estadísticas de forma visual

## Destaca los cursos que se desean destacar en la plataforma

- Los cursos destacados se presentan de forma visual e interactiva

## Muestra la lista de áreas con sus cursos respectivos

- Las áreas de conocimiento son: Computación, Matemáticas, Finanzas

## Ranking para cada usuarios en relación a los problemas resueltos

- Hay una calificación por usuario
- Hay un ranking de usuarios (se ubica al usuario en su percentil)

## Estadísticas

- Se lleva la estadística de acceso a los cursos
- Los problemas resueltos
- Los correctos o los incorrectos, así como los no resueltos y se consultó la solución.
- Problemas propuestos
- Tiempo en la plataforma

# Problemas

Cada problema tiene opción de incluir contenido diferente:

- Escrito con fórmulas matemáticas (Markdown y MathJax)
- Imágenes (Locales o externas)
- Videos (Locales o Youtube)
- Gráficos (Interactivos)
- Control de R (Datacamp Light)

Cada problema tiene un tópico y un nivel de dificultad. La solución de cada problema genera puntos al usuario y lo vá subiendo en el ranking de conocimiento.

El ranking de conocimiento se presenta en una araña de las materias y los niveles que ha subido el usuario. Esa araña genera el footprint del usuario que aparece en pantalla.

# Problemas de la semana

Los problemas propuestos por la comunidad se clasifican y presentan cada semana en niveles básico, intermedio y avanzado.

# Servicio por suscripción

El servicio se cobra mensualmente o anualmente a través de Stripe, Paypal o Mercadopago.

Cada usuario paga y en la medida que pasa el tiempo termina pagando el 50% del pago que realiza un usuario nuevo.

Se debe llevar un registro de las IP desde la cual el usuario accede el servicio y no se deben permitir sesiones simultáneas (sólo web y móvil).

# Chat

Hay un chat con Soporte (Sencillo hecho con Websockets). Del lado de praxi se ve una cónsola con cada usuario con el cual se interactua y del lado del usuario es un chat simple.

Cada conversación se almacena y permanece en un histórico que los operadores pueden consultar y revisar.

# API

Se ofrece un API para permitir a otras aplicaciones acceder al contenido en aplicaciones móviles o web, con sus estadísticas y avance.

# Tecnología (FANE)

- [Firebase](https://www.firebase.google.com)

Toda la persistencia se realizará en Firebase. Se utilizan las facilidades de registro y manejo de usuarios que ofrece Firebase. El usuario puede utilizar sus credenciales de Facebook, Twitter, Email, Github (Los que permita Firebase).

- [Angular](https://angular.io)

Para manejar la interacción en la página web la aplicación se hace con Angular partiendo de una plantilla con diseño.

- [Nodejs](https://nodejs.org)

Se programa toda la lógica, manejo de persistencia, estadísticas, pagos, API, etc.

- [Express](https://expressjs.com)

Generación del sitio y acceso al contenido.

