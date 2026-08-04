# 09 - Arquitectura de la Aplicación

## Introducción

Este documento describe la arquitectura general del Producto Mínimo Viable (MVP).

Su objetivo es definir cómo se organizará el código fuente, la responsabilidad de cada módulo y la comunicación entre los distintos componentes de la aplicación.

---

# Arquitectura general

La aplicación seguirá una arquitectura simple basada en HTML, CSS y JavaScript (Vanilla JS), priorizando la claridad del código, el mantenimiento y la escalabilidad.

Durante el MVP no se utilizarán frameworks ni librerías externas.

---

# Tecnologías

* HTML5
* CSS3
* JavaScript (ES Modules)
* LocalStorage
* Service Worker
* Web App Manifest
* GitHub Pages

---

# Organización del proyecto

```text
campus/

docs/
src/

assets/
│
├── css/
├── js/
├── icons/
└── images/

index.html
manifest.webmanifest
sw.js
```

---

# Organización del código JavaScript

```text
js/
│
├── app.js
├── storage.js
├── profile.js
├── careers.js
├── study-plan.js
├── subjects.js
├── progress.js
└── ui.js
```

### app.js

Punto de entrada de la aplicación.

### storage.js

Gestiona el acceso a LocalStorage.

### profile.js

Gestiona el perfil del estudiante.

### careers.js

Gestiona las carreras.

### study-plan.js

Gestiona los planes de estudio.

### subjects.js

Gestiona las materias.

### progress.js

Calcula el progreso académico.

### ui.js

Controla la interfaz de usuario.

---

# Persistencia

Toda la información será almacenada en LocalStorage mediante una única estructura de datos.

---

# Funcionamiento Offline

La aplicación utilizará un Service Worker para almacenar los archivos necesarios y permitir su funcionamiento sin conexión.

---

# Escalabilidad

La arquitectura permitirá incorporar en el futuro:

* Backend.
* Base de datos.
* Sincronización.
* Autenticación.
* Inteligencia artificial.
* Nuevos módulos académicos.

La incorporación de estas funcionalidades no requerirá modificar la organización principal del proyecto.
