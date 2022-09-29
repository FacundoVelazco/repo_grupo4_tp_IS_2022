# repo_grupo4_tp_IS_2022
## Integrantes:
Facundo Velazco - Tomas Auday - German Vanni - Sofia Nuñez
## Objetivos: 
Repositorio de la aplicación del trabajo práctico 1 de Ingeniería de Software del grupo 4. Este trabajo nos permite familiarizarnos con la gestión de versiones mediante el uso de git, github y el modelo gitflow.

## INFORME:
### 2b. ¿Cómo hacemos para no subir cambios de configuraciones locales? Configurar el repositorio para ignorar estos archivos.
Es posible que sea necesario excluir ciertos archivos del directorio. Algunos ejemplos son archivos generados automáticamente al configurar el entorno, o generados en tiempo de ejecución, o configuraciones personales del entorno. También resulta muy útil para evitar versionar archivos con información sensible.
Para realizar esto, git nos ofrece el archivo .gitignore, en el cual podemos definir qué archivos ignorar ya sea de forma individual, una carpeta o directorio completo, o ciertos tipos de archivo.


### 2.g Llevar al entorno productivo Release 1. ¿Cómo lo hace siguiendo Gitflow?
Siguiendo el modelo gitflow, se debe realizar, a través de un pull request, un merge entre las ramas Main y Release 1, luego establecemos un tag de la nueva versión publicada, para posteriormente realizar un backport a las otras ramas.


### 2.k Llevar los cambios de la rama creada en el punto i a producción. ¿Cómo lo hace siguiendo Gitflow?
En el punto i creamos una rama con una nueva funcionalidad. Siguiendo gitflow, para esto, creamos una rama a partir de la rama develop, qué es la rama Feature, en donde se realizan todos los cambios aún no publicados.  Para llevar esta nueva funcionalidad a producción, debemos primero crear un PR con la rama develop. Una vez aprobada y con el merge entre develop y la funcionalidad realizada, se debe crear una rama release, y finalmente, se repite el proceso indicado en el punto 2.g.

### 3.a En el archivo README del repositorio describimos el proyecto en general para aquellas personas que deben leerlo. 
Dentro del mismo describimos el objetivo del proyecto, características y funcionalidades que soporta actualmente, así como también, se mencionan los errores detectados que todavía no fueron corregidos . De ser necesario, una guía de configuración del entorno de desarrollo y por último una breve guía de usuario o referencia a documentación detallada. 

Cómo se configura el entorno de desarrollo, qué dependencias tiene el proyecto, características o funcionalidades que cuenta el proyecto, objetivo, referencias a manuales y documentación.
Si es público, explicar los términos de uso.  

### 3.b Si un externo realiza una modificación, necesitamos entender el cambio realizado (PR o Pull Request). ¿Qué datos le pediría a esa persona que complete? ¿Qué nos ofrece GitHub para ayudarnos con esto?

GitHub nos ofrece la posibilidad de implementar un pull request template, a través de la cual se propone un formulario a completar por parte del solicitante, donde deberá completar los datos solicitados que correspondan en función de la modificación propuesta.

Algunos de los datos que consideramos relevantes a incluir en un PR  template son:
Descripción del cambio que se hace, si es una nueva funcionalidad o si es un bugfix.
  -En caso de ser un bugfix, deberá  incluir una referencia al error que soluciona, en la aplicación de bugtracking que el proyecto esté usando
  -Detalles del pull request: Qué y cómo se implementa.
  -Otra información que la persona considere relevante.
