# Sprint Planning

**Objetivo del Sprint:** Mejorar la orientación del usuario dentro del sistema y proporcionar retroalimentación visual inmediata durante la carga de datos en el Dashboard.

## Selección de Historias de Usuario (Sprint Backlog)

Hemos seleccionado las siguientes historias para este Sprint debido a su alto impacto en la usabilidad y facilidad de implementación en el tiempo establecido (2 horas de la prueba).

### 1. US-01: Breadcrumbs (Navegación Contextual)
- **Descripción:** Implementar migas de pan en la cabecera de las vistas principales (Dashboard, Tareas, etc.) para que el usuario sepa en qué proyecto está.
- **Responsable:** UX Engineer
- **Estimación:** 3 Puntos
- **Criterios de Aceptación:**
  - Debe mostrar `Proyectos > [Nombre del Proyecto] > Dashboard`.
  - Debe ser visible en todas las pantallas dentro de un proyecto seleccionado.

### 2. US-02: Feedback de Carga (Spinner)
- **Descripción:** Cambiar la opacidad estática del 50% por un spinner circular o un diseño Skeleton mientras se obtienen los datos de la API de Supabase en el Dashboard.
- **Responsable:** UX Engineer
- **Estimación:** 2 Puntos
- **Criterios de Aceptación:**
  - El usuario debe ver claramente que el sistema está trabajando.
  - La interfaz no debe ser interactiva mientras los datos cargan.

## Capacidad del Equipo
- **Total Puntos Comprometidos:** 5 Puntos
- **Duración del Sprint:** 1 Semana (adaptado para el examen de 2 horas).
