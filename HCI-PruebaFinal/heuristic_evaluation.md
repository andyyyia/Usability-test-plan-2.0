# Evaluación Heurística - Usability Test Dashboard 2.0

Se aplicaron las 10 Heurísticas de Usabilidad de Jakob Nielsen para evaluar el estado actual del aplicativo. Se identificaron 10 problemas principales clasificados por severidad.

## 1. Visibilidad del estado del sistema
- **Problema 1 (Crítico):** Al cargar el Dashboard, la pantalla simplemente reduce su opacidad al 50% (`opacity-50`) sin mostrar un *spinner* o indicador de carga claro. El usuario no sabe si el sistema se colgó o está cargando.
- **Problema 2 (Moderado):** Al guardar un formulario de "Nueva Observación", no hay un feedback visual inmediato o mensaje de éxito claro (Toast) que confirme que la acción se realizó correctamente antes de redirigir.

## 2. Relación entre el sistema y el mundo real
- **Problema 3 (Menor):** Algunas métricas en el Dashboard ("Tiempo Promedio") se muestran como texto estático sin una unidad clara (ej. solo dice "0" en lugar de "0 min" o "0 s" dependiendo de los datos iniciales).

## 3. Control y libertad del usuario
- **Problema 4 (Crítico):** Falta de **Navegación Contextual (Breadcrumbs)**. Al estar dentro de la pantalla de "Hallazgos" o "Dashboard", el usuario no tiene una forma rápida de volver a la vista general de proyectos sin usar el menú lateral.
- **Problema 5 (Moderado):** En formularios extensos (como la creación de un guion), si el usuario hace clic en cancelar por error, se pierde todo el progreso sin posibilidad de deshacer.

## 4. Consistencia y estándares
- **Problema 6 (Moderado):** La jerarquía visual de los botones de acción ("Guardar", "Cancelar", "Nuevo") varía en tamaño y contraste en diferentes pantallas, lo que rompe la consistencia.

## 5. Prevención de errores
- **Problema 7 (Crítico):** No hay diálogos de confirmación (Modal) al intentar eliminar un proyecto o un hallazgo, lo que puede resultar en la pérdida accidental de datos críticos.

## 6. Reconocer antes que recordar
- **Problema 8 (Menor):** En los gráficos del Dashboard, si no hay datos (`severityData.every(d => d.value === 0)`), solo se muestra un texto gris que dice "No hay hallazgos". Falta una ilustración o un *empty state* que guíe al usuario sobre qué hacer.

## 7. Flexibilidad y eficiencia de uso
- **Problema 9 (Moderado):** La tabla de observaciones recientes no cuenta con filtros ni paginación, obligando a los usuarios avanzados a hacer *scroll* interminable si el proyecto tiene muchas pruebas.

## 8. Diseño estético y minimalista
- **Problema 10 (Menor):** Carga visual excesiva en los listados debido a la falta de espacio en blanco (padding/margin) entre las tarjetas de proyectos o tarjetas de métricas.

---
**Resumen de Hallazgos:**
- **Críticos:** 3
- **Moderados:** 4
- **Leves / Menores:** 3
