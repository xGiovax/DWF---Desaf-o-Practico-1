# Enlace al video

video: https://drive.google.com/drive/folders/1uxHCgIsueaXglbF7M7OuOisgfT1vNqnH?usp=sharing

------------------------------------------------------------------------

# Sistema Escolar -- Desafío Spring Boot

Proyecto desarrollado con Spring Boot, JPA y H2 que gestiona alumnos y
materias, incluyendo su relación muchos-a-muchos.

------------------------------------------------------------------------

## Tecnologías utilizadas

-   Java 17+
-   Spring Boot
-   Spring Data JPA
-   H2 Database (en memoria)
-   JUnit 5
-   Maven


## Estructura del proyecto

src\
├── main\
│ ├── java/sv/edu/udb\
│ │ ├── controller\
│ │ ├── service\
│ │ ├── repository\
│ │ └── model\
│ └── resources\
│ ├── application.properties\
│ └── data.sql\
└── test\
└── java/sv/edu/udb

------------------------------------------------------------------------

## Modelo de datos

### Alumno

-   id
-   nombre
-   relación muchos-a-muchos con Materia

### Materia

-   id
-   nombre
-   relación muchos-a-muchos con Alumno

Tabla intermedia:

alumno_materia\
- id_alumno\
- id_materia

Clave primaria compuesta:

PRIMARY KEY (id_alumno, id_materia)


## Autor

Giovanni Alberto Ruano Martinez\
Desarrollo de Aplicaciones con Web Frameworks\
Universidad Don Bosco
