# Plantilla de Corrección de Errores con IA

> **Sobre Esta Plantilla:** Esta plantilla proporciona un enfoque estructurado para identificar, analizar y resolver errores (bugs) con la asistencia de un agente de IA. Seguir este proceso asegura que los errores se arreglen sistemáticamente y reduce el riesgo de introducir nuevos problemas.

---

## 1. Identificación del Error

### Título del Error
**Título:** [Título breve y descriptivo del error - ej., "Cierre de Sesión de Usuario Falla en Safari" o "Cálculo Incorrecto en Módulo de Reportes"]

### Clasificación del Error
- **Gravedad:** [Crítica, Alta, Media, Baja]
- **Tipo:** [Funcional, Rendimiento, UI/UX, Datos]

### Descripción del Error
**Descripción:** [Descripción detallada del error, incluyendo qué está sucediendo, qué debería estar sucediendo y el impacto en el usuario o sistema.]

### Pasos para Reproducir
**Pasos:**
1. [Primer paso para reproducir el error]
2. [Segundo paso para reproducir el error]
3. [Tercer paso para reproducir el error]
...

### Entorno
- **Sistema Operativo:** [ej., Windows, macOS, Linux]
- **Navegador (si aplica):** [ej., Chrome, Firefox, Safari, Edge]
- **Versión de App/Commit:** [La versión o hash del commit donde se observó el error]
- **Dependencias:** [Versión de Python/Node si es relevante]

---

## 2. Análisis y Diagnóstico

### Análisis Inicial
[Pensamientos iniciales sobre la causa potencial del error. Aquí es donde la IA puede comenzar su investigación.]

### Archivos Relevantes
[Lista de archivos que podrían estar relacionados con el error. La IA puede usar esto como punto de partida para su análisis de código.]

### Mensajes de Error
[Cualquier mensaje de error de logs, consola o reportes de usuario que sean relevantes para el error.]

---

## 3. Solución Propuesta

### Causa Raíz
[Una explicación clara de la causa raíz del error, basada en el análisis.]

### Cambios Propuestos
[Una descripción detallada de los cambios de código requeridos para arreglar el error. Esto debe incluir nombres de archivos y modificaciones de código específicas.]

### Entregables
- Un commit de Git con la corrección del error, siguiendo las convenciones de commit del proyecto.
- El mensaje del commit debe describir claramente el error y la solución.

---

## 4. Implementación y Verificación

### Pasos de Implementación
1. **Cambios de Código:** Aplica los cambios de código propuestos en la rama actual.
2. **Pruebas (Bajo Demanda):**
    - No ejecutes ninguna prueba ni inicies servidores/aplicaciones por defecto. Asume que ya están corriendo.
    - Si el usuario lo solicita, realiza pruebas específicas.
    - **Pruebas Unitarias:** Si se solicita, agrega o actualiza pruebas unitarias para cubrir la corrección del error.
    - **Pruebas de Integración:** Si se solicita, ejecuta pruebas de integración para asegurar que la corrección no rompa otras partes del sistema.
    - **Pruebas Manuales:** Si se solicita, verifica manualmente que el error esté resuelto siguiendo los pasos de reproducción. Asume que el servidor y/o app están funcionando.

### Verificación
- [ ] El error ya no es reproducible (si se probó).
- [ ] Todas las pruebas relevantes pasan (si se probaron).
- [ ] La corrección no introduce nuevos errores (pruebas de regresión, si se realizaron).

### Lista de Verificación Rápida
- [ ] Error reproducido localmente
- [ ] Causa raíz identificada
- [ ] Solución implementada
- [ ] Código formateado con el formateador apropiado
- [ ] Solución probada (si el usuario lo solicitó)
- [ ] No se introdujeron regresiones (si se probaron)

---

## 5. Instrucciones para el Agente de IA

### Flujo de Trabajo de Implementación
🎯 **PROCESO OBLIGATORIO:**
1.  **Recopilación de Información:** Antes de comenzar, asegúrate de que el usuario haya proporcionado toda la información necesaria en la sección "Identificación del Error". Si falta información, pídesela al usuario.
2.  **Entorno Virtual:** Siempre activa el entorno virtual del proyecto antes de comenzar cualquier trabajo (ej., `ai-env`, `source venv/bin/activate`, `conda activate`, etc.).
3.  **Análisis:** Analiza la descripción del error proporcionada, los pasos para reproducir y los archivos relevantes para entender el problema. Confía en la evaluación del usuario sobre lo que ya funciona y enfoca la investigación en el problema descrito, a menos que sean necesarias comprobaciones adicionales para entender el contexto completo. Usa todos los recursos del proyecto disponibles, incluyendo ejemplos en la carpeta de referencias del proyecto. Para problemas potenciales de versión de librerías, consulta el servidor mcp `context7` si está disponible. Revisa errores similares en commits recientes.
4.  **Proponer Solución:** Propón una solución basada en el análisis.
5.  **Confirmación:** Presenta la solución propuesta al usuario y obtén su confirmación antes de proceder.
6.  **Implementar Solución:** Implementa la solución según los cambios propuestos en la rama actual.
7.  **Verificar Solución (Bajo Demanda):** No ejecutes pruebas ni realices verificaciones a menos que el usuario lo instruya explícitamente. Si se te pide probar, asume que cualquier servidor o aplicación requerida ya está corriendo.
8.  **Formato de Código:** Ejecuta el formateador de código apropiado para el proyecto (ej., `poetry run black .`, `npm run format`, `prettier --write .`, etc.).

### Preferencias de Comunicación
- Proporciona actualizaciones regulares sobre el progreso de la corrección del error.
- Comunica claramente la causa raíz y la solución propuesta antes de implementar la corrección.
- Reporta cualquier problema o bloqueo encontrado durante el proceso.
