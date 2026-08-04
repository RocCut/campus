# 05 - Casos de Uso

## Introducción

Los casos de uso describen cómo interactúa el estudiante con la aplicación para alcanzar un objetivo específico.

Cada caso de uso representa una funcionalidad principal del Producto Mínimo Viable (MVP) y servirá como guía para el diseño de la interfaz y el desarrollo de la aplicación.

---

# CU-001 — Crear perfil

**Actor principal**

Estudiante.

**Objetivo**

Crear el perfil inicial de la aplicación.

**Flujo principal**

1. El estudiante abre la aplicación por primera vez.
2. El sistema muestra la pantalla de bienvenida.
3. El estudiante ingresa su nombre.
4. Guarda la información.
5. El sistema crea el perfil.
6. El sistema invita al estudiante a registrar su primera carrera.

---

# CU-002 — Registrar una carrera

**Actor principal**

Estudiante.

**Objetivo**

Registrar una nueva carrera.

**Flujo principal**

1. El estudiante selecciona "Añadir carrera".
2. Ingresa el nombre de la institución.
3. Ingresa el nombre de la carrera.
4. Guarda la información.
5. El sistema crea la carrera.
6. El sistema muestra el panel de la carrera.

---

# CU-003 — Cambiar entre carreras

**Actor principal**

Estudiante.

**Objetivo**

Consultar o administrar una carrera específica.

**Flujo principal**

1. El estudiante accede al listado de carreras.
2. Selecciona una carrera.
3. El sistema carga el plan de estudios correspondiente.
4. El estudiante comienza a gestionar esa carrera.

---

# CU-004 — Editar una carrera

**Actor principal**

Estudiante.

**Objetivo**

Modificar la información de una carrera.

**Flujo principal**

1. El estudiante abre la configuración de una carrera.
2. Modifica el nombre de la institución o de la carrera.
3. Guarda los cambios.
4. El sistema actualiza la información.

---

# CU-005 — Eliminar una carrera

**Actor principal**

Estudiante.

**Objetivo**

Eliminar una carrera del perfil.

**Flujo principal**

1. El estudiante selecciona una carrera.
2. Elige la opción "Eliminar".
3. El sistema solicita confirmación.
4. El estudiante confirma la acción.
5. El sistema elimina la carrera y toda la información asociada.

---

# CU-006 — Crear el plan de estudios

**Actor principal**

Estudiante.

**Objetivo**

Crear manualmente el plan de estudios de una carrera.

**Flujo principal**

1. El estudiante abre una carrera.
2. Accede al apartado "Plan de estudios".
3. Selecciona "Agregar materia".
4. Ingresa el nombre de la materia.
5. Indica el año.
6. Indica el cuatrimestre.
7. Guarda la materia.
8. El sistema la incorpora al plan de estudios.

Este proceso puede repetirse hasta completar el plan.

---

# CU-007 — Editar una materia

**Actor principal**

Estudiante.

**Objetivo**

Modificar la información de una materia.

**Flujo principal**

1. El estudiante selecciona una materia.
2. El sistema muestra su información.
3. El estudiante modifica los datos necesarios.
4. Guarda los cambios.
5. El sistema actualiza la materia.

---

# CU-008 — Cambiar el estado académico

**Actor principal**

Estudiante.

**Objetivo**

Actualizar el estado académico de una materia.

**Flujo principal**

1. El estudiante abre una materia.
2. Selecciona un nuevo estado.
3. Guarda los cambios.
4. El sistema actualiza la materia.
5. El sistema recalcula automáticamente el progreso de la carrera.

---

# CU-009 — Consultar el plan de estudios

**Actor principal**

Estudiante.

**Objetivo**

Visualizar la estructura académica de una carrera.

**Flujo principal**

1. El estudiante selecciona una carrera.
2. Accede al plan de estudios.
3. El sistema muestra las materias organizadas por año y cuatrimestre.

---

# CU-010 — Consultar el progreso académico

**Actor principal**

Estudiante.

**Objetivo**

Conocer el avance de una carrera.

**Flujo principal**

1. El estudiante selecciona una carrera.
2. Accede a la sección de progreso.
3. El sistema calcula automáticamente el avance.
4. El sistema muestra:

   * porcentaje de avance;
   * materias aprobadas;
   * materias cursando;
   * materias regularizadas;
   * materias pendientes.

---

# CU-011 — Editar el perfil

**Actor principal**

Estudiante.

**Objetivo**

Actualizar la información del perfil.

**Flujo principal**

1. El estudiante accede a su perfil.
2. Modifica los datos deseados.
3. Guarda los cambios.
4. El sistema actualiza la información.

---

# CU-012 — Recuperar la información almacenada

**Actor principal**

Estudiante.

**Objetivo**

Continuar utilizando la aplicación sin perder la información registrada.

**Flujo principal**

1. El estudiante abre la aplicación.
2. El sistema carga automáticamente la información almacenada localmente.
3. El sistema muestra el listado de carreras.
4. El estudiante selecciona la carrera que desea consultar.

---

# Observaciones

* Un perfil puede gestionar una o más carreras.
* Cada carrera mantiene su propio plan de estudios, materias y progreso académico.
* Todas las funcionalidades del MVP estarán disponibles sin conexión a Internet.
* Toda la información será ingresada manualmente por el estudiante y almacenada localmente en el dispositivo.
