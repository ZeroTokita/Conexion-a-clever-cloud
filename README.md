# 📚 Práctica: Base de Datos MySQL en Clever Cloud

## 📌 Descripción del proyecto

Este proyecto consiste en la implementación de una base de datos relacional MySQL alojada en la plataforma Clever Cloud.

La práctica tiene como finalidad crear tres tablas relacionadas mediante claves primarias y foráneas, establecer una conexión remota utilizando MySQL Workbench y realizar consultas SQL para recuperar información almacenada en la nube.

## 🎯 Objetivos

- Crear una base de datos MySQL en Clever Cloud.
- Diseñar e implementar tres tablas relacionadas.
- Establecer relaciones mediante claves primarias y foráneas.
- Insertar registros de prueba en las tablas.
- Configurar una conexión remota desde MySQL Workbench.
- Ejecutar consultas SQL utilizando INNER JOIN.
- Documentar el procedimiento mediante capturas de pantalla.

## 🛠️ Tecnologías utilizadas

| Tecnología | Descripción |
|---|---|
| MySQL | Sistema de gestión de bases de datos relacionales. |
| Clever Cloud | Plataforma de alojamiento de la base de datos en la nube. |
| MySQL Workbench | Herramienta para administrar y consultar MySQL. |
| SQL | Lenguaje utilizado para crear, modificar y consultar datos. |
| GitHub | Plataforma para almacenar el código y la documentación. |

## 🗂️ Estructura de la base de datos

La base de datos contiene tres tablas:

### 1. Estudiantes

Almacena la información de los estudiantes registrados.

- `id_estudiante`: Identificador único, clave primaria.
- `nombre`: Nombre del estudiante.
- `correo`: Correo electrónico.

### 2. Cursos

Almacena la información de los cursos disponibles.

- `id_curso`: Identificador único, clave primaria.
- `nombre_curso`: Nombre del curso.

### 3. Inscripciones

Relaciona los estudiantes con los cursos en los que están inscritos.

- `id_inscripcion`: Identificador único, clave primaria.
- `id_estudiante`: Clave foránea que referencia a estudiantes.
- `id_curso`: Clave foránea que referencia a cursos.
- `fecha_inscripcion`: Fecha de inscripción.

## 🔗 Relaciones entre tablas

- Un estudiante puede tener varias inscripciones.
- Un curso puede tener varias inscripciones.
- Cada inscripción pertenece a un estudiante y a un curso.

La tabla `inscripciones` permite establecer una relación de muchos a muchos entre estudiantes y cursos.

## ☁️ Implementación en Clever Cloud

1. Ingresar a la plataforma Clever Cloud.
2. Crear un servicio de base de datos MySQL.
3. Obtener los parámetros de conexión.
4. Configurar MySQL Workbench con los datos proporcionados.
5. Comprobar la conexión remota.
6. Ejecutar el script SQL para crear las tablas.
7. Insertar los registros de prueba.
8. Ejecutar una consulta SQL para verificar los datos.

## 🔍 Consulta SQL

Se utiliza una consulta con INNER JOIN para relacionar las tres tablas y visualizar los estudiantes junto con sus cursos y fechas de inscripción.

El resultado permite comprobar las relaciones existentes entre los registros.

## 📁 Archivos del repositorio

- `README.md`: Descripción y documentación del proyecto.
- `base_de_datos.sql`: Script para crear las tablas, insertar datos y realizar consultas.
- `Informe_Practica.pdf`: Documento con el desarrollo de la práctica.
- `capturas/`: Carpeta con evidencias de la configuración, creación de tablas y consultas ejecutadas.

## 📸 Evidencias

El proyecto incluye capturas de pantalla de:

1. Creación del servicio MySQL en Clever Cloud.
2. Configuración de la conexión en MySQL Workbench.
3. Verificación de la conexión remota.
4. Creación de las tres tablas relacionadas.
5. Inserción de registros de prueba.
6. Ejecución de la consulta SQL y visualización de resultados.

## 🔐 Seguridad

Las credenciales de acceso a la base de datos, incluidas las contraseñas, no deben publicarse en el repositorio.

## ✅ Conclusión

Esta práctica permite aplicar los conceptos de bases de datos relacionales, servicios en la nube y conexiones remotas. Además, demuestra cómo MySQL Workbench puede utilizarse para gestionar y consultar información almacenada en un servidor MySQL de Clever Cloud.
