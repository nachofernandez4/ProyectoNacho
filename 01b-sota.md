# 01b · Estado del arte (SOTA) de mi proyecto

> **Plantilla.** En **H1 (26-nov-2026)** se entrega una **versión breve** (2-3 páginas: apartados **1, 2 y 5**), junto al `01-analisis.md`. Los apartados 3, 4, 6, 7 y 8 se completan en **H2 (21-ene-2027)** hasta las **4-6 páginas** del documento final. Este documento estudia qué soluciones, **modelos de negocio** y **herramientas** existen ya para el problema elegido, y justifica las decisiones del proyecto.

> **Nota de elaboración:** Contenido redactado a partir de `00-documentoInicio.md` y de información pública consultada en la web (noviembre 2026). El PDF «Proyecto» indicado por el alumnado no ha podido ser procesado en este entorno; si contiene información adicional, debe incorporarse y revisarse.

## 1. Problema y preguntas de búsqueda (CE 1c)

**Problema:** Las personas que quieren mejorar o controlar su alimentación necesitan calcular su gasto energético, distribuir macronutrientes y planificar dietas acordes a su objetivo, pero hacerlo manualmente o con herramientas genéricas resulta complejo, lento y propenso a errores.

| # | Pregunta | Dónde busqué | Fecha |
|---|---|---|---|
| P1 | ¿Qué aplicaciones y herramientas existen para el seguimiento y la planificación de dietas y macronutrientes? | Google, Google Play, App Store, GitHub, sitios web oficiales de productos | 2026-11-19 |
| P2 | ¿Qué funcionalidades ofrecen (cálculo de calorías/TMB, objetivos de macros, base de datos de alimentos, recetas, planes)? | Sitios web oficiales, páginas de ayuda y fichas de producto | 2026-11-19 |
| P3 | ¿Qué modelos de precio y negocio utilizan (gratuito, freemium, suscripción, publicidad, código abierto)? | Sitios web oficiales y comparativas públicas | 2026-11-19 |
| P4 | ¿Qué alternativas gratuitas, de código abierto y no digitales existen? | GitHub, sitios de proyectos open source, búsqueda general | 2026-11-19 |
| P5 | ¿Qué carencias presentan frente a una planificación sencilla con automatización de la distribución de macros y uso de alimentos/recetas propios según el objetivo del usuario? | Análisis comparativo de funcionalidades públicas | 2026-11-19 |

## 2. Soluciones existentes (CE 1a, 1c, 2a)

Tabla de soluciones que resuelven total o parcialmente el problema. Se incluyen alternativas comerciales, de código abierto y una alternativa no digital.

| Solución | Para quién | Qué hace | Modelo de precio | Enlace y fecha de acceso | Estado |
|---|---|---|---|---|---|
| MyFitnessPal | Público general que quiere registrar alimentación y ejercicio | Registro de comidas, gran base de datos de alimentos, escaneo de códigos de barras, objetivos calóricos y de macros, sincronización con dispositivos | Freemium (plan gratuito con anuncios; suscripción Premium/Premium+) | [https://www.myfitnesspal.com/](https://www.myfitnesspal.com/) (2026-11-19) | leído (web oficial) |
| Cronometer | Usuarios que priorizan precisión nutricional y micronutrientes | Seguimiento de calorías, macros y micronutrientes, base de datos verificada, objetivos y registro diario | Freemium (plan gratuito; suscripción Gold) | [https://cronometer.com/](https://cronometer.com/) (2026-11-19) | leído (web oficial) |
| YAZIO | Usuarios interesados en control de calorías, planes y ayuno (especialmente en Europa) | Contador de calorías y macros, planes de alimentación, recetas, temporizador de ayuno intermitente | Freemium (plan gratuito; suscripción PRO) | [https://www.yazio.com/es](https://www.yazio.com/es) (2026-11-19) | leído (web oficial) |
| FatSecret | Público general que busca un contador amplio sin coste inicial | Diario de alimentos, contador de calorías, información nutricional, recetas y comunidad | Freemium (funciones gratuitas con publicidad; suscripción Premium opcional) | [https://www.fatsecret.es/](https://www.fatsecret.es/) (2026-11-19) | leído (web oficial) |
| Lifesum | Usuarios que buscan mejorar hábitos con planes guiados | Seguimiento de comidas y hábitos, planes de dieta, objetivos nutricionales y recomendaciones | Freemium (plan gratuito; suscripción Premium) | [https://lifesum.com/](https://lifesum.com/) (2026-11-19) | leído (web oficial) |
| MacroFactor | Usuarios avanzados que quieren ajuste dinámico de objetivos según progreso | Registro de macros y peso con ajuste adaptativo del gasto energético estimado y recomendaciones | Suscripción de pago (sin plan gratuito permanente) | [https://macrofactorapp.com/](https://macrofactorapp.com/) (2026-11-19) | leído (web oficial) |
| wger (Workout Manager) | Personas que quieren software libre/autohospedable para nutrición y ejercicio | Gestión de nutrición, planes, registro de peso y entrenamientos; opción de autohospedaje | Gratuito y de código abierto (AGPL), servicio alojado disponible | [https://wger.de/](https://wger.de/) · [https://github.com/wger-project/wger](https://github.com/wger-project/wger) (2026-11-19) | leído (web oficial y repositorio) |
| Hoja de cálculo (Excel/Google Sheets) o planificación en papel | Cualquier persona que planifica su dieta de forma manual | Cálculo manual de calorías y macros con tablas de alimentos, fórmulas y menús semanales | Gratuito / coste de herramientas ofimáticas ya disponibles; no digital en el caso del papel | [https://www.google.com/sheets/about/](https://www.google.com/sheets/about/) · [https://www.microsoft.com/es-es/microsoft-365/excel](https://www.microsoft.com/es-es/microsoft-365/excel) (2026-11-19) | leído (descripción general de la herramienta) |

## 3. Modelos de negocio (CE 1d, 1e)

Patrones observados en las soluciones del apartado 2:

| Patrón | Soluciones que lo usan | Ventaja | Riesgo |
|---|---|---|---|
| Freemium con suscripción | MyFitnessPal, Cronometer, YAZIO, FatSecret, Lifesum | Permite captar muchos usuarios con funciones básicas y monetizar funciones avanzadas | Limitación percibida del plan gratuito; dependencia de conversión a pago |
| Suscripción de pago (premium puro) | MacroFactor | Ingresos recurrentes claros y propuesta especializada | Barrera de entrada para usuarios nuevos; exige alto valor percibido |
| Software libre / servicio gratuito o autohospedado | wger | Transparencia, control de datos y posibilidad de uso sin coste de licencia | Sostenibilidad, mantenimiento y menor financiación para marketing/UX |
| Herramienta manual sin modelo de plataforma | Hojas de cálculo, papel | Coste muy bajo, flexibilidad total y control directo del usuario | Requiere tiempo, conocimientos y es propenso a errores; sin automatización |

**Casos (descripción tipo Business Model Canvas, resumida):**
- **MyFitnessPal (freemium):** propuesta de valor basada en facilidad de registro y gran base de datos; segmentos masivos; canales app/web; ingresos por suscripción y publicidad; recursos clave: base de datos, comunidad y marca.
- **Cronometer (freemium de nicho):** propuesta de valor centrada en precisión y micronutrientes; segmento de usuarios exigentes/profesionales; ingresos por suscripción Gold; recurso clave: calidad y verificación de datos nutricionales.
- **wger (open source):** propuesta de valor de gestión integral y control/autohospedaje; comunidad y contribuidores como recurso; "ingresos" no comerciales directos, sostenido por comunidad/donaciones o uso propio; ventaja en soberanía de datos.

**Modelo de ProyectoNacho:** proyecto académico sin ánimo de lucro en su fase actual. Su valor no es comercial, sino educativo y funcional: ofrecer una herramienta web sencilla que automatice el cálculo de necesidades y la distribución de macros a partir de datos del usuario y sus propios alimentos/recetas, facilitando el aprendizaje de desarrollo full-stack.

## 4. Herramientas y tecnologías (CE 2a, 2b)

Comparación de opciones con los mismos criterios para las decisiones principales. Se marca la opción elegida para el proyecto (propuesta inicial, sujeta a ajuste en diseño/desarrollo).

| Decisión | Opción | Madurez | Licencia | Coste | Curva de aprendizaje | Encaje con el ciclo | Elegida |
|---|---|---|---|---|---|---|---|
| Frontend (interfaz) | React + Tailwind CSS | Alta, ecosistema amplio | MIT / MIT | Bajo (herramientas gratuitas) | Media | Encaja con cliente, diseño de interfaces y componentes | Sí |
| Frontend (interfaz) | JavaScript (Vanilla) + CSS | Muy alta, estándar web | Estándares abiertos | Bajo | Baja-media | Encaja con fundamentos de cliente | No |
| Backend (API/servidor) | Node.js + Express | Alta, muy extendido | MIT | Bajo | Media | Encaja con servidor y desarrollo de APIs; unifica lenguaje con cliente (JS) | Sí |
| Backend (API/servidor) | PHP + Laravel | Alta, muy usado en web | MIT | Bajo | Media | Encaja con servidor; habitual en DAW | No |
| Backend (API/servidor) | Java 21 + Spring Boot | Muy alta, estándar empresarial | Apache 2.0 | Bajo | Media-alta | Muy alineado con tecnologías vistas en ciclo; mayor complejidad inicial para el alcance | No (alternativa valorada) |
| Base de datos | MySQL | Muy alta, ampliamente usada | GPL (edición comunitaria) | Bajo | Baja-media | Muy alineado con contenidos de BD/servidor del ciclo | Sí |
| Base de datos | PostgreSQL | Muy alta, robusta | PostgreSQL License (permisiva) | Bajo | Media | Buena opción técnica; algo menos habitual en prácticas básicas del ciclo | No |
| Despliegue | Render (backend/BD) + Vercel (frontend) | Alta en PaaS modernos | Servicios propietarios con planes gratuitos | Bajo en planes iniciales | Baja-media | Encaja con despliegue de aplicaciones web y CI/CD básico | Sí |
| Despliegue | Railway | Alta, plataforma PaaS | Servicio propietario con plan inicial | Bajo-medio según uso | Baja-media | Adecuado para despliegue rápido | No |

> Nota: la elección prioriza un alcance abordable para el TFG y la integración de los módulos de 2.º (cliente, servidor, diseño y despliegue). Cada decisión relevante se formalizará en `decisiones/` cuando se disponga de la plantilla correspondiente.

## 5. Hueco y diferenciación (CE 1e)

Las soluciones analizadas cubren bien el registro de alimentos y, en muchos casos, ofrecen grandes bases de datos y funciones avanzadas; sin embargo, suelen ser complejas para usuarios que solo quieren planificar su dieta de forma sencilla, presentan funciones clave bajo suscripción o están orientadas al seguimiento diario más que a la construcción guiada de dietas con alimentos y recetas propios. **ProyectoNacho** se diferencia por centrarse en una aplicación web simple que automatiza el cálculo energético (p. ej. mediante fórmulas como Harris-Benedict/Mifflin-St Jeor, a concretar) y la distribución de macronutrientes según el objetivo del usuario (subir, mantener o bajar de peso), permitiendo gestionar sus propios alimentos, recetas y pesos. No pretende competir con plataformas comerciales en volumen de datos, apps móviles nativas o funciones avanzadas, sino ofrecer una herramienta clara, educativa y adaptada a un flujo de planificación básico.

## 6. Decisiones derivadas (CE 1e, 1f, 2b)

- **Tipo de proyecto elegido** (enlaza con el apartado 3 de [`01-analisis.md`](01-analisis.md)): aplicación web de desarrollo a medida para la creación y gestión de dietas personalizadas con cálculo y distribución de calorías y macronutrientes.
- **Requisitos que salen del estudio** (con su ID del apartado 4 de `01-analisis.md`): RF-01 a RF-07 y RNF-01 a RNF-04 (gestión de perfil y objetivo, cálculo energético, definición de macros, gestión de alimentos/recetas, planificación y visualización de totales; seguridad básica, usabilidad responsive y rendimiento razonable). REST-01 a REST-03 recogen restricciones de plazo, uso de datos de prueba e integración de módulos.
- **Decisiones técnicas** (enlace a cada archivo de `decisiones/`): pendiente de crear en la fase correspondiente (frontend, backend, base de datos y despliegue) siguiendo la plantilla de decisiones del repositorio.

## 7. Fuentes y calidad (CE 2a)

| # | Fuente (enlace) | Tipo | Fecha de acceso | Fiabilidad (alta / media / baja) y por qué |
|---|---|---|---|---|
| F1 | [https://www.who.int/news-room/fact-sheets/detail/obesity-and-overweight](https://www.who.int/news-room/fact-sheets/detail/obesity-and-overweight) | Institucional / organismo internacional (OMS) | 2026-11-19 | Alta: fuente oficial con datos sanitarios y metodología institucional |
| F2 | [https://wger.de/](https://wger.de/) y [https://github.com/wger-project/wger](https://github.com/wger-project/wger) | Primaria de producto / repositorio oficial de software libre | 2026-11-19 | Alta para funcionalidades y licencia: información publicada por el propio proyecto |
| F3 | [https://www.myfitnesspal.com/](https://www.myfitnesspal.com/) | Primaria de producto (sitio oficial) | 2026-11-19 | Media-alta para descripción de funciones y planes: fuente oficial, con enfoque comercial |
| F4 | [https://cronometer.com/](https://cronometer.com/) | Primaria de producto (sitio oficial) | 2026-11-19 | Media-alta para descripción de funciones y planes: fuente oficial, con enfoque comercial |
| F5 | [https://www.yazio.com/es](https://www.yazio.com/es) | Primaria de producto (sitio oficial) | 2026-11-19 | Media-alta para descripción de funciones y planes: fuente oficial, con enfoque comercial |
| F6 | [https://www.fatsecret.es/](https://www.fatsecret.es/) | Primaria de producto (sitio oficial) | 2026-11-19 | Media-alta para descripción de funciones y planes: fuente oficial, con enfoque comercial |
| F7 | [https://lifesum.com/](https://lifesum.com/) | Primaria de producto (sitio oficial) | 2026-11-19 | Media-alta para descripción de funciones y planes: fuente oficial, con enfoque comercial |
| F8 | [https://macrofactorapp.com/](https://macrofactorapp.com/) | Primaria de producto (sitio oficial) | 2026-11-19 | Media-alta para descripción de funciones y planes: fuente oficial, con enfoque comercial |
| F9 | [https://www.google.com/sheets/about/](https://www.google.com/sheets/about/) y [https://www.microsoft.com/es-es/microsoft-365/excel](https://www.microsoft.com/es-es/microsoft-365/excel) | Primaria de producto (herramientas ofimáticas) | 2026-11-19 | Alta para descripción general de la herramienta: documentación oficial del proveedor |

## 8. Límites

- No se ha podido consultar el PDF «Proyecto» aportado por el alumnado en este entorno; el contenido se apoya en `00-documentoInicio.md` y fuentes públicas web.
- Los precios, planes concretos y detalles internos de las aplicaciones comerciales pueden cambiar; se han descrito a nivel general según la información pública disponible en la fecha de acceso.
- No se han realizado pruebas de uso exhaustivas (instalación prolongada, mediciones de rendimiento o comparación empírica controlada) de todas las soluciones; la comparación se basa en funcionalidades declaradas públicamente.
- La viabilidad del algoritmo de ajuste automático de macros y selección de alimentos se considera preliminar y deberá validarse en fases de diseño e implementación.
- Las decisiones tecnológicas son una propuesta inicial y pueden revisarse según restricciones del profesorado, del despliegue o del aprendizaje durante el proyecto.

---

## Criterios de evaluación que alimenta este documento (texto literal)

- **1a)** Se han clasificado las empresas del sector por sus características organizativas y el tipo de producto o servicio que ofrecen.
- **1c)** Se han identificado las necesidades más demandadas a las empresas.
- **1d)** Se han valorado las oportunidades de negocio previsibles en el sector.
- **1e)** Se ha identificado el tipo de proyecto requerido para dar respuesta a las demandas previstas.
- **1f)** Se han determinado las características específicas requeridas al proyecto.
- **2a)** Se ha recopilado información relativa a los aspectos que van a ser tratados en el proyecto.
- **2b)** Se ha realizado el estudio de viabilidad técnica del mismo.

> El SOTA **no añade criterios de evaluación**: reúne en un solo sitio lo que 1a-1f y 2a-2b ya piden. La evaluación sigue las listas de cotejo de H1 y H2.
