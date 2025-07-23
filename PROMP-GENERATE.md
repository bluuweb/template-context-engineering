**Rol**: Actúa como un experto en ingeniería de contexto y un desarrollador senior. Tu objetivo es crear un **Prompt de Requisitos de Producto (PRP)** completo y detallado.

**Instrucción Crítica**: Utiliza los siguientes archivos de contexto como tu única fuente de verdad y referencia. Tu tarea es sintetizar la información de estos archivos para producir un PRP que sirva como un "plano" para una IA de codificación.

**Archivos de Contexto**:

1.  `GEMINI.md`: Reglas globales y anti-patrones que deben seguirse.
2.  `PRP_BASE.md`: La plantilla base para la estructura del PRP.
3.  `INITIAL.md`: Requisitos específicos, tecnologías y características del proyecto actual.

**Proceso de Generación del PRP**:

1.  **Investigación y Contextualización**:

    - Lee y comprende el `INITIAL.md` para identificar la tecnología, propósito, y características clave.
    - Sigue los principios de `GEMINI.md`, como la inmersión profunda en la documentación y la extracción de patrones, para entender el proyecto en su totalidad.

2.  **Adaptación de la Plantilla**:

    - Utiliza `prp_base.md` como la estructura principal.
    - Rellena cada sección del template con la información extraída de tu investigación y del `INITIAL.md`.
    - Asegúrate de que el PRP resultante sea denso en información y claro en sus directivas.

3.  **Definición del Plan de Implementación**:

    - Basándote en los requisitos, crea una lista de tareas ordenada y modular.
    - Define los modelos de datos y la estructura necesaria.
    - Identifica los puntos de integración (ej. base de datos, configuración, rutas).

4.  **Creación del Ciclo de Validación**:

    - Diseña un ciclo de validación específico para el proyecto.
    - Incluye comandos de prueba para sintaxis, estilo, pruebas unitarias y de integración.
    - Asegúrate de que los criterios de validación sean claros y medibles.

5.  **Revisión Final**:
    - Revisa el PRP final para asegurar que cumple con todos los principios y anti-patrones de `GEMINI.md`.
    - Verifica que toda la información crítica, como los "gotchas" y los patrones, esté documentada de forma explícita.

**Instrucción Final**: Genera el PRP completo en formato Markdown, listo para ser utilizado por una IA de codificación. El nombre del archivo debe ser `PRP_{nombre_proyecto}.md`.
