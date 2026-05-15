# Evidencia de uso de Inteligencia Artificial (IA)

Para la realización de esta prueba práctica, se utilizó la asistencia de un agente IA avanzado (Google Gemini 3.1 Pro) como UX Engineer & Developer. A continuación se documenta el proceso y los prompts utilizados.

## 1. Herramienta Utilizada
- **IA:** Gemini 3.1 Pro y Gemini Banana
- **Rol:** UX/UI Engineer Assistant
- **Capacidades usadas:** Análisis de código fuente (React/TS), Generación de imágenes (DALL-E / Imagen para wireframes), y refactorización de código.

## 2. Documentación de Prompts Utilizados

### Para la Evaluación Heurística
**Prompt del humano:** 
> "Analiza el código del archivo `Dashboard.tsx` y otros componentes principales. Identifica problemas de usabilidad reales basándote en las 10 heurísticas de Nielsen y clasifícalos por severidad (Crítico, Moderado, Leve)."
**Resultado:** La IA leyó el código y detectó problemas reales, como la falta de Breadcrumbs (Navegación) y el uso de un simple `opacity-50` para el estado de carga, lo cual violaba la heurística de "Visibilidad del estado del sistema".

### Para la Generación de Wireframes
**Prompts para DALL-E / Generador de Imágenes:**
> **Lo-Fi:** "Boceto a mano alzada (estructura básica) de un panel de análisis para pruebas de usabilidad. Presenta una ruta de navegación en la parte superior, un diseño limpio con cuatro tarjetas de indicadores clave de rendimiento (KPI) y dos gráficos en la parte inferior. Trazos sencillos, estilo lápiz, minimalista"
> 
> **Mid-Fi:** "Un wireframe digital en escala de grises de un panel de pruebas de usabilidad. Muestra navegación tipo "breadcrumbs" en la parte superior, 4 tarjetas de métricas. Espaciado profesional, diseño estructurado, sin colores."
> 
> **Hi-Fi:** "Diseño de interfaz de usuario moderno y de alta fidelidad para un panel de análisis de pruebas de usabilidad. Interfaz de aplicación web limpia y estética. Incluye navegación superior con breadcrumbs."

**Resultado:** Tres imágenes (`lo-fi.png`, `mid-fi.png`, `hi-fi.png`) que sirvieron como referencia visual para el rediseño antes de codificarlo.

### Para la Implementación en Código
**Prompt del humano:**
> "Modifica el archivo `Dashboard.tsx` para implementar los Breadcrumbs y el nuevo Feedback visual de carga (Spinner en lugar de opacidad) siguiendo las leyes de Gestalt de los wireframes generados."
**Resultado:** La IA inyectó directamente los componentes `Loader2`, `ChevronRight` y `Home` de `lucide-react`, e implementó la lógica condicional `{isLoading ? <Spinner /> : <Dashboard />}` respetando el flujo de React.

## 3. Conclusión de cómo ayudó la IA en el diseño UX
La IA no solo actuó como un generador de código, sino como un **compañero de diseño (Design Partner)**. Ayudó a:
1. **Identificar problemas "invisibles"** a simple vista (como la falta de feedback de estado en peticiones asíncronas).
2. **Aplicar teoría sólida** (Leyes de Gestalt y heurísticas) para justificar los cambios técnicos.
3. **Agilizar el proceso de prototipado**, pasando de la teoría a wireframes visuales en minutos, lo que permitió validar la solución antes de escribir una sola línea de código en el archivo `Dashboard.tsx`.
