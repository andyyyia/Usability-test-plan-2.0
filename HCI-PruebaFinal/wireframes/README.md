# Rediseño UX - Dashboard Principal

## Problema Identificado
Durante la evaluación heurística, se identificó que el Dashboard carece de **navegación contextual (Breadcrumbs)**, lo que impide al usuario saber exactamente en qué proyecto se encuentra y regresar fácilmente. Además, el estado de carga (feedback del sistema) es muy pobre (solo opacidad), lo que incumple con la heurística de "Visibilidad del estado del sistema".

## Solución Propuesta (Rediseño)
Hemos propuesto un rediseño del Dashboard que integra lo siguiente:

### 1. Leyes de Gestalt Aplicadas
- **Ley de Proximidad:** Las métricas clave (Tarjetas superiores) se agrupan visualmente para que el cerebro las perciba como un solo conjunto de indicadores de éxito.
- **Ley de Semejanza:** Todas las tarjetas de métricas comparten la misma estructura visual (ícono a la izquierda, título, valor grande) para facilitar el escaneo.

### 2. Jerarquía Visual
Se ha dado mayor peso tipográfico a los datos más importantes (ej. Porcentaje de éxito) y se ha dejado en texto secundario los títulos. Se añadió contraste de color a los íconos para guiar la mirada.

### 3. Arquitectura de Información y Navegación Contextual
Se incorporó una **Navegación tipo Breadcrumbs** en la parte superior izquierda:
`Proyectos > [Nombre del Proyecto Activo] > Dashboard`
Esto permite al usuario tener un modelo mental claro de dónde se encuentra en el árbol de navegación.

### 4. Prevención de errores y Feedback visual
Se integrará un *Loading Spinner* o diseño tipo Skeleton cuando los datos estén cargando desde Supabase. Si no hay datos, en lugar de un texto plano, se usarán componentes visuales (empty states) para invitar a la acción.

---

## Evolución de los Wireframes

Los wireframes generados se encuentran en esta misma carpeta:

1. **Lo-Fi (`lo-fi.png`):** Boceto rápido enfocado en estructurar la ubicación de los Breadcrumbs y las tarjetas de métricas.
2. **Mid-Fi (`mid-fi.png`):** Wireframe digital estructurado en escala de grises. Se define el espaciado (padding/margin) y la alineación real de los componentes.
3. **Hi-Fi (`hi-fi.png`):** Diseño final con aplicación de colores (branding), sombras suaves para dar profundidad y tipografía moderna, listo para ser implementado en código.
