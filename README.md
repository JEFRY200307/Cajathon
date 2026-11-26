# WENANCE.AI — Weather + Finance

Plataforma de IA agéntica que anticipa los riesgos climáticos de los microempresarios financiados por **Caja Trujillo** y los convierte en estrategias preventivas ejecutables, con supervisión humana y guardrails.

Hackathon Caja Trujillo · Eje 4 · Inclusión financiera y resiliencia — Microfinanzas resilientes al clima.

## Prototipo funcional

`index.html` (y `prototipo/index.html`) es una página autocontenida: ábrela en el navegador o publícala con GitHub Pages (Settings → Pages → Branch `main` / root).

Flujo de demo (guía en la parte superior de la app):

1. Simular comunicado ENFEN → riesgo recalculado y estrategias IA.
2. Abrir la ficha: por qué este cliente o segmento (exposición, vulnerabilidad, capacidad de pago).
3. Crear una regla en lenguaje natural (p. ej. "no reprogramar a quien tenga más de 30 días de atraso") → la IA regenera las estrategias.
4. Aprobar (Sí / No / Modificar) en el Kanban.
5. Ver un guardrail bloquear una acción y escalarla al jefe de riesgos (4-eyes); kill switch disponible.
6. KPIs y resultado medido.

Incluye 5,000 clientes sintéticos (Piura, Lambayeque, La Libertad), mapa de riesgo, what-if, motor de políticas (P-01…P-09), catálogo de acciones A1–A7, modos del agente M0–M5 y auditoría con hash encadenado.

> Datos sintéticos y core bancario simulado. La traducción de reglas y la redacción de estrategias usan lógica determinista en lugar de un LLM real para que la demo funcione sin conexión.

## Documentación

- `docs/WENANCE_AI_Design_System_y_Arquitectura_C4.pdf` — design system (colores, tipografía, tokens, componentes), modelo C4 (contexto, contenedores, componentes), vista dinámica, flujos de proceso y automatización, modos, acciones y guardrails.
- `docs/diagramas/mermaid/` — fuentes Mermaid de todos los diagramas (`npx @mermaid-js/mermaid-cli -i archivo.mmd -c config.json`).
- `docs/diagramas/svg/` — diagramas renderizados.

## Stack propuesto

Python, pandas/GeoPandas, LightGBM, SHAP, OR-Tools, FastAPI, PostgreSQL + PostGIS, Redis Streams, LangGraph + API de LLM, OPA/Rego, React.
