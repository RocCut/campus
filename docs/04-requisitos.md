# 04 - Requisitos

## Introducción

Este documento define los requisitos funcionales y no funcionales del Producto Mínimo Viable (MVP).

Los requisitos describen el comportamiento esperado de la aplicación y servirán como base para el diseño, desarrollo y pruebas del sistema.

---

# Requisitos Funcionales

## RF-001 — Gestión del perfil

El sistema deberá permitir crear un perfil de estudiante.

---

## RF-002 — Edición del perfil

El sistema deberá permitir modificar la información del perfil en cualquier momento.

---

## RF-003 — Gestión de carreras

El sistema deberá permitir registrar una o más carreras dentro del perfil del estudiante.

---

## RF-004 — Edición de carreras

El sistema deberá permitir modificar la información de cualquier carrera registrada.

---

## RF-005 — Eliminación de carreras

El sistema deberá permitir eliminar una carrera del perfil del estudiante.

---

## RF-006 — Cambio entre carreras

El sistema deberá permitir seleccionar una carrera para consultar y administrar su información académica.

---

## RF-007 — Información de la carrera

Cada carrera deberá almacenar de forma independiente:

* Nombre de la carrera.
* Institución.
* Plan de estudios.

---

## RF-008 — Plan de estudios

El sistema deberá permitir crear manualmente un plan de estudios para cada carrera.

---

## RF-009 — Gestión de materias

El sistema deberá permitir agregar materias al plan de estudios de una carrera.

---

## RF-010 — Edición de materias

El sistema deberá permitir modificar la información de cualquier materia.

---

## RF-011 — Eliminación de materias

El sistema deberá permitir eliminar materias del plan de estudios.

---

## RF-012 — Organización académica

El sistema deberá mostrar las materias organizadas por año y cuatrimestre.

---

## RF-013 — Estado académico

El sistema deberá permitir asignar un estado a cada materia.

Estados iniciales:

* Pendiente.
* Cursando.
* Regularizada.
* Aprobada.

---

## RF-014 — Actualización del estado académico

El sistema deberá permitir modificar el estado de una materia en cualquier momento.

---

## RF-015 — Progreso académico

El sistema deberá calcular automáticamente el progreso de cada carrera a partir del estado de sus materias.

---

## RF-016 — Consulta del progreso

El sistema deberá mostrar para cada carrera:

* Porcentaje de avance.
* Cantidad de materias aprobadas.
* Cantidad de materias cursando.
* Cantidad de materias regularizadas.
* Cantidad de materias pendientes.

---

## RF-017 — Persistencia

El sistema deberá almacenar localmente toda la información del estudiante para conservarla al cerrar la aplicación.

---

# Requisitos No Funcionales

## RNF-001 — Progressive Web App

La aplicación deberá desarrollarse como una Progressive Web App (PWA).

---

## RNF-002 — Instalación

La aplicación deberá poder instalarse en dispositivos compatibles.

---

## RNF-003 — Funcionamiento offline

La aplicación deberá funcionar sin conexión a Internet para todas las funcionalidades del MVP.

---

## RNF-004 — Mobile First

La interfaz deberá diseñarse priorizando dispositivos móviles.

---

## RNF-005 — Usabilidad

La aplicación deberá ofrecer una interfaz simple, intuitiva y fácil de utilizar.

---

## RNF-006 — Almacenamiento local

Toda la información del estudiante permanecerá almacenada únicamente en el dispositivo durante el MVP.

---

## RNF-007 — Sin autenticación

La aplicación no requerirá crear una cuenta ni iniciar sesión para utilizar sus funcionalidades principales.

---

## RNF-008 — Sin backend

Durante el MVP, la aplicación no dependerá de servidores ni bases de datos externas.

---

# Restricciones del MVP

Durante la primera versión del producto:

* Toda la información será cargada manualmente por el estudiante.
* No existirán sugerencias automáticas de universidades, carreras o materias.
* Cada estudiante podrá gestionar una o más carreras.
* Cada carrera tendrá su propio plan de estudios.
* Toda la información permanecerá almacenada localmente.
* No existirá sincronización entre dispositivos.
* No se integrarán servicios externos.

---

# Evolución futura

La arquitectura permitirá incorporar nuevas funcionalidades sin modificar la estructura principal del sistema.

Entre ellas:

* Sincronización en la nube.
* Backend.
* Base de datos.
* Cuentas de usuario.
* Importación de planes de estudio.
* Sugerencias automáticas.
* Integraciones con plataformas académicas.
* Herramientas inteligentes de asistencia al estudiante.
