# 04 - Requisitos

## Introducción

Este documento define los requisitos funcionales y no funcionales del Producto Mínimo Viable (MVP).

Los requisitos describen el comportamiento esperado de la aplicación y servirán como base para el diseño, el desarrollo y las pruebas del sistema.

---

# Requisitos funcionales

## RF-001 Gestión del perfil

El sistema deberá permitir crear un perfil de estudiante.

---

## RF-002 Edición del perfil

El sistema deberá permitir modificar la información del perfil en cualquier momento.

---

## RF-003 Institución

El sistema deberá permitir registrar manualmente el nombre de la institución educativa.

---

## RF-004 Carrera

El sistema deberá permitir registrar manualmente el nombre de la carrera.

---

## RF-005 Plan de estudios

El sistema deberá permitir crear manualmente un plan de estudios.

---

## RF-006 Materias

El sistema deberá permitir agregar materias al plan de estudios.

---

## RF-007 Edición de materias

El sistema deberá permitir modificar la información de cualquier materia.

---

## RF-008 Eliminación de materias

El sistema deberá permitir eliminar materias del plan de estudios.

---

## RF-009 Organización

El sistema deberá mostrar las materias organizadas por año y cuatrimestre.

---

## RF-010 Estado académico

El sistema deberá permitir asignar un estado a cada materia.

Estados iniciales:

* Pendiente
* Cursando
* Regularizada
* Aprobada

---

## RF-011 Actualización del estado

El sistema deberá permitir modificar el estado de una materia.

---

## RF-012 Progreso académico

El sistema deberá calcular automáticamente el progreso de la carrera a partir del estado de las materias.

---

## RF-013 Consulta del progreso

El sistema deberá mostrar el porcentaje de avance y el resumen de materias pendientes, cursando, regularizadas y aprobadas.

---

## RF-014 Persistencia

El sistema deberá almacenar toda la información del usuario localmente para conservarla al cerrar la aplicación.

---

# Requisitos no funcionales

## RNF-001

La aplicación deberá funcionar como una Progressive Web App (PWA).

---

## RNF-002

La aplicación deberá poder instalarse en dispositivos compatibles.

---

## RNF-003

La aplicación deberá funcionar sin conexión a Internet para las funcionalidades del MVP.

---

## RNF-004

La interfaz deberá estar optimizada para dispositivos móviles (Mobile First).

---

## RNF-005

La aplicación deberá ofrecer una interfaz simple, intuitiva y fácil de utilizar.

---

## RNF-006

Toda la información del usuario permanecerá únicamente en su dispositivo durante el MVP.

---

## RNF-007

La aplicación no requerirá crear una cuenta ni iniciar sesión.

---

## RNF-008

El sistema no dependerá de un servidor para funcionar durante el MVP.

---

## Consideraciones

En futuras versiones podrán incorporarse funcionalidades como sincronización entre dispositivos, autenticación, almacenamiento en la nube, importación de planes de estudio e integración con servicios externos, sin modificar los principios definidos para el Producto Mínimo Viable.

