# 00 · Documento de inicio del proyecto

> **Plantilla.** Se rellena durante el **ciclo 1 (16-19 nov)** y el tutor la revisa el jueves 19. Es breve: una página. Si algo no lo sabes todavía, escribe «pendiente» y por qué. Borra las notas en cursiva al rellenar.
>
> **No escribas datos personales sensibles** (teléfono, dirección, DNI) ni tu correo personal. Tu repositorio es público.

## 1. Datos del alumno/a

| | |
|---|---|
| **Nombre** (real o alias, como prefieras) | Nacho Fernández Álvarez |
| **Usuario de GitHub** | nachofernandez4 |
| **Repositorio del proyecto** | Pendiente (se creará y enlazará tras la aprobación inicial del tutor) |
| **Ciclo y curso** | DAW, 2.º · curso 2026-27 |
| **Fecha** | 2026-11-17 |

## 2. Nombre del proyecto

**MacroTrack** (nombre provisional). Aplicación web para el cálculo personalizado de macronutrientes y el registro diario de alimentación según el objetivo físico de cada usuario.

## 3. Qué quiero hacer

Quiero desarrollar una aplicación web intuitiva que permita a cualquier persona gestionar su alimentación diaria de forma sencilla y visual. Al registrarse, el usuario introducirá sus datos físicos básicos (edad, sexo, altura, peso actual y nivel de actividad física) junto con su objetivo principal: pérdida de grasa (déficit calórico), mantenimiento o ganancia de masa muscular (superávit calórico).

A partir de estos parámetros, la aplicación calculará automáticamente su gasto energético diario y repartirá las calorías en objetivos concretos de proteínas, hidratos de carbono y grasas. En el uso diario, el usuario podrá ir añadiendo los alimentos consumidos en cada comida (desayuno, comida, cena y snacks) desde una base de datos interna o creando sus propios alimentos, visualizando mediante barras de progreso cuánto le falta o cuánto ha consumido respecto a su meta del día.

## 4. Qué problema o necesidad resuelve

Muchas personas que quieren mejorar su composición corporal abandonan el control nutricional porque las aplicaciones comerciales actuales resultan excesivamente complejas, están saturadas de funciones sociales innecesarias o bloquean el reparto personalizado de macronutrientes tras suscripciones de pago.

Esta necesidad la he observado tanto por experiencia propia en el entorno del entrenamiento y el gimnasio como hablando con compañeros que intentan seguir una pauta nutricional sin ser expertos. Existe una demanda clara de herramientas directas, limpias y gratuitas que vayan al grano: saber qué necesitas comer hoy y registrar de forma rápida si lo estás cumpliendo.

## 5. Para quién

Está dirigida principalmente a **usuarios particulares** (deportistas amateur, personas que acuden al gimnasio o cualquier persona interesada en mejorar sus hábitos alimenticios) que buscan controlar su ingesta calórica y de macronutrientes de manera autónoma, sin necesidad de conocimientos avanzados de nutrición.

## 6. Funcionalidades principales

| # | Funcionalidad | ¿Imprescindible? (sí / no) |
|---|---|---|
| 1 | Registro e inicio de sesión de usuarios con perfil físico y selección de objetivo (definición, mantenimiento o volumen). | sí |
| 2 | Cálculo automático de calorías diarias objetivo y reparto de macronutrientes (proteínas, carbohidratos y grasas). | sí |
| 3 | Buscador de alimentos precargados y formulario para dar de alta alimentos personalizados (por cada 100 g). | sí |
| 4 | Diario de comidas por fecha con barras de progreso en tiempo real hacia el objetivo diario. | sí |
| 5 | Registro histórico de peso corporal con gráfica básica de evolución semanal/mensual. | no |
| 6 | Creación de recetas o comidas compuestas reutilizables a partir de varios ingredientes. | no |

## 7. Tecnologías previstas

| Tecnología | Para qué | Nivel actual (nada / algo / bien) |
|---|---|---|
| HTML5 / CSS3 (Tailwind CSS) | Maquetación y diseño responsivo de la interfaz | bien |
| JavaScript / React | Desarrollo del frontend interactivo y gestión de estado | algo |
| Node.js + Express (o PHP / Laravel) | API REST en el servidor y lógica de cálculo nutricional | algo |
| MySQL / MariaDB | Almacenamiento relacional de usuarios, alimentos y registros diarios | bien |
| Git y GitHub | Control de versiones y alojamiento del código fuente | bien |
| Docker / Render (o Vercel + Railway) | Despliegue en producción de la aplicación y la base de datos | nada |

## 8. Dónde se integra con los módulos de 2.º

- [x] Desarrollo web en entorno cliente (0612)
- [x] Desarrollo web en entorno servidor (0613)
- [x] Despliegue de aplicaciones web (0614)
- [x] Diseño de interfaces web (0615)

## 9. Datos y empresas

- ¿El proyecto parte de una **empresa** (por ejemplo, de tus prácticas)? **No**. Se plantea como un encargo simulado / proyecto propio.
- ¿Usará **datos personales reales**? **No**: durante el desarrollo y las pruebas se emplearán exclusivamente usuarios ficticios y datos de ejemplo generados para la demostración.

## 10. Riesgos y dudas iniciales

- **Alcance de la base de datos de alimentos:** Recopilar demasiados alimentos puede consumir mucho tiempo; lo acotaré cargando inicialmente un catálogo base de unos 80-100 alimentos comunes mediante *seeders* y permitiendo al usuario crear los suyos propios.
- **Despliegue full-stack:** Es la parte con la que tengo menos experiencia práctica, por lo que tendré que investigar con antelación cómo conectar correctamente el frontend, la API y la base de datos en un entorno gratuito en la nube.
- **Gestión del tiempo:** Compaginar el desarrollo del proyecto con las entregas habituales de los módulos del segundo trimestre para llegar sin agobios a la versión mínima del 31 de marzo.

## 11. Qué espero aprender

Espero consolidar la comunicación completa entre un frontend moderno y una API REST propia, ganando soltura en la arquitectura real de una aplicación web de principio a fin. Además, quiero perderle el miedo al despliegue en producción y aplicar buenas prácticas de diseño de interfaces centradas en la usabilidad.

---

## Aprobación del tutor

| Criterio mínimo | Cumple |
|---|---|
| Necesidad real y documentada | ☐ |
| Alcance abordable en el tiempo disponible | ☐ |
| Integra contenidos de al menos tres módulos de 2.º | ☐ |
| No usa datos personales reales | ☐ |

**Estado:** ☐ Aprobada · ☐ Aprobada con cambios · ☐ Necesita rehacerse

**Fecha:** 

**Comentarios del tutor:**