### Solicitud de Generación de Template

#### TECNOLOGÍA/FRAMEWORK:

**Tu tecnología:** **Next.js (con App Router)**, **React**, **Tailwind CSS**, **Prisma**, **MongoDB (Atlas)**, **NextAuth.js**, **Zustand**.

---

#### PROPÓSITO DEL TEMPLATE:

**Tu propósito:** Crear una **aplicación web full-stack altamente optimizada, fácil de navegar y extremadamente rápida (lightning fast)**, que funcione como un **clon completo de Airbnb**. Este template debería permitir a los desarrolladores construir fácilmente una experiencia de usuario fluida y responsiva en **todos los dispositivos (desde escritorio hasta móvil)**, con capacidades avanzadas de búsqueda, reserva y gestión de propiedades, aprovechando los **Server Components de Next.js para la obtención directa de datos de la base de datos** y los **Client Components para la construcción de la interfaz de usuario**.

---

#### CARACTERÍSTICAS CENTRALES:

**Tus características centrales:**

- **Desarrollo Full-Stack:** Construcción de una aplicación completa que abarca tanto el frontend como el backend.
- **Next.js App Router:** Utilización de la nueva estructura de `app directory` para el manejo de rutas y el renderizado avanzado.
- **Componentes de Servidor (Server Components):** Implementación para **obtener datos directamente de la base de datos**, optimizando el rendimiento y la experiencia de usuario.
- **Componentes de Cliente (Client Components):** Uso para construir la interfaz de usuario (UI) interactiva y asegurar un diseño fluido y responsivo.
- **Diseño Responsivo con Tailwind CSS:** Creación de una apariencia moderna y elegante, completamente responsiva para **todos los dispositivos**, con animaciones y efectos.
- **Autenticación Flexible:** Implementación de **autenticación por credenciales** (email/contraseña), así como **integración con Google y GitHub OAuth** para un proceso de inicio de sesión sin interrupciones.
- **Carga y Gestión de Imágenes:** Utilización de **Cloudinary CDN** para la carga de imágenes.
- **Validación y Manejo de Formularios:** Implementación de `React Hook Form` para la validación y el manejo de formularios, incluyendo validación en el cliente.
- **Manejo de Errores de Servidor:** Uso de `React Toast` para mostrar mensajes de éxito y error en el cliente.
- **Sistema de Reservas y Calendario:** Integración de `React Date Range` para la selección de fechas en calendarios y un sistema robusto de reserva y cancelación (para huéspedes y propietarios).
- **Gestión de Propiedades:** Funcionalidades para la **creación y eliminación de propiedades** por parte de los usuarios.
- **Cálculo Avanzado de Precios:** Funcionalidad para calcular el precio total de las reservas basado en el rango de fechas.
- **Algoritmo de Búsqueda Avanzado:** Filtrado de resultados por categoría, rango de fechas, ubicación en el mapa, número de huéspedes, habitaciones y baños.
- **Sistema de Favoritos:** Permite a los usuarios marcar propiedades como favoritas y gestionarlas.
- **Filtros de URL Compartibles:** La capacidad de compartir URLs con filtros aplicados, permitiendo a otros usuarios (incluso no registrados) ver los mismos resultados.
- **Estados de Carga y Vacíos:** Implementación de estados de carga (`loading.tsx`) y estados vacíos (`empty-state`) para una mejor experiencia de usuario.

---

#### EJEMPLOS A INCLUIR:

**Your examples:**

- **Configuración del Entorno:** Inicio de un proyecto Next.js con App Router y TypeScript, configuración de Tailwind CSS, gestión de fuentes con `next/font` y configuración de variables de entorno.
- **Componentes de Navegación:** Creación de `Navbar`, `Container`, `Logo`, `Search` y `UserMenu`, demostrando la organización de componentes y el uso de `use client`.
- **Modales de Autenticación:** Implementación de los modales de Registro y Login, con formularios de credenciales y botones para autenticación social (Google y GitHub).
- **Gestión de Usuario Actual:** Obtención del usuario actual usando `getServerSession` en un Server Component y pasándolo a Client Components, con sanitización de objetos `Date`.
- **Funcionalidad de Logout:** Implementación para cerrar la sesión del usuario.
- **Creación de Listados (Rent Model):** Un flujo de múltiples pasos (categoría, ubicación, información, imágenes, descripción, precio) para que los usuarios puedan crear nuevas propiedades, utilizando componentes reutilizables como `CategoryInput`, `CountrySelect`, `Counter` e `ImageUpload`.
- **Integración con Bases de Datos:** Configuración de Prisma y MongoDB Atlas, definición de esquemas para `User`, `Account`, `Listing` y `Reservation`, y migraciones de esquemas (`npx prisma db push`).
- **API Routes (Next.js):** Implementación de rutas de API en el App Router (`route.ts`) para:
  - Registro de usuarios (`/api/register`).
  - Creación de listados (`/api/listings`).
  - Creación de reservas (`/api/reservations`).
  - Manejo de favoritos (POST y DELETE en `/api/favorites/[listingId]`).
  - Cancelación de reservas (DELETE en `/api/reservations/[reservationId]`).
  - Eliminación de listados (`/api/listings/[listingId]`).
- **Visualización de Listados:** Muestra todos los listados en la página principal (`page.tsx`), utilizando el componente `ListingCard`.
- **Página Individual de Listado:** Una vista detallada de un listado específico, incluyendo información del anfitrión y un calendario de reservas (`listing-client.tsx`).
- **Páginas Específicas del Usuario:**
  - **Mis Viajes (`/trips`):** Muestra todas las reservas que el usuario ha hecho.
  - **Mis Reservas (`/reservations`):** Muestra todas las reservas hechas en las propiedades del usuario.
  - **Mis Propiedades (`/properties`):** Muestra todos los listados creados por el usuario.
  - **Mis Favoritos (`/favorites`):** Muestra todos los listados que el usuario ha marcado como favoritos.
- **Sistema de Búsqueda y Filtros:** Funcionalidad completa de búsqueda con filtros dinámicos que actualizan la URL y persisten, mostrando resultados filtrados.
- **Manejo de Estados de Carga y Error:** Implementación de `loading.tsx` y `error.tsx` para una experiencia de usuario robusta durante las operaciones asíncronas.

---

#### DOCUMENTATION TO RESEARCH:

**Your documentation:**

- **Next.js:**
  - Documentación oficial de Next.js (especialmente la sección de **App Router**): **https://nextjs.org/docs/app/**.
  - Guías sobre **Server Components** y **Client Components**.
  - Manejo de **API Routes** (`route.ts`) en el App Router.
  - Optimización de imágenes con `next/image`.
  - `next/font` para la optimización de fuentes.
  - Manejo de `useRouter` y `useSearchParams` para el enrutamiento del cliente y los parámetros de URL.
  - `next/server` para `NextResponse` en API Routes.
  - `next/dynamic` para la importación dinámica de componentes.
  - **Middleware** de Next.js para proteger rutas.
- **React:**
  - Documentación oficial de React para Hooks (`useState`, `useEffect`, `useCallback`, `useMemo`).
- **Tailwind CSS:**
  - Documentación oficial de Tailwind CSS: **https://tailwindcss.com/docs**.
  - Clases para diseño responsivo, utilidades de diseño, animaciones y efectos.
- **Prisma:**
  - Documentación oficial de Prisma: **https://www.prisma.io/docs/**.
  - Definición de esquemas (`schema.prisma`), modelos (`model User`, `model Listing`, etc.), y relaciones (`@relation`).
  - Operaciones de base de datos (`findUnique`, `create`, `update`, `deleteMany`, `findMany`).
  - Configuración con MongoDB.
  - Extensiones de Prisma para VS Code.
- **MongoDB Atlas:**
  - Guías de conexión y creación de bases de datos en la nube: **https://www.mongodb.com/cloud/atlas**.
- **NextAuth.js:**
  - Documentación oficial de NextAuth.js: **https://next-auth.js.org/docs**.
  - Proveedores de autenticación (Google, GitHub) y credenciales.
  - Manejo de sesiones (`getServerSession`).
  - Manejo de `signIn` y `signOut` desde el cliente.
- **Cloudinary:**
  - Documentación oficial de Cloudinary para carga y gestión de imágenes: **https://cloudinary.com/documentation**.
  - Widgets de carga (`CldUploadWidget`) y presets de carga.
- **React Hook Form:**
  - Documentación oficial de React Hook Form: **https://react-hook-form.com/docs**.
  - Uso de `useForm`, `register`, `handleSubmit`, `watch`, `formState` y `reset`.
- **React Hot Toast:**
  - Documentación para notificaciones tipo "toast": **https://react-hot-toast.com/**.
- **React Date Range:**
  - Documentación para componentes de calendario y selección de rangos de fechas: **https://hypeserver.github.io/react-date-range/**.
- **React Icons:**
  - Cómo usar iconos de diversas librerías (AI, BI, FC, GI, TB, BS, IO): **https://react-icons.github.io/react-icons/**.
- **Axios:**
  - Documentación para realizar peticiones HTTP (POST, DELETE).
- **Bcrypt.js:**
  - Cómo usar `bcrypt.hash` y `bcrypt.compare` para el manejo seguro de contraseñas.
- **Date-FNS:**
  - Funciones para el manejo de fechas (`format`, `eachDayOfInterval`, `differenceInCalendarDays`, `formatISO`).
- **Zustand:**
  - Cómo crear un almacén de estado ligero para la gestión de modales: **https://zustand-demo.pmnd.rs/**.
- **Query String (qs):**
  - Cómo parsear y stringificar parámetros de URL para filtros.
- **World Countries:**
  - Cómo obtener datos de países para el selector de ubicación.
- **Leaflet & React-Leaflet:**
  - Documentación para la integración de mapas interactivos: **https://react-leaflet.js.org/**.
- **React Spinners:**
  - Documentación para animaciones de carga: **https://www.react-spinners.com/**.

---

#### DEVELOPMENT PATTERNS:

**Your development patterns:**

- **Estructura de Carpetas Modular:** Organización clara de la aplicación en carpetas como `app` (raíz del App Router), `components` (con subcarpetas para `navbar`, `models`, `inputs`, `listings`), `hooks`, `libs` (para Prisma DB), `actions` (para la lógica del servidor/base de datos), `providers` (para envolver librerías externas), y `types` (para la definición de tipos global).
- **Segregación Server vs. Client Components:** Patrón de diseño crucial en Next.js donde los **Server Components se usan para la lógica de negocio y obtención de datos del backend**, mientras que los **Client Components se usan para la interactividad de la UI**.
- **Manejo de Errores de Hidratación:** Utilización de un componente `ClientOnly` para envolver componentes de cliente que dependen de estado o efectos, previniendo errores de "text content does not match".
- **Gestión de Estado Global (Zustand):** Implementación de un `store` ligero con Zustand para el control de la visibilidad de los modales (registro, login, renta, búsqueda).
- **Control de Formularios con `React Hook Form`:** Estructuración de formularios complejos, con `register`, `handleSubmit`, `watch` y `formState` para una validación eficiente y una experiencia de usuario fluida.
- **Manejo de Rutas de API (Route Handlers):** Definición de funciones asíncronas exportadas (`export async function POST`, `GET`, `DELETE`, etc.) en archivos `route.ts` dentro de la carpeta `app/api` para las operaciones del backend.
- **Utilidad de Prisma Client:** Creación de una instancia de Prisma Client global para evitar múltiples instanciaciones en desarrollo con hot-reloading.
- **Gestión de Variables de Entorno:** Uso de archivos `.env` y el prefijo `NEXT_PUBLIC_` para variables accesibles en el cliente.
- **Importaciones Dinámicas (`next/dynamic`):** Importación de componentes pesados o que solo se renderizan en el cliente (como el mapa de Leaflet) con `SSR: false` para evitar problemas de renderizado del lado del servidor.
- **Manejo de Parámetros de URL:** Uso de `useRouter` y `useSearchParams` para construir URLs con filtros complejos, lo que permite compartir los estados de búsqueda y mantiene la persistencia.
- **Reutilización de Componentes:** Diseño de componentes genéricos (ej. `Input`, `Button`, `Heading`, `Counter`, `Calendar`, `ListingCard`) para maximizar la reutilización en toda la aplicación.
- **Manejo de CSS Global:** Sobrescritura de estilos de librerías de terceros en `globals.css` para asegurar una apariencia coherente.
- **Autenticación con Middleware:** Implementación de un middleware de NextAuth.js para proteger rutas específicas del lado del servidor, redirigiendo a usuarios no autenticados.

---

#### SECURITY & BEST PRACTICES:

**Your security considerations:**

- **Gestión Segura de Claves API:** Almacenamiento de claves sensibles (GitHub ID/Secret, Google Client ID/Secret, NextAuth Secret) en **variables de entorno** y no directamente en el código.
- **Hash de Contraseñas:** Uso de `bcrypt` para **hashear las contraseñas** antes de almacenarlas en la base de datos y para compararlas durante el inicio de sesión, en lugar de almacenar contraseñas en texto plano.
- **Políticas de Autenticación de NextAuth.js:** Configuración de `NextAuth.js` con proveedores específicos (credenciales, Google, GitHub) y uso de JWT para la gestión de sesiones.
- **Control de Acceso a la Base de Datos (Prisma):** Asegurar que las operaciones de creación, eliminación y actualización de datos solo puedan ser realizadas por usuarios autenticados y autorizados (ej. solo el propietario puede eliminar su propiedad, o el creador de la reserva puede cancelarla).
- **Validación de Entrada (Server-Side):** Realizar **validación de datos tanto en el cliente como en el servidor** (en las API routes) para prevenir inyecciones o datos malformados.
- **Sanitización de Datos (Server a Client):** **Convertir objetos `Date` a `ISO strings`** al pasar datos de Server Components a Client Components para evitar errores de hidratación y asegurar la compatibilidad de tipos.
- **Gestión de IP en MongoDB Atlas:** Configurar las reglas de acceso a la red en MongoDB Atlas, incluyendo la opción de permitir conexiones desde cualquier IP (`0.0.0.0/0`) para entornos de desarrollo/tutoriales, con advertencias sobre su uso en producción.
- **Seguridad en Carga de Imágenes:** Utilizar un servicio como Cloudinary que maneje de forma segura el almacenamiento y la entrega de imágenes, incluyendo la generación de URLs seguras.
- **Protección de Rutas:** Implementación de **middleware** para proteger rutas específicas (ej. `/trips`, `/favorites`) de usuarios no autenticados.
- **Prevenir el Phishing:** Advertencia explícita sobre no usar "Airbnb" en nombres de dominio o URLs de aplicaciones clonadas para evitar ser marcado por phishing.

---

#### COMMON GOTCHAS:

**Your gotchas:**

- **Errores de Hidratación:** La aparición de `Unhandled Runtime Error: Text content does not match server rendered HTML`, especialmente con componentes interactivos o estado del cliente en el App Router. La solución implica envolver estos componentes en un `ClientOnly` wrapper.
- **Diferencias entre Server y Client Components:** Confusión sobre cuándo usar la directiva `use client` y el impacto de pasar objetos no "plain" (como `Date` directamente) de Server a Client Components, lo que causa advertencias y posibles errores.
- **Ubicación de NextAuth.js API Route:** La necesidad de que las rutas de NextAuth.js permanezcan en la estructura de `pages/api/auth/[...nextauth].ts` en lugar del nuevo App Router, debido a que el soporte completo aún está en fase experimental.
- **Múltiples Instancias de Prisma Client:** Problemas en desarrollo con hot-reloading que pueden generar múltiples instancias de Prisma Client, resuelto mediante una estrategia de exportación global.
- **Configuración de `next.config.js` para Imágenes Externas:** Errores al cargar imágenes de dominios externos (ej. Cloudinary, GitHub, Google User Content) si no están configurados en la sección `images.domains` del archivo `next.config.js`.
- **Conflictos de CSS de Librerías:** Problemas de renderizado o estilos inesperados con librerías de terceros (ej. Leaflet, React Date Range) que requieren la importación de sus CSS y a veces la sobrescritura de reglas en `globals.css` (con `!important`).
- **Manejo de Fechas y Zonas Horarias:** Confusión con las funciones de `date-fns` (ej. `differenceInDays` vs. `differenceInCalendarDays`) que pueden llevar a cálculos incorrectos de días si no se tiene en cuenta la hora actual.
- **Reasignación de Iconos:** La necesidad de reasignar las URL predeterminadas de los iconos de Leaflet debido a que no funcionan correctamente con React sin configuración adicional.
- **Formatos de Variables de Entorno:** Olvidar el prefijo `NEXT_PUBLIC_` para las variables de entorno que deben ser accesibles en el lado del cliente.
- **Problemas de Caché de Next.js:** Errores de fuentes o comportamientos inesperados que a veces se resuelven eliminando la carpeta `.next/` (la caché de Next.js).
- **Exportaciones en Route Handlers:** Errores de rutas API (`404 not found`) si se usa `export default async function` en lugar de `export async function` en los archivos `route.ts` del App Router.

---

#### VALIDATION REQUIREMENTS:

**Your validation requirements:**

- **Validación de Formularios en Cliente:** Pruebas exhaustivas para asegurar que todos los campos requeridos en los formularios (registro, login, creación de listados) sean validados correctamente por `React Hook Form` antes del envío.
- **Manejo de Respuestas de API:** Verificación de que la aplicación maneje correctamente las respuestas exitosas (ej. `200 OK` con `toast.success`) y los errores (ej. `404`, `500` con `toast.error` o `NextResponse.error()`) de todas las llamadas a la API.
- **Estado de Autenticación del Usuario:** Validación de que las operaciones protegidas (ej. crear listados, hacer reservas, ver páginas de usuario) solo sean accesibles para usuarios autenticados, y que se redirija o se muestre un mensaje adecuado si no lo están.
- **Integridad de Datos en la Base de Datos:** Confirmar que los datos se almacenen y recuperen con precisión, manteniendo la unicidad (ej. email único) y las relaciones definidas en el esquema de Prisma.
- **Tipificación Estricta con TypeScript:** Realizar verificaciones de tipos para asegurar que las props de los componentes, los parámetros de las funciones y las estructuras de datos coincidan con las interfaces definidas (`SafeUser`, `SafeListing`, `SafeReservation`).
- **Responsividad de la UI:** Pruebas en diferentes tamaños de pantalla (móvil, tablet, escritorio) para confirmar que el diseño de Tailwind CSS se adapte y funcione correctamente.
- **Lógica de Filtros de Búsqueda:** Verificar que la aplicación de filtros por categoría, ubicación, fechas, número de huéspedes/habitaciones/baños, modifique correctamente la URL y que los resultados mostrados sean precisos.
- **Funcionalidad del Sistema de Reservas:** Asegurar que las fechas reservadas se deshabiliten en el calendario, que el cálculo de precios sea correcto y que las cancelaciones (tanto por el huésped como por el propietario) funcionen como se espera, liberando las fechas correspondientes.
- **Carga de Imágenes con Cloudinary:** Validar que la carga de imágenes se realice sin problemas, que las imágenes se almacenen correctamente en Cloudinary y que sus URLs se actualicen en la base de datos.

---

#### INTEGRATION FOCUS:

**Your integration focus:**

- **Next.js:** Como framework principal para el desarrollo full-stack, incluyendo Server Components, Client Components, y API Routes.
- **React:** Para la construcción de la interfaz de usuario interactiva y el manejo del estado con hooks.
- **Tailwind CSS:** Para un diseño de interfaz de usuario rápido, responsivo y basado en utilidades.
- **Prisma:** Como ORM (Object-Relational Mapper) para la interacción con la base de datos MongoDB.
- **MongoDB Atlas:** Como la base de datos NoSQL basada en la nube para el almacenamiento de datos.
- **NextAuth.js:** Para la gestión completa de la autenticación de usuarios, incluyendo autenticación por credenciales y OAuth con proveedores como Google y GitHub.
- **Cloudinary:** Para la gestión de carga y entrega de imágenes a través de su CDN.
- **React Hook Form:** Para simplificar la gestión de formularios complejos y su validación.
- **React Toast:** Para mostrar notificaciones `toast` informativas al usuario.
- **React Date Range:** Para ofrecer una interfaz de usuario interactiva para la selección de rangos de fechas.
- **React Icons:** Para un acceso fácil a una amplia variedad de iconos vectoriales para la UI.
- **Axios:** Como cliente HTTP para realizar solicitudes API desde el cliente a las rutas API de Next.js.
- **Bcrypt.js:** Para el hashing seguro de contraseñas.
- **Date-FNS:** Para el manejo y formato de fechas de manera eficiente.
- **Zustand:** Para una gestión de estado global ligera para la UI.
- **Query String (qs):** Para parsear y stringificar parámetros de URL, esencial para la funcionalidad de búsqueda y filtros.
- **World Countries:** Para obtener una lista de países y sus datos para el selector de ubicación.
- **Leaflet & React-Leaflet:** Para la integración de mapas interactivos que muestran la ubicación de las propiedades.
- **React Spinners:** Para implementar animaciones de carga visualmente atractivas.
- **Vercel:** Como la plataforma de despliegue para la aplicación.

---

#### ADDITIONAL NOTES:

**Your additional notes:**

- **Enfoque en TypeScript:** El template debe **priorizar el uso de TypeScript** con definiciones de tipos exhaustivas para asegurar la robustez y el mantenimiento del código.
- **Optimización del Rendimiento:** Énfasis en técnicas para lograr un rendimiento "lightning fast", como la **obtención de datos con Server Components** y el **manejo inteligente de caché**.
- **Experiencia de Usuario (UX):** Considerar la fluidez de las interacciones, las animaciones sutiles y los mensajes de feedback claros para una experiencia de usuario superior.
- **Patrones de Reutilización de Código:** Destacar cómo se reutilizan componentes y lógica (ej. `ListingCard`, `Button`, hooks personalizados) a lo largo de la aplicación para evitar la duplicación.
- **Modularidad:** Promover una estructura de proyecto modular que facilite la adición de nuevas características y el mantenimiento a largo plazo.
- **Despliegue Sencillo:** El template debe estar configurado para un **despliegue fácil y eficiente en Vercel**, incluyendo la gestión de variables de entorno para producción.
- **No Redundancia de API GET:** Un punto clave es que la aplicación **no necesita ningún endpoint GET de API** para la carga de listados o usuarios, ya que los Server Components se comunican directamente con la base de datos a través de `Prisma`.

---

#### TEMPLATE COMPLEXITY LEVEL:

**Your choice:** **Avanzado** - Este template abarca una **amplia gama de características y tecnologías modernas** para construir una aplicación full-stack robusta. Incluye **patrones de diseño complejos** como la gestión de Server/Client Components, un sistema de autenticación completo, la manipulación de URLs para filtros avanzados, la integración de servicios de terceros (Cloudinary, Google Maps), y el manejo de estados de aplicación complejos (modales de múltiples pasos, estados de carga/error). Además, aborda **problemas comunes de desarrollo** como errores de hidratación y optimización de rendimiento, lo que lo hace adecuado para desarrolladores con un conocimiento intermedio-avanzado de Next.js y ecosistema React.
