# CLAUDE.md — MAPA_MANTENEDOR_ALGARROBO

## ¿Qué es este proyecto?
Este proyecto es un geoportal ligero basado en FastAPI, DuckDB, y SpatiaLite. Permite evaluar las restricciones territoriales interactuando sobre un mapa web. - `etl/`: Pipeline en Python y DuckDB para generar y procesar las capas vectoriales, construyendo la base de datos `chile_territorial.sqlite`. - `backend/`: API en FastAPI que responde a las consultas espaciales simultáneas utilizando SpatiaLite y modo WAL.

---

## Comandos de Referencia Rápida
Este es un proyecto Fullstack con frontend de Node y backend de Python.

### Frontend (React/Node)
- **Iniciar servidor de desarrollo:** `cd frontend && npm run dev`
- **Compilar para producción:** `cd frontend && npm run build`
- **Ejecutar pruebas (Tests):** `cd frontend && npm test`
- **Lint / Formateo:** `cd frontend && npm run lint`

### Backend (Python)
- **Ejecutar servidor local:** `python -m uvicorn main:app --reload`
- **Instalar dependencias:** `pip install -r requirements.txt`
- **Ejecutar pruebas:** `pytest`

## Tecnología y Stack
- **Frontend:** React / Node.js (Vite: True, TS: False, React: True)
- **Backend:** Python (FastAPI)

## Guía de Estilo y Convenciones
- **Idioma del código:** Inglés para infraestructura, nombres de variables y funciones. Español para comentarios de negocio e interfaz de usuario.
- **Frontend JavaScript/TypeScript:** Estilo `camelCase` para variables y funciones, `PascalCase` para componentes React y tipos. Cumplir con ESLint/Prettier.
- **Backend Python:** Cumplir con PEP 8. Estilo `snake_case` para variables, funciones y nombres de archivos; `PascalCase` para clases.
- **Trazabilidad:** Cada cambio debe rastrearse directamente a un requerimiento o corrección solicitada.


## Directrices de Desarrollo (Claude Code)

### 1. Pensar antes de Codificar
- **No asumas:** Si hay ambigüedad o múltiples interpretaciones, pregunta antes de codificar.
- **Simplifica:** Elige el camino más simple y limpio. Evita la sobreingeniería y abstracciones innecesarias.

### 2. Cambios Quirúrgicos
- Modifica únicamente las líneas necesarias para cumplir el objetivo.
- No realices refactorizaciones no solicitadas en código adyacente.
- Respeta estrictamente el formato y estilo del archivo existente.

### 3. Ejecución Orientada a Objetivos
- Define el criterio de éxito para cada cambio.
- Comprueba que tus modificaciones no introduzcan errores de compilación o de linting.
