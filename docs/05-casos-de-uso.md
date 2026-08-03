# 05 - Casos de Uso

## Introducción

Los casos de uso describen cómo interactúa el estudiante con la aplicación para alcanzar un objetivo específico.

Cada caso de uso representa una tarea importante dentro del Producto Mínimo Viable (MVP) y servirá como guía para el diseño de la interfaz y el desarrollo de las funcionalidades.

---

# CU-001 Crear perfil

**Actor principal**

Estudiante.

**Objetivo**

Crear el perfil inicial de la aplicación.

**Flujo principal**

1. El estudiante abre la aplicación por primera vez.
2. El sistema muestra la pantalla de bienvenida.
3. El estudiante ingresa su nombre.
4. El estudiante ingresa el nombre de la institución.
5. El estudiante ingresa el nombre de la carrera.
6. El estudiante guarda la información.
7. El sistema almacena los datos localmente.
8. El sistema muestra la pantalla principal.

---

# CU-002 Crear plan de estudios

**Actor principal**

Estudiante.

**Objetivo**

Crear manualmente el plan de estudios.

**Flujo principal**

1. El estudiante accede al apartado "Plan de estudios".
2. Selecciona "Agregar materia".
3. Ingresa el nombre de la materia.
4. Indica el año correspondiente.
5. Indica el cuatrimestre.
6. Guarda la materia.
7. El sistema incorpora la materia al plan.

Este proceso puede repetirse hasta completar el plan de estudios.

---

# CU-003 Editar una materia

**Actor principal**

Estudiante.

**Objetivo**

Modificar la información de una materia.

**Flujo principal**

1. El estudiante selecciona una materia.
2. El sistema muestra su información.
3. El estudiante modifica los datos necesarios.
4. Guarda los cambios.
5. El sistema actualiza la información.

---

# CU-004 Cambiar el estado de una materia

**Actor principal**

Estudiante.

**Objetivo**

Actualizar la situación académica de una materia.

**Flujo principal**

1. El estudiante abre una materia.
2. Selecciona el estado correspondiente.
3. Guarda los cambios.
4. El sistema actualiza la materia.
5. El progreso académico se recalcula automáticamente.

---

# CU-005 Consultar el plan de estudios

**Actor principal**

Estudiante.

**Objetivo**

Visualizar la estructura completa de la carrera.

**Flujo principal**

1. El estudiante abre el plan de estudios.
2. El sistema muestra las materias organizadas por año y cuatrimestre.
3. El estudiante consulta la información.

---

# CU-006 Consultar el progreso académico

**Actor principal**

Estudiante.

**Objetivo**

Conocer el avance en la carrera.

**Flujo principal**

1. El estudiante accede a la sección de progreso.
2. El sistema calcula el avance.
3. El sistema muestra:

   * porcentaje de avance;
   * materias aprobadas;
   * materias cursando;
   * materias regularizadas;
   * materias pendientes.

---

# CU-007 Editar el perfil

**Actor principal**

Estudiante.

**Objetivo**

Actualizar los datos del perfil.

**Flujo principal**

1. El estudiante accede a su perfil.
2. Modifica los datos deseados.
3. Guarda los cambios.
4. El sistema actualiza la información.

---

# CU-008 Continuar utilizando la aplicación

**Actor principal**

Estudiante.

**Objetivo**

Recuperar la información previamente almacenada.

**Flujo principal**

1. El estudiante abre la aplicación.
2. El sistema carga automáticamente los datos almacenados.
3. Se muestra la pantalla principal con toda la información disponible.

---

## Observaciones

Los casos de uso del MVP se centran exclusivamente en la gestión manual de la trayectoria académica.

No contemplan autenticación, sincronización en la nube ni integración con servicios externos. Estas funcionalidades podrán incorporarse en futuras versiones sin alterar el flujo principal de uso de la aplicación.

