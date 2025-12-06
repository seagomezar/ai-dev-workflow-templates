# Plantilla de Revisión de Código con IA

> **Sobre Esta Plantilla:** Esta plantilla proporciona un enfoque estructurado para realizar revisiones de código exhaustivas con asistencia de IA. Seguir este proceso asegura que los cambios de código sean evaluados adecuadamente por calidad, seguridad, rendimiento y mantenibilidad.

---

## 1. Resumen de la Revisión

### Título de la Revisión
**Título:** [Título breve y descriptivo de la revisión de código - ej., "Revisar Implementación de Autenticación de Usuario" o "Revisar Cambios de Migración de Base de Datos"]

### Tipo de Revisión
- **Tipo:** [Revisión de Característica, Revisión de Corrección de Error, Revisión de Refactorización, Revisión de Seguridad, Revisión de Rendimiento]
- **Prioridad:** [Alta, Media, Baja]
- **Revisor:** [Nombre del revisor o agente de IA realizando la revisión]

### Información del Pull Request
- **Número de PR:** [#123]
- **Rama:** [ej., `feat/user-auth` o `fix/payment-bug`]
- **Autor:** [Nombre del autor del código]
- **Archivos Cambiados:** [Número de archivos modificados]

---

## 2. Análisis de Código

### Evaluación de Calidad de Código
- **Legibilidad:** [Excelente, Buena, Regular, Mala] - [Breve explicación]
- **Mantenibilidad:** [Excelente, Buena, Regular, Mala] - [Breve explicación]
- **Rendimiento:** [Excelente, Buena, Regular, Mala] - [Breve explicación]
- **Seguridad:** [Excelente, Buena, Regular, Mala] - [Breve explicación]

### Estilo y Estándares de Código
- [ ] El código sigue las pautas de estilo del proyecto
- [ ] Se usan convenciones de nomenclatura consistentes
- [ ] Indentación y formato adecuados
- [ ] No queda código comentado
- [ ] Uso apropiado de comentarios y documentación

### Arquitectura y Diseño
- [ ] El código sigue patrones arquitectónicos establecidos
- [ ] Separación adecuada de preocupaciones
- [ ] Uso apropiado de patrones de diseño
- [ ] Sin acoplamiento innecesario entre componentes
- [ ] Sigue principios SOLID (si aplica)

---

## 3. Revisión Funcional

### Cumplimiento de Requisitos
- [ ] El código cumple con los requisitos establecidos
- [ ] Todas las historias de usuario/criterios de aceptación están abordados
- [ ] Los casos borde se manejan adecuadamente
- [ ] Las condiciones de error se gestionan apropiadamente

### Cobertura de Pruebas
- [ ] Las pruebas unitarias están presentes y son completas
- [ ] Las pruebas de integración cubren los cambios
- [ ] Los casos borde están probados
- [ ] Los escenarios de error están probados
- [ ] La cobertura de pruebas cumple con los estándares del proyecto

### Documentación
- [ ] El código es autodocumentado
- [ ] La lógica compleja se explica con comentarios
- [ ] La documentación de la API está actualizada (si aplica)
- [ ] El README o documentación de usuario está actualizado (si aplica)

---

## 4. Revisión de Seguridad

### Consideraciones de Seguridad
- [ ] Sin secretos o credenciales hardcodeadas
- [ ] La validación de entrada está implementada
- [ ] La codificación de salida se usa donde es apropiado
- [ ] Prevención de inyección SQL (si aplica)
- [ ] Prevención de XSS (si aplica)
- [ ] Protección CSRF (si aplica)
- [ ] La autenticación y autorización están implementadas correctamente
- [ ] Los datos sensibles se manejan de forma segura

### Manejo de Datos
- [ ] Los datos personales se manejan de acuerdo con los requisitos de privacidad
- [ ] La validación de datos es completa
- [ ] Los mensajes de error no filtran información sensible
- [ ] El registro (logging) no expone datos sensibles

---

## 5. Revisión de Rendimiento

### Consideraciones de Rendimiento
- [ ] Sin cuellos de botella de rendimiento obvios
- [ ] Las consultas a base de datos están optimizadas (si aplica)
- [ ] El caché se usa apropiadamente
- [ ] El uso de memoria es razonable
- [ ] Sin llamadas a API u operaciones innecesarias
- [ ] Las operaciones asíncronas se usan donde es apropiado

### Escalabilidad
- [ ] El código puede manejar la carga esperada
- [ ] Sin operaciones bloqueantes en el hilo principal
- [ ] El uso de recursos escala apropiadamente
- [ ] Las consultas a base de datos escalan con el crecimiento de datos

---

## 6. Problemas Encontrados

### Problemas Críticos
- [ ] **Problema 1:** [Descripción del problema crítico]
- [ ] **Problema 2:** [Descripción del problema crítico]

### Problemas Mayores
- [ ] **Problema 1:** [Descripción del problema mayor]
- [ ] **Problema 2:** [Descripción del problema mayor]

### Problemas Menores
- [ ] **Problema 1:** [Descripción del problema menor]
- [ ] **Problema 2:** [Descripción del problema menor]

### Sugerencias de Mejora
- [ ] **Sugerencia 1:** [Descripción de la sugerencia de mejora]
- [ ] **Sugerencia 2:** [Descripción de la sugerencia de mejora]

---

## 7. Retroalimentación Positiva

### Lo Que Se Hizo Bien
- [ ] **Fortaleza 1:** [Descripción de lo que se hizo bien]
- [ ] **Fortaleza 2:** [Descripción de lo que se hizo bien]
- [ ] **Fortaleza 3:** [Descripción de lo que se hizo bien]

### Mejores Prácticas Seguidas
- [ ] **Práctica 1:** [Descripción de mejor práctica seguida]
- [ ] **Práctica 2:** [Descripción de mejor práctica seguida]

---

## 8. Resumen de la Revisión

### Evaluación General
**Calificación General:** [Excelente, Buena, Regular, Mala]

**Resumen:** [Breve resumen de los hallazgos de la revisión, destacando problemas clave y fortalezas]

### Entregables
- Un resumen de revisión de código con retroalimentación detallada sobre calidad de código, seguridad y rendimiento.
- Una lista de problemas identificados, categorizados por gravedad.
- Una recomendación clara (Aprobar, Solicitar Cambios o Rechazar).

### Recomendación
- [ ] **Aprobar** - El código está listo para fusionar
- [ ] **Aprobar con cambios menores** - Fusionar después de abordar problemas menores
- [ ] **Solicitar cambios** - Abordar problemas mayores antes de fusionar
- [ ] **Rechazar** - Problemas significativos necesitan resolverse

### Próximos Pasos
1. [Elemento de acción 1]
2. [Elemento de acción 2]
3. [Elemento de acción 3]

---

## 9. Instrucciones para el Agente de IA

### Proceso de Revisión
🎯 **PROCESO OBLIGATORIO:**
1.  **Análisis de Código:** Analiza minuciosamente todos los archivos cambiados, enfocándote en las áreas mencionadas en las secciones de revisión anteriores.
2.  **Entendimiento del Contexto:** Entiende el propósito y contexto de los cambios revisando la descripción del PR y los problemas relacionados.
3.  **Revisión Completa:** Verifica calidad de código, funcionalidad, seguridad, rendimiento y adherencia a estándares del proyecto.
4.  **Identificación de Problemas:** Identifica y categoriza problemas por gravedad (Crítica, Mayor, Menor).
5.  **Retroalimentación Positiva:** Reconoce buenas prácticas y características bien implementadas.
6.  **Recomendaciones Claras:** Proporciona retroalimentación específica y accionable para mejorar.
7.  **Evaluación Final:** Haz una recomendación clara sobre si aprobar o solicitar cambios.

### Áreas de Enfoque de Revisión
- **Calidad de Código:** Legibilidad, mantenibilidad y adherencia a estándares de codificación
- **Funcionalidad:** Corrección, completitud y manejo adecuado de errores
- **Seguridad:** Vulnerabilidades potenciales y prácticas de codificación segura
- **Rendimiento:** Eficiencia y consideraciones de escalabilidad
- **Pruebas:** Cobertura de pruebas adecuada y calidad
- **Documentación:** Claridad y completitud de la documentación del código

### Pautas de Comunicación
- Sé constructivo y específico en la retroalimentación
- Proporciona ejemplos y sugerencias para mejoras
- Equilibra la crítica con refuerzo positivo
- Enfócate en el código, no en la persona
- Haz preguntas aclaratorias cuando sea necesario
- Prioriza problemas por gravedad e impacto

---

## 10. Lista de Verificación de Revisión

### Pre-Revisión
- [ ] El pull request está descrito adecuadamente
- [ ] Todas las comprobaciones requeridas están pasando
- [ ] El código está formateado adecuadamente
- [ ] Las pruebas están incluidas y pasando

### Durante la Revisión
- [ ] Todos los archivos cambiados son revisados
- [ ] La lógica del código se entiende
- [ ] Se consideran las implicaciones de seguridad
- [ ] Se evalúa el impacto en el rendimiento
- [ ] La cobertura de pruebas es adecuada

### Post-Revisión
- [ ] Todos los problemas están claramente documentados
- [ ] Las recomendaciones son accionables
- [ ] La revisión se completa de manera oportuna
- [ ] Se planifica seguimiento para cambios solicitados