# Solicitud de Generación de Template

## TECNOLOGÍA/FRAMEWORK:

**Ejemplo:** Agentes Pydantic AI
**Ejemplo:** Aplicaciones frontend Supabase
**Ejemplo:** Sistemas multi-agente CrewAI

**Tu tecnología:** \[Especifica el framework exacto, librería o tecnología para la cual quieres crear un template de context engineering]

---

## PROPÓSITO DEL TEMPLATE:

**¿Para qué caso de uso específico debería estar optimizado este template?**

**Ejemplo para Pydantic AI:** "Construir agentes IA inteligentes con integración de herramientas, manejo de conversaciones y validación de datos estructurados usando el framework Pydantic AI"

**Ejemplo para Supabase:** "Crear aplicaciones web full-stack con datos en tiempo real, autenticación y funciones serverless usando Supabase como backend"

**Tu propósito:** \[Sé muy específico sobre lo que los desarrolladores deberían poder construir fácilmente con este template]

---

## CARACTERÍSTICAS CENTRALES:

**¿Cuáles son las características esenciales que este template debería ayudar a los desarrolladores a implementar?**

**Ejemplo para Pydantic AI:**

- Creación de agentes con diferentes proveedores de modelo (OpenAI, Anthropic, Gemini)
- Patrones de integración de herramientas (búsqueda web, operaciones de archivos, llamadas API)
- Memoria de conversación y gestión de contexto
- Validación de salida estructurada con modelos Pydantic
- Manejo de errores y mecanismos de reintento
- Patrones de testing para comportamiento de agentes IA

**Ejemplo para Supabase:**

- Diseño de esquema de base de datos y migraciones
- Suscripciones en tiempo real y actualizaciones de datos en vivo
- Implementación de políticas Row Level Security (RLS)
- Flujos de autenticación (email, OAuth, magic links)
- Funciones edge serverless para lógica de backend
- Almacenamiento de archivos e integración CDN

**Tus características centrales:** \[Lista las capacidades específicas que los desarrolladores deberían poder implementar fácilmente]

---

## EJEMPLOS A INCLUIR:

**¿Qué ejemplos funcionales deberían estar incluidos en el template?**

**Ejemplo para Pydantic AI:**

- Agente de chat básico con memoria
- Agente con herramientas habilitadas (búsqueda web + calculadora)
- Agente con flujo de trabajo de múltiples pasos
- Agente con modelos Pydantic personalizados para salidas estructuradas
- Ejemplos de pruebas para respuestas de agente y uso de herramientas

**Ejemplo para Supabase:**

- Autenticación de usuario y gestión de perfiles
- Sistema de mensajería o chat en tiempo real
- Funcionalidad para subir y compartir archivos
- Patrones de aplicación multi-tenant
- Disparadores de base de datos y funciones

**Tus ejemplos:** \[Especifica ejemplos funcionales concretos que deberían incluirse]

---

## DOCUMENTACIÓN A INVESTIGAR:

**¿Qué documentación específica debe investigarse a fondo y referenciarse?**

**Ejemplo para Pydantic AI:**

- [https://ai.pydantic.dev/](https://ai.pydantic.dev/) - Documentación oficial de Pydantic AI
- [https://docs.pydantic.dev/](https://docs.pydantic.dev/) - Librería de validación de datos Pydantic
- APIs de proveedores de modelos (OpenAI, Anthropic) para patrones de integración
- Buenas prácticas y ejemplos de integración de herramientas
- Frameworks de testing para aplicaciones de IA

**Ejemplo para Supabase:**

- [https://supabase.com/docs](https://supabase.com/docs) - Documentación completa de Supabase
- [https://supabase.com/docs/guides/auth](https://supabase.com/docs/guides/auth) - Guía de autenticación
- [https://supabase.com/docs/guides/realtime](https://supabase.com/docs/guides/realtime) - Características en tiempo real
- Patrones de diseño de base de datos y políticas RLS
- Desarrollo y despliegue de funciones edge

**Tu documentación:** \[Lista URLs y secciones específicas de documentación a investigar en profundidad]

---

## PATRONES DE DESARROLLO:

**¿Qué patrones de desarrollo, estructuras de proyecto o flujos de trabajo deberían investigarse e incluirse?**

**Ejemplo para Pydantic AI:**

- Cómo estructurar módulos de agentes y definiciones de herramientas
- Gestión de configuración para diferentes proveedores de modelo
- Configuración del entorno para desarrollo vs producción
- Patrones de logging y monitoreo para agentes IA
- Patrones de control de versiones para prompts y configuraciones de agente

**Ejemplo para Supabase:**

- Patrones de estructura de proyecto Frontend + Supabase
- Flujo de trabajo de desarrollo local con Supabase CLI
- Estrategias de migración y versionado de base de datos
- Gestión de entornos (local, staging, producción)
- Estrategias de testing para aplicaciones full-stack con Supabase

**Tus patrones de desarrollo:** \[Especifica los flujos de trabajo y patrones organizacionales a investigar]

---

## SEGURIDAD Y MEJORES PRÁCTICAS:

**¿Qué consideraciones de seguridad y mejores prácticas son críticas para esta tecnología?**

**Ejemplo para Pydantic AI:**

- Gestión y rotación de claves API
- Validación y saneamiento de entradas para agentes
- Limitación de tasa y monitoreo de uso
- Prevención de inyecciones en prompts
- Control y monitoreo de costos por uso de modelos

**Ejemplo para Supabase:**

- Diseño de políticas Row Level Security (RLS)
- Patrones de autenticación con claves API vs JWT
- Seguridad de base de datos y control de acceso
- Seguridad en la carga de archivos y escaneo de virus
- Limitación de tasa y prevención de abusos

**Tus consideraciones de seguridad:** \[Lista los patrones de seguridad específicos de la tecnología a investigar y documentar]

---

## GOTCHAS COMUNES:

**¿Cuáles son los errores típicos, casos límite o problemas complejos que enfrentan los desarrolladores con esta tecnología?**

**Ejemplo para Pydantic AI:**

- Limitaciones de longitud de contexto del modelo y su gestión
- Manejo de límites de tasa y errores de proveedores de modelo
- Conteo de tokens y optimización de costos
- Gestión del estado de conversación entre peticiones
- Manejo de errores de ejecución de herramientas y reintentos

**Ejemplo para Supabase:**

- Debugging y testing de políticas RLS
- Rendimiento de suscripciones en tiempo real con grandes volúmenes de datos
- Arranque en frío y optimización de funciones edge
- Agrupación de conexiones a base de datos en entornos serverless
- Configuración CORS para diferentes dominios

**Tus gotchas:** \[Identifica los desafíos específicos que comúnmente enfrentan los desarrolladores]

---

## REQUISITOS DE VALIDACIÓN:

**¿Qué validaciones, pruebas o controles de calidad específicos deberían incluirse en el template?**

**Ejemplo para Pydantic AI:**

- Pruebas de calidad de respuestas de agentes
- Testing de integración de herramientas
- Pruebas de fallback con proveedores de modelo
- Benchmarking de costos y rendimiento
- Validación de flujo conversacional

**Ejemplo para Supabase:**

- Pruebas de migración de base de datos
- Validación de políticas RLS
- Pruebas de funcionalidades en tiempo real
- Testing de flujos de autenticación
- Testing de integración de funciones edge

**Tus requisitos de validación:** \[Especifica los patrones de prueba y validación necesarios]

---

## ENFOQUE DE INTEGRACIÓN:

**¿Qué integraciones específicas o servicios de terceros se usan comúnmente con esta tecnología?**

**Ejemplo para Pydantic AI:**

- Integración con bases vectoriales (Pinecone, Weaviate)
- Herramientas y APIs de web scraping
- Integraciones con APIs externas para herramientas
- Servicios de monitoreo (Weights & Biases, LangSmith)
- Plataformas de despliegue (Modal, Replicate)

**Ejemplo para Supabase:**

- Frameworks frontend (Next.js, React, Vue)
- Procesamiento de pagos (Stripe)
- Servicios de email (SendGrid, Resend)
- Procesamiento de archivos (optimización de imágenes, análisis de documentos)
- Herramientas de monitoreo y analítica

**Tu enfoque de integración:** \[Lista las integraciones clave a investigar e incluir]

---

## NOTAS ADICIONALES:

**¿Hay otros requisitos, restricciones o consideraciones específicas para este template?**

**Ejemplo:** "Enfocarse en patrones con TypeScript e incluir definiciones de tipos completas"
**Ejemplo:** "Enfatizar patrones de despliegue serverless y optimización de costos"
**Ejemplo:** "Incluir patrones tanto para casos de uso principiantes como avanzados"

**Tus notas adicionales:** \[Cualquier otra consideración importante]

---

## NIVEL DE COMPLEJIDAD DEL TEMPLATE:

**¿Qué nivel de complejidad debe tener este template?**

- [ ] **Principiante** - Patrones simples para empezar
- [ ] **Intermedio** - Patrones listos para producción con características comunes
- [ ] **Avanzado** - Patrones comprehensivos que incluyan escenarios complejos
- [ ] **Empresarial** - Patrones completos de nivel empresarial con monitoreo, escalado y seguridad

**Tu elección:** \[Selecciona el nivel de complejidad apropiado y explica por qué]

---

**RECORDATORIO: Sé lo más específico posible en cada sección. Cuanto más detallado seas aquí, mejor será el template generado. Este archivo INITIAL.md es donde debes poner todos tus requisitos, no solo información básica.**
