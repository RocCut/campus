# 07 - Decisiones de Arquitectura

## Introducción

Este documento registra las decisiones de arquitectura tomadas durante el diseño del proyecto.

Su objetivo es documentar el razonamiento detrás de las principales decisiones técnicas y funcionales, facilitando la evolución del sistema y evitando perder el contexto de por qué fueron adoptadas.

---

## DA-001 — Aplicación Offline First

**Decisión**

La aplicación deberá funcionar sin conexión a Internet para todas las funcionalidades del Producto Mínimo Viable (MVP).

**Motivación**

El estudiante debe poder consultar y gestionar su información académica en cualquier momento, incluso sin acceso a Internet.

**Consecuencia**

Toda la información del MVP se almacenará localmente en el dispositivo.

---

## DA-002 — Gestión manual de la información

**Decisión**

El estudiante ingresará manualmente toda la información relacionada con su institución, carreras, plan de estudios y materias.

**Motivación**

Eliminar la dependencia de bases de datos externas y permitir que cualquier estudiante pueda comenzar a utilizar la aplicación inmediatamente.

**Consecuencia**

En futuras versiones podrán incorporarse sugerencias, importaciones o sincronización, sin reemplazar la carga manual.

---

## DA-003 — Arquitectura Mobile First

**Decisión**

La interfaz será diseñada priorizando dispositivos móviles.

**Motivación**

La mayor parte de los estudiantes consulta su información académica desde el teléfono.

**Consecuencia**

Las pantallas deberán adaptarse correctamente a distintos tamaños de dispositivo.

---

## DA-004 — Soporte para múltiples carreras

**Decisión**

Un mismo perfil podrá administrar una o más carreras.

**Motivación**

Existen estudiantes que cursan simultáneamente más de una carrera o cambian de institución y desean conservar su historial académico en la aplicación.

**Consecuencia**

La entidad Perfil dejará de contener una única carrera y pasará a administrar una colección de carreras, cada una con su propio plan de estudios y conjunto de materias.

---

## DA-005 — Evolución gradual de la arquitectura

**Decisión**

El MVP no utilizará backend ni sincronización en la nube.

**Motivación**

Priorizar un desarrollo simple, estable y completamente funcional antes de incorporar infraestructura adicional.

**Consecuencia**

La arquitectura deberá permitir la incorporación futura de un backend sin requerir un rediseño completo del sistema.
