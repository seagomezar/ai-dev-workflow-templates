# Contribuyendo a Plantillas de Flujo de Trabajo de Desarrollo con IA

¡Gracias por tu interés en contribuir al proyecto de Plantillas de Flujo de Trabajo de Desarrollo con IA! Este documento proporciona pautas para contribuir con nuevas plantillas de flujo de trabajo y mejorar las existentes.

## Visión del Proyecto

El proyecto de Plantillas de Flujo de Trabajo de Desarrollo con IA tiene como objetivo crear una colección completa de plantillas estandarizadas y reutilizables que permitan a los agentes de IA asistir a los desarrolladores de manera más efectiva. Nuestro objetivo es:

- **Estandarizar flujos de trabajo asistidos por IA** a través de diferentes escenarios de desarrollo
- **Mejorar la efectividad de los agentes de IA** mediante instrucciones claras y estructuradas
- **Reducir el tiempo de configuración** para tareas comunes de desarrollo
- **Promover mejores prácticas** en el desarrollo asistido por IA
- **Construir una comunidad** de colaboradores que compartan conocimientos y flujos de trabajo

## Tabla de Contenidos

- [Visión del Proyecto](#visión-del-proyecto)
- [Comenzando](#comenzando)
- [Estructura de la Plantilla](#estructura-de-la-plantilla)
- [Creando Nuevas Plantillas](#creando-nuevas-plantillas)
- [Convención de Nomenclatura de Plantillas](#convención-de-nomenclatura-de-plantillas)
- [Estándares de Calidad](#estándares-de-calidad)
- [Proceso de Envío](#proceso-de-envío)
- [Proceso de Revisión](#proceso-de-revisión)
- [Categorías de Plantillas](#categorías-de-plantillas)
- [Ejemplos y Referencias](#ejemplos-y-referencias)
- [Mantenimiento de Plantillas](#mantenimiento-de-plantillas)
- [Obteniendo Ayuda](#obteniendo-ayuda)
- [Reconocimiento](#reconocimiento)
- [Licencia](#licencia)

## Comenzando

### Prerrequisitos

- Entendimiento básico de formato markdown
- Familiaridad con flujos de trabajo de desarrollo asistidos por IA
- Entendimiento del propósito del proyecto y plantillas existentes

### Configurando Tu Entorno

1. Haz un fork del repositorio
2. Clona tu fork localmente
3. Crea una nueva rama para tu contribución
4. Revisa las plantillas existentes para entender la estructura y el estilo

### Flujo de Trabajo de Desarrollo

1. **Crea una rama de característica** desde `main`
2. **Haz tus cambios** siguiendo las pautas en este documento
3. **Prueba tu plantilla** con un escenario real
4. **Envía un pull request** con una descripción clara
5. **Responde a la retroalimentación** y haz las revisiones necesarias

## Estructura de la Plantilla

Todas las plantillas deben seguir una estructura consistente para asegurar que se integren perfectamente con el sistema de flujo de trabajo del agente de IA. Aquí está el formato requerido:

### Secciones Requeridas

1. **Encabezado con Información de la Plantilla**
   - Título de la plantilla
   - Breve descripción del propósito de la plantilla
   - Sección "Sobre Esta Plantilla" explicando el uso

2. **Secciones de Contenido Central**
   - Secciones numeradas (1, 2, 3, etc.)
   - Subsecciones claras y accionables
   - Marcadores TODO para personalización
   - Casillas de verificación para seguimiento de progreso

3. **Instrucciones para el Agente de IA**
   - Pasos del proceso obligatorio
   - Preferencias de comunicación
   - Estándares de calidad
   - Pautas de implementación

### Ejemplo de Formato de Plantilla

```markdown
# [Nombre de la Plantilla]

> **Sobre Esta Plantilla:** [Breve descripción de lo que hace esta plantilla y cuándo usarla]

---

## 1. [Primera Sección]

### [Título de Subsección]
[Contenido con marcadores TODO para personalización]

---

## 2. [Segunda Sección]
[Más contenido...]

---

## [N]. Instrucciones para el Agente de IA

### [Nombre del Proceso]
🎯 **PROCESO OBLIGATORIO:**
1. [Paso 1]
2. [Paso 2]
...

---

```

## Creando Nuevas Plantillas

### Paso 1: Elige Tu Tipo de Plantilla

Considera qué flujo de trabajo o proceso se beneficiaría de la asistencia de IA. Las categorías comunes incluyen:

- **Flujos de Trabajo de Desarrollo** (planificación de tareas, correcciones de errores, revisiones de código)
- **DevOps y Despliegue** (CI/CD, infraestructura, monitoreo)
- **Documentación** (docs de API, guías de usuario, escritura técnica)
- **Pruebas** (planificación de pruebas, automatización de pruebas, aseguramiento de calidad)
- **Gestión de Proyectos** (planificación de sprints, retrospectivas, recopilación de requisitos)
- **Seguridad** (auditorías de seguridad, evaluaciones de vulnerabilidad, cumplimiento)

### Paso 2: Planifica la Estructura de Tu Plantilla

Antes de escribir, esquema:
- ¿Qué problema resuelve esta plantilla?
- ¿Cuáles son los pasos clave en el proceso?
- ¿Qué información necesita un agente de IA para ejecutar este flujo de trabajo?
- ¿Cuáles son los estándares de calidad y mejores prácticas?

### Paso 3: Escribe la Plantilla

Sigue estas pautas:

1. **Usa encabezados claros y descriptivos**
2. **Incluye marcadores TODO** para personalización
3. **Proporciona instrucciones específicas** para agentes de IA
4. **Incluye listas de verificación** para seguimiento de progreso
5. **Agrega ejemplos** donde sea útil
6. **Mantenlo completo** pero no abrumador

### Paso 4: Agrega Instrucciones para el Agente de IA

Cada plantilla debe incluir una sección con instrucciones específicas para agentes de IA, incluyendo:
- Pasos del proceso obligatorio
- Preferencias de comunicación
- Estándares de calidad
- Procedimientos de manejo de errores

### Paso 5: Prueba Tu Plantilla

Antes de enviar, prueba minuciosamente tu plantilla:

1. **Úsala tú mismo**: Sigue la plantilla con un escenario de proyecto real
2. **Prueba con agentes de IA**: Si es posible, prueba con herramientas de IA reales
3. **Verifica completitud**: Asegura que todas las secciones estén llenadas adecuadamente
4. **Verifica formato**: Revisa el renderizado de markdown y la estructura
5. **Valida instrucciones**: Confirma que las instrucciones del agente de IA sean claras y accionables

## Convención de Nomenclatura de Plantillas

Las plantillas deben seguir este patrón de nomenclatura:

```
[numero]_[nombre_descriptivo]_template.md
```

Ejemplos:
- `005_deployment_workflow_template.md`
- `006_security_audit_template.md`
- `007_documentation_generation_template.md`
- `008_performance_optimization_template.md`

### Pautas de Numeración

- Usa números de 3 dígitos con ceros a la izquierda (001, 002, 003, etc.)
- Los números deben asignarse secuencialmente
- Revisa las plantillas existentes para determinar el siguiente número disponible
- Si no estás seguro sobre la numeración, envía tu plantilla y asignaremos el número apropiado

## Estándares de Calidad

### Calidad de Contenido

- **Claridad**: Usa lenguaje claro y conciso
- **Completitud**: Cubre todos los pasos y consideraciones necesarias
- **Precisión**: Asegura precisión técnica y mejores prácticas
- **Consistencia**: Sigue el formato y estilo establecidos
- **Accionabilidad**: Proporciona instrucciones específicas y accionables

### Estándares de Formato

- Usa formato markdown consistentemente
- Incluye jerarquía de encabezados adecuada
- Usa viñetas y listas numeradas apropiadamente
- Incluye marcadores TODO para personalización
- Agrega casillas de verificación para seguimiento de progreso

### Estándares Técnicos

- Las plantillas deben ser agnósticas a la tecnología cuando sea posible
- Incluye flexibilidad para diferentes tipos de proyectos
- Proporciona guía clara para agentes de IA
- Incluye manejo de errores y consideraciones de casos borde

## Proceso de Envío

### Antes de Enviar

1. **Revisa tu plantilla** contra los estándares de calidad
2. **Prueba la plantilla** usándola en un escenario real
3. **Verifica errores tipográficos** y problemas de formato
4. **Asegura consistencia** con plantillas existentes

### Cómo Enviar

1. **Crea un Pull Request** con tu nueva plantilla
2. **Incluye una descripción** de lo que hace la plantilla y por qué es útil
3. **Referencia cualquier issue relacionado** o discusiones
4. **Agrégate** a la lista de colaboradores (si lo deseas)

### Plantilla de Pull Request

Al crear un pull request, incluye:

```markdown
## Template: [Nombre de la Plantilla]

### Description
[Breve descripción de lo que hace esta plantilla]

### Use Cases
- [Caso de uso 1]
- [Caso de uso 2]
- [Caso de uso 3]

### Key Features
- [Característica 1]
- [Característica 2]
- [Característica 3]

### Testing
- [ ] Plantilla probada con escenario real
- [ ] Instrucciones de agente de IA verificadas
- [ ] Formato verificado
- [ ] Contenido revisado por precisión

### Additional Notes
[Cualquier información o consideración adicional]
```

## Proceso de Revisión

### Lo Que Buscamos

1. **Adherencia a la Estructura**: Sigue el formato de plantilla establecido
2. **Calidad de Contenido**: Clara, precisa y completa
3. **Compatibilidad con Agente de IA**: Las instrucciones son claras para agentes de IA
4. **Valor Práctico**: Resuelve problemas reales en el desarrollo asistido por IA
5. **Consistencia**: Coincide con el estilo y tono de las plantillas existentes

### Cronograma de Revisión

- Revisión inicial: Dentro de 3-5 días hábiles
- Retroalimentación proporcionada: Dentro de 1 semana
- Aprobación final: Dentro de 2 semanas (dependiendo de las revisiones necesarias)

### Áreas Comunes de Retroalimentación

- Instrucciones de agente de IA faltantes
- Formato inconsistente
- Secciones poco claras o incompletas
- Marcadores TODO faltantes
- Falta de ejemplos prácticos

### Errores Comunes a Evitar

- **Saltar Instrucciones de Agente de IA**: Cada plantilla debe incluir instrucciones específicas para agentes de IA
- **Numeración Inconsistente**: Usa jerarquía de encabezados adecuada (1, 2, 3, no 1, 1.1, 1.2)
- **Marcadores TODO Faltantes**: Incluye puntos de personalización para diferentes proyectos
- **Ejemplos Demasiado Específicos**: Mantén los ejemplos genéricos y adaptables
- **Listas de Verificación Incompletas**: Asegura que todos los pasos de verificación necesarios estén incluidos
- **Mala Organización de Secciones**: Sigue la estructura y flujo establecidos
- **Manejo de Errores Faltante**: Incluye guía para casos borde y escenarios de error

## Categorías de Plantillas

### Categorías Actuales

1. **Planificación de Tareas** (001_task_planning_template.md)
2. **Corrección de Errores** (002_bug_fix_template.md)
3. **Revisiones de Código** (003_code_review_template.md)
4. **Flujo de Trabajo de Git** (004_git_commit_workflow.md)

### Nuevas Categorías Sugeridas

- **Despliegue y DevOps**
- **Seguridad y Cumplimiento**
- **Pruebas y Aseguramiento de Calidad**
- **Documentación y Escritura Técnica**
- **Optimización de Rendimiento**
- **Gestión de Base de Datos**
- **Desarrollo de API**
- **Desarrollo Frontend**
- **Desarrollo Backend**
- **Desarrollo Móvil**
- **Ciencia de Datos y ML**
- **Gestión de Proyectos**
- **Investigación de Usuario y UX**

## Ejemplos y Referencias

### Estudia Plantillas Existentes

Antes de crear tu plantilla, estudia estos ejemplos:

- **001_task_planning_template.md**: Planificación de proyectos completa
- **002_bug_fix_template.md**: Resolución de errores sistemática
- **003_code_review_template.md**: Evaluación de código exhaustiva
- **004_git_commit_workflow.md**: Estandarización de flujo de trabajo Git

### Mejores Prácticas de Plantillas Existentes

1. **Estructura Clara**: Usa secciones numeradas con encabezados descriptivos
2. **Marcadores TODO**: Incluye puntos de personalización para diferentes proyectos
3. **Instrucciones para Agente de IA**: Proporciona guía específica y accionable
4. **Seguimiento de Progreso**: Incluye listas de verificación y pasos de verificación
5. **Estándares de Calidad**: Define expectativas claras y mejores prácticas

## Mantenimiento de Plantillas

### Actualizando Plantillas Existentes

Si encuentras problemas con plantillas existentes o quieres mejorarlas:

1. **Abre un Issue** describiendo el problema o mejora
2. **Crea un Pull Request** con tus cambios propuestos
3. **Sigue los mismos estándares de calidad** que las nuevas plantillas
4. **Prueba tus cambios** minuciosamente antes de enviar

### Proceso de Desaprobación (Deprecation)

Las plantillas pueden ser desaprobadas si:
- Se vuelven obsoletas debido a cambios tecnológicos
- Son reemplazadas por mejores alternativas
- Ya no sirven a su propósito previsto

Las plantillas desaprobadas serán:
- Marcadas claramente en la documentación
- Movidas a una carpeta de desaprobadas
- Reemplazadas con versiones actualizadas cuando sea posible

## Obteniendo Ayuda

### ¿Preguntas o Problemas?

- **Abre un Issue**: Para preguntas sobre el proyecto o creación de plantillas
- **Inicia una Discusión**: Para conversaciones más amplias sobre mejoras de flujo de trabajo
- **Revisa Issues Existentes**: Verifica si tu pregunta ha sido respondida antes

### Pautas de la Comunidad

- Sé respetuoso y constructivo
- Proporciona retroalimentación útil
- Comparte conocimientos y mejores prácticas
- Ayuda a otros a aprender y mejorar

## Reconocimiento

Los colaboradores serán reconocidos en:

- El README.md del proyecto
- Encabezados de plantillas individuales (si se desea)
- Notas de lanzamiento para contribuciones significativas
- La lista de colaboradores del proyecto

## Licencia

Al contribuir a este proyecto, aceptas que tus contribuciones serán licenciadas bajo la misma licencia que el proyecto (ver archivo LICENSE para detalles).