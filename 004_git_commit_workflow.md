# Flujo de Trabajo de Commit de Git

Este documento describe el procedimiento estándar para hacer commit de cambios de código en un repositorio. Todos los colaboradores, incluidos los agentes de IA, deben seguir estas pautas para mantener un historial de commits limpio, legible y consistente.

## Principios Básicos

- **Commits Atómicos:** Cada commit debe representar un único cambio lógico. Evita agrupar cambios no relacionados en un solo commit.
- **Claridad:** Los mensajes de commit deben ser claros, concisos y descriptivos. Sirven como la documentación principal para la historia del proyecto.
- **Consistencia:** Seguir un formato consistente para los mensajes de commit hace que la historia sea más fácil de leer y permite que herramientas automatizadas la analicen.

## El Proceso de Commit

Sigue estos pasos cada vez que hagas commit de cambios:

1.  **Verificar Rama:**
    *   Asegúrate de estar en la rama correcta para los cambios que estás comiteando.
    *   **Comando:** `git branch --show-current`

2.  **Revisar Cambios:**
    *   Antes de preparar (stage), verifica las modificaciones que has hecho.
    *   **Comando:** `git status`
    *   **Comando:** `git diff` (para ver cambios no preparados)
    *   **Comando:** `git diff --staged` (para ver cambios preparados)

2.  **Preparar Archivos (Stage):**
    *   Agrega solo los archivos que pertenecen a un único cambio lógico al área de preparación.
    *   **Comando:** `git add <ruta_archivo_1> <ruta_archivo_2>`
    *   Para archivos nuevos: `git add <ruta_nuevo_archivo>`

3.  **Construir el Mensaje de Commit:**
    *   El mensaje de commit **debe** seguir la especificación [Conventional Commits](https://www.conventionalcommits.org/en/v1.0.0/).
    *   El formato es: `tipo(ámbito): asunto`
    *   **`tipo`**: Debe ser uno de los siguientes:
        *   **feat**: Una nueva característica.
        *   **fix**: Una corrección de error.
        *   **docs**: Cambios solo de documentación.
        *   **style**: Cambios que no afectan el significado del código (espacios en blanco, formato, falta de punto y coma, etc.).
        *   **refactor**: Un cambio de código que no arregla un error ni agrega una característica.
        *   **perf**: Un cambio de código que mejora el rendimiento.
        *   **test**: Agregar pruebas faltantes o corregir pruebas existentes.
        *   **build**: Cambios que afectan el sistema de construcción o dependencias externas (ej., `pyproject.toml`, `package.json`).
        *   **ci**: Cambios en archivos y scripts de configuración de CI.
        *   **chore**: Otros cambios que no modifican archivos `src` o `test`.
    *   **`ámbito`** (opcional): Un sustantivo que especifica la sección del código base afectada (ej., `api`, `ui`, `database`).
    *   **`asunto`**: Una descripción concisa del cambio.
        *   Usa el modo imperativo, tiempo presente: "add" no "added" ni "adds".
        *   No capitalices la primera letra.
        *   Sin punto (.) al final.
    *   **`cuerpo`** (opcional): Una descripción más larga que proporciona contexto y el "por qué" detrás del cambio. Úsalo para explicar qué y por qué vs. cómo.
    *   **`pie`** (opcional):
        *   Úsalo para `BREAKING CHANGE:` seguido de una descripción del cambio. Un cambio rompedor **debe** tener un `!` después del tipo/ámbito (ej., `feat(api)!: ...`).
        *   Úsalo para referenciar números de issues (ej., `Closes #123`).

4.  **Proponer el Commit:**
    *   Como agente de IA, debes presentar el mensaje de commit completo al usuario para su aprobación antes de ejecutar el commit.

5.  **Esperar Aprobación del Usuario:**
    *   No procedas con el comando `git commit` hasta que el usuario lo apruebe explícitamente.

6.  **Ejecutar el Commit:**
    *   Una vez aprobado, ejecuta el comando de commit.
    *   **Comando:** `git commit -m "<asunto>" -m "<cuerpo>"`

7.  **Verificar:**
    *   Después de hacer commit, ejecuta `git log -1` para asegurar que el commit se creó correctamente.

## Ejemplos de Mensajes de Commit

### Característica (Feature)
```
feat(agent): add tool for reading CSV files

The new CsvReaderTool allows the agent to ingest and process data from CSV files, enabling it to answer questions based on structured data.
```

### Corrección con Ámbito (Fix with Scope)
```
fix(api): correct pagination logic for user endpoint

The pagination for the `/users` endpoint was not calculating the offset correctly, causing it to skip records on subsequent pages. This commit fixes the offset calculation.

Closes #42
```

### Cambio Rompedor (Breaking Change)
```
refactor(auth)!: replace JWT with session-based authentication

BREAKING CHANGE: The authentication mechanism has been changed from stateless JWT tokens to stateful server-side sessions. All API clients must be updated to handle cookies for session management instead of sending an `Authorization` header.
```

### Documentación
```
docs: update README with new setup instructions
```

### Entregables
- Un commit de Git con un mensaje que se adhiere a la especificación Conventional Commits.
- El commit debe representar un cambio lógico único.