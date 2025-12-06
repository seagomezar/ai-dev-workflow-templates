# Flujo de Trabajo y Reglas del Agente de IA

Este documento describe el procedimiento operativo estándar para cualquier asistente de IA (como Gemini CLI, Cursor, etc.) trabajando en un proyecto. Todas las acciones deben adherirse a este flujo de trabajo.

## 1. Flujo de Trabajo Central

1.  **Acción Inicial:** Al comenzar cualquier nueva interacción o tarea, tu primer paso es leer y entender este documento (`AGENTS.md`) en su totalidad.

2.  **Análisis de Tarea y Coincidencia de Plantilla:**
    *   Para cualquier solicitud, primero verifica el directorio de plantillas del proyecto (ej., `templates/`, `@ai_docs/templates/`, o similar) para ver si existe una plantilla específica para la tarea solicitada (ej., `002_bug_fix_template.md`, `003_code_review_template.md`, `004_git_commit_workflow.md`).
    *   Si la solicitud es arreglar un error, **debes** usar la plantilla `002_bug_fix_template.md` como tu guía.
    *   Si se encuentra una plantilla coincidente, **debes** seguir las instrucciones proporcionadas dentro de esa plantilla para ejecutar la tarea.

3.  **Nueva Característica o Implementación de Desarrollo:**
    *   Si la solicitud implica crear una nueva característica, implementar código nuevo o cualquier forma de nuevo desarrollo, **debes** usar `001_task_planning_template.md` como tu guía.
    *   Tu salida principal será un nuevo documento de tarea detallado. Este documento debe crearse como un nuevo archivo `.md` dentro de la carpeta de tareas del proyecto (ej., `tasks/`, `@ai_docs/tasks/`, o similar).
    *   El contenido y estructura de este nuevo documento de tarea debe generarse siguiendo las instrucciones dispuestas en `001_task_planning_template.md`.
    *   **CRÍTICO:** Los documentos de tarea deben comenzar directamente con "1. Resumen de la Tarea" - nunca incluyas encabezados de plantilla, descripciones o contenido promocional del archivo de plantilla.
    *   **CONVENCIÓN DE NOMENCLATURA DE TAREAS:** Los archivos de tarea deben seguir el formato `<numero_tarea>_<nombre_de_la_tarea>.md` (ej., `001_fastapi_backend_implementation.md`, `002_user_authentication.md`). Usa números de 3 dígitos con ceros a la izquierda para un orden adecuado.

4.  **Contexto y Referencias:**
    *   Si requieres contexto adicional, documentación, ejemplos de código o pautas arquitectónicas para el proyecto, consulta los archivos ubicados en el directorio de referencias del proyecto (ej., `references/`, `@ai_docs/references/`, o similar).
    *   Para documentación de librerías externas, si tienes acceso a MCPs (Protocolo de Contexto de Modelo), prioriza usar el servidor MCP `context7` para obtener información precisa y actualizada.

## 2. Ciclo de Vida de Desarrollo

1.  **Configuración y Verificación del Proyecto:**
    *   **ENTORNO VIRTUAL:** Siempre activa el entorno virtual del proyecto antes de comenzar cualquier trabajo (ej., `ai-env`, `source venv/bin/activate`, `conda activate`, etc.).
    *   Antes de comenzar el trabajo, asegúrate de que las dependencias del proyecto estén instaladas usando el gestor de paquetes apropiado (ej., `poetry install`, `npm install`, `pip install -r requirements.txt`, etc.).
    *   Después de la instalación, ejecuta el conjunto de pruebas para confirmar que el proyecto está en un estado estable (ej., `poetry run pytest`, `npm test`, `python -m pytest`, etc.).
    *   **VERSIÓN DE LENGUAJE:** Usa la versión de lenguaje apropiada según lo especificado en la configuración del proyecto.
    *   **DEPENDENCIAS:** Usa las últimas versiones compatibles de dependencias requeridas para integraciones.

2.  **Calidad de Código y Linting:**
    *   Después de hacer cualquier cambio de código, **debes** ejecutar el formateador de código apropiado para el proyecto (ej., `poetry run black .`, `npm run format`, `prettier --write .`, etc.). Esto asegura que todo el código cumpla con el estilo del proyecto.

3.  **Gestión de Dependencias:**
    *   **RESTRICCIONES DE VERSIÓN:** Siempre usa restricciones de versión mínima (>=) en lugar de versiones exactas (==) en archivos de dependencia para evitar conflictos de dependencias.
    *   **COMPATIBILIDAD:** Asegura que todas las dependencias sean compatibles entre sí y con los requisitos del proyecto.
    *   **RESOLUCIÓN DE CONFLICTOS:** Verifica conflictos de dependencias entre paquetes antes de finalizar requisitos y prueba la instalación en un entorno limpio.

4.  **Estándares de Implementación:**
    *   **IMPLEMENTACIONES GENÉRICAS:** Siempre implementa soluciones genéricas a menos que se te diga explícitamente que uses herramientas/servicios específicos.
    *   **SIN SUPOSICIONES:** No asumas servicios específicos (Supabase, Auth0, etc.) a menos que sean mencionados explícitamente por el usuario.
    *   **DISEÑO FLEXIBLE:** Diseña para flexibilidad y portabilidad a través de diferentes proveedores.
    *   **REQUISITOS EXPLÍCITOS:** Solo usa herramientas específicas cuando sean solicitadas explícitamente por el usuario.

5.  **Pautas de Commit de Git:**
    *   Al prepararte para hacer commit de cambios, **debes** usar la plantilla `004_git_commit_workflow.md` como tu guía.

6.  **Seguridad y Gestión de Secretos:**
    *   **NUNCA** registres (log), comitees o expongas secretos, claves API o cualquier otra credencial sensible en el código.
    *   Usa variables de entorno o un sistema de gestión de secretos seguro para todas las credenciales.
    *   Si encuentras secretos hardcodeados, márcalos al usuario inmediatamente.

7.  **Protocolo de Manejo de Errores:**
    *   Si cualquier comando falla (ej., pruebas fallan, una construcción se rompe), detén inmediatamente la tarea actual.
    *   Reporta el comando que fue ejecutado, su salida completa (stdout y stderr) y el error. No intentes arreglar el problema sin instrucciones explícitas del usuario.

## 3. Directivas Críticas

*   **CONFIRMACIÓN REQUERIDA:** Tienes **prohibido** aplicar cualquier cambio de código, modificar archivos o ejecutar el plan descrito en un documento de tarea hasta que recibas confirmación explícita del usuario para proceder. Tu rol es preparar el plan para aprobación.

*   **RETROALIMENTACIÓN Y REFINAMIENTO DE PLANTILLA:** Si el usuario proporciona retroalimentación indicando que una definición de tarea generada es incorrecta o incompleta, eres responsable de refinar la plantilla original (archivo `.md` en el directorio de plantillas) que se utilizó. Incorpora la retroalimentación del usuario para mejorar la plantilla y prevenir el mismo error en el futuro.