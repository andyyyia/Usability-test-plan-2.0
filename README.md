# Usability Test Dashboard 2.0 - Prueba Práctica HCI

Esta es la resolución de la Prueba Práctica Final de la asignatura de **Interacción Humano / Computador (HCI)**.

## Resolución del Examen

Toda la documentación, análisis y evidencia requeridos para el examen se encuentran organizados dentro del directorio **[`HCI-PruebaFinal/`](./HCI-PruebaFinal/)**. 

Estructura de la entrega:
- `product_backlog.md` y `sprint_planning.md` (Fase 1 - Scrum)
- `heuristic_evaluation.md` (Fase 2 - Evaluación de 10 problemas UX)
- `wireframes/` (Fase 3 - Rediseño UX con Lo-Fi, Mid-Fi y Hi-Fi)
- `implementation/` (Fase 4 - Documentación de cambios en el código)
- `ai_evidence.md` (Fase 5 - Prompts y uso de IA en el proceso)

### Funcionalidad Modificada
Se implementó una mejora UX real en `src/app/pages/Dashboard.tsx` agregando:
1. **Breadcrumbs** para la navegación contextual.
2. **Spinner animado (Feedback Visual)** durante la carga de datos.

---

## Para ejecutar el proyecto en desarrollo:

1. Instalar dependencias:
```bash
npm install
```
2. Ejecutar el servidor:
```bash
npm run dev
```