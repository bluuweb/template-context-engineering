### Plantilla Base para PRP v2 - Rica en Contexto con Ciclos de Validación

Este documento sirve como una plantilla para generar un **Prompt de Requisitos de Producto (PRP)** completo, diseñado para guiar a un agente de IA en la implementación de una característica o un proyecto con el máximo contexto y capacidades de autovalidación.

#### Principios Fundamentales del PRP

1.  **Contexto es la clave**: Proporcionar toda la documentación, ejemplos, y advertencias necesarias.
2.  **Ciclos de Validación**: Incluir pasos de prueba o validación que la IA pueda ejecutar y corregir.
3.  **Información densa**: Usar palabras clave y patrones específicos del código existente.
4.  **Éxito Progresivo**: Empezar de forma simple, validar cada paso, y luego expandir.
5.  **Reglas Globales**: Asegurarse de seguir todas las reglas globales de ingeniería de contexto.

---

#### 1. Objetivo del Proyecto/Funcionalidad

- **Qué se debe construir**: Descripción concisa del objetivo final.
- **Por qué**: Valor de negocio, impacto en el usuario, y cómo se integra con el proyecto actual.
- **Criterios de Éxito**: Lista de resultados medibles para determinar si la implementación es exitosa.

---

#### 2. Contexto Necesario

- **Documentación y Referencias**:

  - **Docs Oficiales**: URL de la documentación de la librería/framework y qué secciones son relevantes.
  - **Archivos de Ejemplo**: Ruta a archivos existentes que muestran el patrón de código a seguir o a evitar.
  - **Gotchas del Proyecto**: Advertencias sobre configuraciones específicas del proyecto, dependencias o patrones de código que la IA debe conocer.

- **Estructura del Código Actual**:

  - Descripción de la estructura de directorios del proyecto. (Puedes pedirle a la IA que use `tree` o una herramienta similar para autogenerar esto).

- **Estructura del Código Deseada**:
  - Especifica qué archivos se deben crear o modificar y cuál es la responsabilidad de cada uno.

---

#### 3. Plan de Implementación

- **Modelos de Datos y Estructura**:

  - Define los modelos de datos, esquemas, y validadores necesarios para la funcionalidad.

- **Tareas a Completar**:

  - Lista numerada y ordenada de las tareas de implementación. Cada tarea debe ser clara y modular.
  - **Ejemplo**: `MODIFICAR src/api/routes.py`: Agregar un nuevo endpoint.

- **Pseudocódigo (si es necesario)**:

  - Fragmentos de pseudocódigo que ilustren patrones críticos, manejo de errores y advertencias (`gotchas`). No debe ser el código completo, sino una guía.

- **Puntos de Integración**:
  - **Base de datos**: Migraciones necesarias, índices o cambios en el esquema.
  - **Configuración**: Variables de entorno, configuraciones en archivos `.json` o `.env`.
  - **Rutas/Endpoints**: Nuevas rutas o modificaciones a las existentes.

---

#### 4. Ciclo de Validación

- **Nivel 1: Sintaxis y Estilo**:

  - Comandos de Linter (ej. `npm run lint`) y Type Checking (ej. `tsc`) que la IA debe ejecutar y corregir antes de continuar.

- **Nivel 2: Pruebas Unitarias**:

  - Ejemplos de casos de prueba que la IA debe generar y pasar para la nueva funcionalidad (ej. `happy path`, `edge cases`, `error handling`).

- **Nivel 3: Pruebas de Integración (si aplica)**:

  - Comandos (ej. `curl`) o descripciones de pruebas manuales para verificar que la funcionalidad se integra correctamente.

- **Checklist de Validación Final**:
  - Lista de verificación para asegurar que todas las pruebas pasaron, no hay errores de linting, la funcionalidad es estable, y el manejo de errores es robusto.

---

#### 5. Anti-patrones a Evitar

- Lista de prácticas específicas del proyecto o la tecnología que la IA debe evitar.
