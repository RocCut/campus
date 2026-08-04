# 06 - Modelo de Datos

## Introducción

Este documento define las entidades principales del Producto Mínimo Viable (MVP), sus atributos y las relaciones entre ellas.

El modelo de datos representa la estructura lógica de la información que gestionará la aplicación y servirá como base para la implementación en JavaScript y el almacenamiento local.

---

# Modelo conceptual

```text
Perfil (1)
│
└── Carreras (1..N)
      │
      ├── Institución
      ├── Nombre
      ├── Plan de Estudios (1)
      │      │
      │      └── Materias (1..N)
      │
      └── Progreso
```

---

# Entidad: Perfil

Representa al estudiante que utiliza la aplicación.

| Atributo           | Tipo   | Descripción                     |
| ------------------ | ------ | ------------------------------- |
| id                 | UUID   | Identificador único del perfil. |
| nombre             | String | Nombre del estudiante.          |
| fechaCreacion      | Date   | Fecha de creación del perfil.   |
| fechaActualizacion | Date   | Última modificación del perfil. |

---

# Entidad: Carrera

Representa una carrera gestionada por el estudiante.

Un perfil puede registrar una o más carreras.

| Atributo           | Tipo   | Descripción                            |
| ------------------ | ------ | -------------------------------------- |
| id                 | UUID   | Identificador único de la carrera.     |
| nombre             | String | Nombre de la carrera.                  |
| institucion        | String | Institución donde se cursa la carrera. |
| fechaCreacion      | Date   | Fecha de creación del registro.        |
| fechaActualizacion | Date   | Última modificación.                   |

---

# Entidad: Plan de Estudios

Representa el conjunto de materias que pertenecen a una carrera.

Cada carrera posee un único plan de estudios.

| Atributo      | Tipo   | Descripción                             |
| ------------- | ------ | --------------------------------------- |
| id            | UUID   | Identificador del plan de estudios.     |
| nombre        | String | Nombre del plan (ej.: Plan 2024).       |
| descripcion   | String | Descripción opcional.                   |
| totalMaterias | Number | Cantidad total de materias registradas. |

---

# Entidad: Materia

Representa una asignatura perteneciente al plan de estudios de una carrera.

| Atributo      | Tipo   | Descripción                        |
| ------------- | ------ | ---------------------------------- |
| id            | UUID   | Identificador único de la materia. |
| nombre        | String | Nombre de la materia.              |
| año           | Number | Año al que pertenece.              |
| cuatrimestre  | Number | Cuatrimestre correspondiente.      |
| estado        | Enum   | Estado académico de la materia.    |
| observaciones | String | Notas opcionales del estudiante.   |

## Estados académicos

* Pendiente.
* Cursando.
* Regularizada.
* Aprobada.

---

# Relaciones entre entidades

## Perfil → Carrera

* Un perfil puede tener una o más carreras.
* Cada carrera pertenece a un único perfil.

**Cardinalidad:** 1 : N

---

## Carrera → Plan de Estudios

* Cada carrera posee un único plan de estudios.
* Cada plan de estudios pertenece a una única carrera.

**Cardinalidad:** 1 : 1

---

## Plan de Estudios → Materia

* Un plan de estudios contiene una o más materias.
* Cada materia pertenece a un único plan de estudios.

**Cardinalidad:** 1 : N

---

# Persistencia

Durante el MVP:

* Toda la información se almacenará utilizando `localStorage`.
* No existirá sincronización entre dispositivos.
* No se utilizará una base de datos externa.
* La aplicación funcionará completamente sin conexión a Internet.

---

# Evolución del modelo

La estructura fue diseñada para permitir el crecimiento de la aplicación sin modificar su arquitectura principal.

En futuras versiones podrán incorporarse nuevas entidades, como por ejemplo:

* Profesor.
* Horario.
* Examen.
* Trabajo práctico.
* Bibliografía.
* Apunte.
* Archivo adjunto.
* Compañero.
* Calendario académico.
* Cuenta de usuario.
* Sincronización en la nube.

---

# Consideraciones de diseño

* Cada carrera será completamente independiente de las demás.
* El progreso académico se calculará por carrera.
* El estudiante podrá administrar una o más carreras desde un único perfil.
* Todas las entidades utilizarán identificadores únicos (UUID) para facilitar una futura migración a un backend o base de datos.
* El modelo prioriza la simplicidad para el MVP, manteniendo una estructura escalable para futuras versiones.

