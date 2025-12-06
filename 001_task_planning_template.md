# Plantilla de Planificación de Tareas con IA

> **Sobre Esta Plantilla:** Este es un marco sistemático para planificar y ejecutar proyectos técnicos con asistencia de IA. Utiliza esta estructura para dividir funciones complejas, mejoras o correcciones en tareas manejables y rastreables que los agentes de IA puedan ejecutar de manera efectiva.

---

## 1. Resumen de la Tarea

### Título de la Tarea
<!-- Dale a tu tarea un nombre claro y específico que describa lo que estás construyendo o arreglando -->
**Título:** [Título breve y descriptivo - ej., "Agregar Sistema de Autenticación de Usuarios" o "Arreglar Error de Integración de Pagos"]

### Declaración del Objetivo
<!-- Escribe un párrafo explicando qué quieres lograr y por qué es importante para tu proyecto -->
**Objetivo:** [Declaración clara del resultado final que deseas y el valor para el negocio/usuario que proporciona]

### Nombre de la Rama
<!-- Especifica el nombre de la rama creada para esta tarea -->
**Rama:** [ej., `feat/T-123-add-user-auth` o `fix/T-456-bug-fix`]


---

## 2. Análisis del Proyecto y Estado Actual

### Tecnología y Arquitectura
<!-- Aquí es donde documentas tu stack tecnológico actual para que la IA entienda tu entorno -->
- **Frameworks y Versiones:** TODO: Enumera tus frameworks principales y versiones (usa >= para versiones mínimas para evitar conflictos)
- **Lenguaje:** TODO: Especifica tu lenguaje de programación y versión
- **Base de Datos y ORM:** TODO: Define tu elección de base de datos y ORM (si aplica)
- **UI y Estilos:** TODO: Enumera tu framework de UI y enfoque de estilos (si aplica)
- **Autenticación:** TODO: Especifica tu sistema de autenticación (si aplica)
- **Patrones Arquitectónicos Clave:** TODO: Enumera tus patrones arquitectónicos principales
- **Gestión de Dependencias:** TODO: Usa restricciones de versión mínima (>=) en lugar de versiones exactas (==) para evitar conflictos

### Estado Actual
<!-- Describe lo que existe hoy - qué funciona, qué está roto, qué falta -->
[Análisis del estado actual de tu código base, funcionalidad existente y lo que necesita cambiarse]

## 3. Contexto y Definición del Problema

### Planteamiento del Problema
<!-- Aquí es donde defines claramente el problema específico que estás resolviendo -->
[Explicación detallada del problema, incluyendo impacto en el usuario, puntos de dolor y por qué necesita resolverse ahora]

### Criterios de Éxito
<!-- Define exactamente cómo sabrás cuando esta tarea esté completa y sea exitosa -->
- [ ] [Resultado específico y medible 1]
- [ ] [Resultado específico y medible 2]
- [ ] [Resultado específico y medible 3]

### Entregables
- Un nuevo documento de tarea creado en el directorio `tasks/` del proyecto (ej., `tasks/001_add_user_auth.md`)
- El documento de tarea contendrá el plan completo para la nueva función, incluyendo requisitos técnicos, plan de implementación e instrucciones para el agente de IA.

---

## 4. Contexto del Modo de Desarrollo

### Contexto del Modo de Desarrollo
<!-- Aquí es donde le cuentas al agente de IA sobre las restricciones y prioridades de tu proyecto -->
- **🚨 Etapa del Proyecto:** TODO: Define si esto es nuevo desarrollo, sistema en producción o migración de legado
- **Cambios Rompedores (Breaking Changes):** TODO: Especifica si los cambios rompedores son aceptables o deben evitarse
- **Manejo de Datos:** TODO: Define los requisitos de preservación de datos
- **Base de Usuarios:** TODO: Describe quién se verá afectado por los cambios
- **Prioridad:** TODO: Establece tus prioridades de velocidad vs estabilidad

---

## 5. Requisitos Técnicos

### Requisitos Funcionales
<!-- Aquí es donde la IA entenderá exactamente qué debe hacer el sistema - sé específico sobre acciones del usuario y comportamientos del sistema -->

TODO: Define qué pueden hacer los usuarios y qué manejará automáticamente el sistema
- Formato de ejemplo: "El usuario puede [acción específica]"
- Formato de ejemplo: "El sistema automáticamente [comportamiento específico]" 
- Formato de ejemplo: "Cuando ocurre [condición], entonces [respuesta del sistema]"

### Requisitos No Funcionales
<!-- Aquí es donde defines estándares de rendimiento, seguridad y usabilidad -->
- **Rendimiento:** TODO: Define tiempo de respuesta y requisitos de manejo de carga
- **Seguridad:** TODO: Especifica necesidades de autenticación y protección de datos
- **Usabilidad:** TODO: Establece estándares de experiencia de usuario y accesibilidad
- **Diseño Responsivo:** TODO: Define requisitos de soporte para móvil, tablet y escritorio
- **Soporte de Temas:** TODO: Especifica requisitos de modo claro/oscuro y marca

### Restricciones Técnicas
<!-- Aquí es donde listas las limitaciones dentro de las cuales debe trabajar el agente de IA -->
- [Debe usar el sistema existente X]
- [No puede modificar la tabla de base de datos Y]
- [Debe mantener compatibilidad con la función Z]

---

## 6. Cambios en Datos y Base de Datos

### Cambios en el Esquema de Base de Datos
<!-- Aquí es donde especificas cualquier modificación de base de datos necesaria (si aplica) -->

TODO: Agrega tus cambios de esquema de base de datos aquí (nuevas tablas, columnas, índices, etc.)

### Actualizaciones del Modelo de Datos
<!-- Aquí es donde defines tipos de datos, actualizaciones de esquema o cambios en la estructura de datos -->

TODO: Define tus tipos de datos, interfaces y cambios en la estructura de datos

### Plan de Migración de Datos
<!-- Aquí es donde planificas cómo manejar los datos existentes durante los cambios (si aplica) -->

TODO: Planifica tus pasos de migración de datos (respaldo, aplicar cambios, transformar datos, validar)

---

## 7. Cambios en API y Backend

### Reglas de Patrones de Acceso a Datos
<!-- Aquí es donde le dices al agente de IA cómo estructurar el código backend en tu proyecto (si aplica) -->

TODO: Define dónde deben ir los diferentes tipos de código en tu proyecto (mutaciones, consultas, rutas de API)

### Acciones del Servidor
<!-- Lista las operaciones de mutación backend que necesitas (si aplica) -->

TODO: Lista tus operaciones de crear, actualizar, eliminar y qué hacen

### Consultas a Base de Datos
<!-- Especifica cómo obtendrás datos (si aplica) -->

TODO: Define tu enfoque de obtención de datos (consultas directas vs funciones separadas)

---

## 8. Cambios en Frontend

### Nuevos Componentes
<!-- Aquí es donde especificas los componentes de UI a crear (si aplica) -->

TODO: Lista los nuevos componentes que necesitas crear y su propósito

### Actualizaciones de Página
<!-- Aquí es donde listas las páginas que necesitan modificaciones (si aplica) -->

TODO: Lista las páginas que necesitan cambios y qué modificaciones se requieren

### Gestión de Estado
<!-- Aquí es donde planificas cómo fluyen los datos a través de tu frontend (si aplica) -->

TODO: Define tu enfoque de gestión de estado y estrategia de flujo de datos

---

## 9. Plan de Implementación

TODO: Divide tu trabajo en fases con tareas específicas y rutas de archivo

---

## 10. Seguimiento de Finalización de Tareas

### Seguimiento de Progreso en Tiempo Real
<!-- Aquí es donde le dices a la IA que actualice el progreso a medida que se completa el trabajo -->

TODO: Define cómo quieres que la IA rastree e informe el progreso en las tareas

---

## 11. Estructura de Archivos y Organización

TODO: Planifica qué nuevos archivos crear y qué archivos existentes modificar

---

## 12. Instrucciones para el Agente de IA

### Flujo de Trabajo de Implementación
<!-- Aquí es donde das instrucciones específicas a tu agente de IA -->
🎯 **PROCESO OBLIGATORIO:**
1.  **Entorno Virtual:** Siempre activa el entorno virtual del proyecto antes de comenzar cualquier trabajo (ej., `ai-env`, `source venv/bin/activate`, `conda activate`, etc.).
2.  **Ramas:** Antes de comenzar la implementación, asegúrate de estar en la rama `main` y que esté actualizada. Crea una nueva rama para la tarea con un nombre descriptivo (ej., `feat/T-123-add-user-auth`).
TODO:

### Preferencias de Comunicación
<!-- Aquí es donde estableces expectativas sobre cómo debe comunicarse la IA -->
TODO: Cómo quieres que el agente se comunique contigo

### Estándares de Calidad de Código
<!-- Aquí es donde defines tus estándares de codificación para que la IA los siga -->
- **Estilo de Código:** Sigue las convenciones de codificación y pautas de estilo establecidas del proyecto
- **Patrones de Arquitectura:** Usa patrones arquitectónicos establecidos de las implementaciones de referencia del proyecto
- **Manejo de Errores:** Implementa patrones adecuados de manejo de errores y registro (logging)
- **Pruebas:** Sigue las convenciones de pruebas del proyecto y asegura una cobertura de pruebas adecuada
- **Documentación:** Mantén documentación clara y actualizada para todo el código nuevo

### Estándares de Gestión de Dependencias
<!-- Aquí es donde defines las mejores prácticas de gestión de dependencias -->
- **Restricciones de Versión:** Usa restricciones de versión mínima (>=) en lugar de versiones exactas (==) para evitar conflictos
- **Resolución de Conflictos:** Verifica conflictos de dependencias entre paquetes antes de finalizar los requisitos
- **Compatibilidad:** Asegura que todas las dependencias sean compatibles entre sí y con los requisitos del proyecto
- **Pruebas de Dependencias:** Siempre prueba la instalación de dependencias en un entorno limpio

### Estándares de Implementación
<!-- Aquí es donde defines las mejores prácticas de implementación -->
- **Implementaciones Genéricas:** Siempre implementa soluciones genéricas a menos que se te indique explícitamente usar herramientas/servicios específicos
- **Sin Suposiciones:** No asumas servicios específicos a menos que se mencionen explícitamente
- **Diseño Flexible:** Diseña para flexibilidad y portabilidad a través de diferentes proveedores
- **Requisitos Explícitos:** Solo usa herramientas específicas cuando el usuario lo solicite explícitamente
- **Implementación de Referencia:** Para cualquier tarea especializada, referencia y sigue patrones de las implementaciones de referencia del proyecto

---

## 13. Análisis de Impacto de Segundo Orden

### Evaluación de Impacto
<!-- Aquí es donde piensas en las consecuencias más amplias de tus cambios -->

TODO: Dile a la IA qué secciones de código te preocupa romper, preocupaciones de rendimiento e impactos en el flujo de trabajo del usuario