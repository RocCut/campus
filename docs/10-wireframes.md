# 11 - Wireframes

## Introducción

Este documento define los wireframes iniciales del Producto Mínimo Viable (MVP).

Los wireframes representan de manera esquemática las principales pantallas y flujos de interacción de la aplicación.

Su objetivo es visualizar la estructura de la interfaz antes de comenzar el desarrollo, permitiendo validar la navegación y las acciones principales del usuario.

Los wireframes no representan el diseño visual definitivo. Los colores, tipografías, iconografía y otros elementos visuales podrán definirse posteriormente.

---

# 1. Flujo de bienvenida

## WF-001 — Pantalla de bienvenida

**Objetivo:**
Presentar la aplicación al estudiante y permitirle comenzar a configurar su perfil.

```text
┌────────────────────────────┐
│                            │
│         MI CAMPUS          │
│                            │
│  Organiza tu trayectoria   │
│       académica            │
│                            │
│       [ Comenzar ]         │
│                            │
└────────────────────────────┘
```

### Acciones

* Comenzar configuración.

### Resultado esperado

El estudiante accede a la pantalla de creación del perfil.

---

# 2. Flujo de perfil

## WF-002 — Crear perfil

**Objetivo:**
Permitir al estudiante crear su perfil inicial.

```text
┌────────────────────────────┐
│       Crear perfil         │
├────────────────────────────┤
│                            │
│ Nombre                     │
│ [______________________]   │
│                            │
│       [ Continuar ]        │
│                            │
└────────────────────────────┘
```

### Acciones

* Ingresar nombre.
* Continuar.
* Cancelar.

### Resultado esperado

El sistema crea el perfil y permite registrar la primera carrera.

---

## WF-003 — Editar perfil

**Objetivo:**
Permitir modificar la información del perfil.

```text
┌────────────────────────────┐
│       Editar perfil        │
├────────────────────────────┤
│                            │
│ Nombre                     │
│ [______________________]   │
│                            │
│    [ Guardar cambios ]     │
│                            │
└────────────────────────────┘
```

### Acciones

* Modificar nombre.
* Guardar cambios.
* Cancelar.

### Resultado esperado

El sistema actualiza la información del perfil.

---

# 3. Flujo de carreras

## WF-004 — Panel de carreras

**Objetivo:**
Mostrar las carreras registradas por el estudiante y permitir seleccionar una para administrarla.

```text
┌────────────────────────────┐
│         Mi Campus          │
├────────────────────────────┤
│                            │
│ 👤 Nombre del estudiante   │
│                            │
│ Mis carreras               │
│                            │
│ ┌────────────────────────┐ │
│ │ Comunicación Social    │ │
│ │ Universidad X           │ │
│ │ ████████░░ 80%          │ │
│ └────────────────────────┘ │
│                            │
│ ┌────────────────────────┐ │
│ │ Otra carrera           │ │
│ │ Universidad Y           │ │
│ │ ██░░░░░░░░ 20%          │ │
│ └────────────────────────┘ │
│                            │
│    [ + Añadir carrera ]    │
│                            │
└────────────────────────────┘
```

### Acciones

* Seleccionar una carrera.
* Añadir una carrera.
* Acceder al perfil.

### Resultado esperado

El estudiante puede seleccionar la trayectoria académica que desea gestionar.

---

## WF-005 — Crear carrera

**Objetivo:**
Permitir registrar una nueva carrera.

```text
┌────────────────────────────┐
│       Nueva carrera        │
├────────────────────────────┤
│                            │
│ Institución                │
│ [______________________]   │
│                            │
│ Carrera                    │
│ [______________________]   │
│                            │
│      [ Guardar ]           │
│                            │
└────────────────────────────┘
```

### Acciones

* Ingresar institución.
* Ingresar nombre de la carrera.
* Guardar.
* Cancelar.

### Resultado esperado

La nueva carrera queda asociada al perfil del estudiante y aparece en el panel de carreras.

---

## WF-006 — Editar carrera

**Objetivo:**
Permitir modificar la información de una carrera.

```text
┌────────────────────────────┐
│       Editar carrera       │
├────────────────────────────┤
│                            │
│ Institución                │
│ [______________________]   │
│                            │
│ Carrera                    │
│ [______________________]   │
│                            │
│ [ Guardar cambios ]        │
│                            │
│ [ Eliminar carrera ]       │
│                            │
└────────────────────────────┘
```

### Acciones

* Modificar institución.
* Modificar nombre de la carrera.
* Guardar cambios.
* Eliminar carrera.
* Cancelar.

### Resultado esperado

El sistema actualiza la información de la carrera o la elimina si el estudiante confirma la acción.

---

# 4. Flujo del plan de estudios

## WF-007 — Visualizar plan de estudios

**Objetivo:**
Mostrar las materias de la carrera organizadas según su estructura académica.

```text
┌────────────────────────────┐
│ ← Comunicación Social      │
├────────────────────────────┤
│                            │
│ Progreso: 60%              │
│                            │
│ 1.º AÑO                    │
│                            │
│ ✓ Introducción             │
│ ✓ Historia                 │
│ ○ Sociología               │
│                            │
│ 2.º AÑO                    │
│                            │
│ ✓ Comunicación             │
│ ○ Economía                 │
│ ○ Teoría                   │
│                            │
│     [ + Añadir materia ]   │
│                            │
└────────────────────────────┘
```

### Acciones

* Consultar materias.
* Seleccionar una materia.
* Añadir una materia.
* Volver al panel de carreras.

### Resultado esperado

El estudiante puede consultar rápidamente la estructura de su carrera y el estado de sus materias.

---

# 5. Flujo de materias

## WF-008 — Crear materia

**Objetivo:**
Permitir agregar manualmente una materia al plan de estudios.

```text
┌────────────────────────────┐
│       Nueva materia        │
├────────────────────────────┤
│                            │
│ Nombre                     │
│ [______________________]   │
│                            │
│ Año                        │
│ [ 1 ▼ ]                    │
│                            │
│ Cuatrimestre               │
│ [ 1 ▼ ]                    │
│                            │
│ Estado                     │
│ [ Pendiente ▼ ]            │
│                            │
│ Observaciones              │
│ [______________________]   │
│ [______________________]   │
│                            │
│       [ Guardar ]          │
│                            │
└────────────────────────────┘
```

### Acciones

* Ingresar nombre.
* Seleccionar año.
* Seleccionar cuatrimestre.
* Seleccionar estado.
* Agregar observaciones.
* Guardar.
* Cancelar.

### Resultado esperado

La materia se incorpora al plan de estudios de la carrera.

---

## WF-009 — Editar materia

**Objetivo:**
Permitir modificar la información de una materia existente.

```text
┌────────────────────────────┐
│       Editar materia       │
├────────────────────────────┤
│                            │
│ Nombre                     │
│ [______________________]   │
│                            │
│ Año                        │
│ [ 2 ▼ ]                    │
│                            │
│ Cuatrimestre               │
│ [ 1 ▼ ]                    │
│                            │
│ Estado                     │
│ [ Aprobada ▼ ]             │
│                            │
│ Observaciones              │
│ [______________________]   │
│ [______________________]   │
│                            │
│ [ Guardar cambios ]        │
│                            │
│ [ Eliminar materia ]       │
│                            │
└────────────────────────────┘
```

### Acciones

* Modificar nombre.
* Modificar año.
* Modificar cuatrimestre.
* Modificar estado.
* Modificar observaciones.
* Guardar cambios.
* Eliminar materia.
* Cancelar.

### Resultado esperado

El sistema actualiza o elimina la materia según la acción seleccionada.

---

# 6. Flujo de progreso académico

## WF-010 — Consultar progreso

**Objetivo:**
Permitir al estudiante visualizar su avance en una carrera.

```text
┌────────────────────────────┐
│      Mi progreso           │
├────────────────────────────┤
│                            │
│ Comunicación Social        │
│                            │
│       ███████░░░           │
│           70%              │
│                            │
│ ✓ Aprobadas       28       │
│ ⏳ Cursando         4       │
│ ◐ Regularizadas    3       │
│ ○ Pendientes       9       │
│                            │
└────────────────────────────┘
```

### Acciones

* Consultar progreso.
* Volver al plan de estudios.
* Cambiar de carrera.

### Resultado esperado

El sistema muestra el progreso correspondiente exclusivamente a la carrera seleccionada.

---

# 7. Navegación principal

La navegación inicial del MVP seguirá una estructura simple:

```text
                 ┌──────────────┐
                 │   Bienvenida │
                 └──────┬───────┘
                        ↓
                 ┌──────────────┐
                 │    Perfil    │
                 └──────┬───────┘
                        ↓
              ┌────────────────────┐
              │  Panel de carreras │
              └─────────┬──────────┘
                        ↓
                 ┌──────────────┐
                 │    Carrera   │
                 └──────┬───────┘
                        ↓
              ┌────────────────────┐
              │  Plan de estudios  │
              └─────────┬──────────┘
                        ↓
                 ┌──────────────┐
                 │    Materia   │
                 └──────────────┘
```

El estudiante podrá regresar a niveles anteriores mediante la navegación de la aplicación.

---

# 8. Principios de los wireframes

Los wireframes deberán respetar los siguientes principios:

* **Mobile First:** las pantallas se diseñarán primero para dispositivos móviles.
* **Simplicidad:** cada pantalla deberá presentar únicamente las acciones necesarias.
* **Acceso rápido:** la información académica importante deberá estar disponible con pocos pasos.
* **Consistencia:** las acciones similares deberán comportarse de la misma manera en toda la aplicación.
* **Independencia entre carreras:** cada carrera deberá mantener su propio plan de estudios y progreso.
* **Carga manual:** durante el MVP, el estudiante ingresará manualmente la información.
* **Offline First:** las pantallas principales deberán poder utilizarse sin conexión a Internet.

---

# 9. Alcance de los wireframes

Estos wireframes corresponden al MVP inicial.

No se incluyen todavía interfaces para:

* Apuntes.
* Archivos.
* Compañeros.
* Horarios.
* Exámenes.
* Calendario.
* Recordatorios.
* Backend.
* Sincronización.
* Funciones de inteligencia artificial.

Estas funcionalidades podrán incorporarse posteriormente junto con sus respectivos wireframes.

