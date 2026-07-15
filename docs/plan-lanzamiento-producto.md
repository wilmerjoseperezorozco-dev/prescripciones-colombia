# Plan de lanzamiento — de repositorio educativo a producto (web app / PWA)

**Estado: planificación (Fase 0.5 / puente a Fase 3+). Ningún desarrollo de software ha comenzado — este es el plan antes de escribir la primera línea de código de producto.**

## 1. Decisión de plataforma: Web App (PWA), no app nativa — por qué

| Criterio | Web App / PWA | App nativa (Play Store / App Store) |
|---|---|---|
| Fricción de acceso | Cero — se abre por link (WhatsApp, SMS, Google) | Requiere descarga, espacio, cuenta en la tienda |
| Costo y velocidad de desarrollo | Un solo código para todos los dispositivos | Doble esfuerzo (Android + iOS) o framework híbrido |
| Público objetivo (adultos mayores, pensionados, zonas con bajo acceso) | Funciona en celulares gama baja, sin actualizar apps | Muchos usuarios evitan instalar apps desconocidas por miedo a fraude — problema real dado que este mismo proyecto ya trabaja el tema de estafas ([[project_escudo_anti_estafas]]) | 
| Indexable en buscadores | Sí — alguien puede buscar "mi deuda ya prescribió" en Google y llegar directo | No — las apps no se indexan en Google de la misma forma |
| Notificaciones | Notificaciones push web (limitadas en iOS, pero mejorando) | Push nativo completo |
| Costo de mantenimiento y revisión de tiendas | Ninguno | Revisiones de Google/Apple, políticas cambiantes, riesgo de rechazo por ser contenido "legal/financiero sensible" |

**Decisión: Web App con capacidades PWA (instalable "como app" desde el navegador, funciona offline para contenido estático como plantillas ya descargadas).** Si en 12-18 meses hay tracción real y necesidad clara de funciones solo-nativas (notificaciones push agresivas, cámara para escanear documentos, etc.), se evalúa entonces una app nativa o híbrida (React Native/Expo — ya usado en [[project_structai_mobile_fase0]]) sobre la misma base de negocio.

## 2. Qué hace este producto (alcance del MVP)

**No es** un generador automático de demandas ni un despacho de abogados online. **Sí es**:

1. Un **calculador de prescripción**: el usuario responde preguntas simples (tipo de crédito, fecha de última gestión de cobro, si hubo pagos) y la herramienta indica si, según los plazos legales, la deuda **probablemente** ya prescribió — con lenguaje de probabilidad, nunca de certeza, y siempre remitiendo a verificación humana antes de actuar.
2. Un **generador de cartas** (derecho de petición, y con mucha más advertencia, la estructura de excepción de prescripción y de tutela) que rellena la plantilla ya existente en `plantillas/` con los datos que el usuario ingresa.
3. Una **biblioteca educativa** (el contenido de `docs/` y `recursos-legales/` ya escrito, con buscador simple).
4. Un **directorio de ayuda real**: consultorios jurídicos universitarios, Defensoría del Pueblo, dónde denunciar cobranza abusiva — con datos de contacto verificados.

**Explícitamente fuera del MVP**: pagos, cuentas de usuario con historial persistente de casos, IA generativa sin supervisión que redacte documentos legales sin plantilla base, cualquier función que se pueda interpretar como "representación legal".

## 3. Regulaciones que aplican al construir esto como producto activo (no solo como repositorio de texto)

Un repositorio de Markdown no recolecta datos de nadie. Una web app que pide "fecha de tu deuda, tipo de crédito" sí. Esto activa obligaciones que el repositorio actual no tenía:

| Obligación | Norma | Qué implica para el producto |
|---|---|---|
| Protección de datos personales | Ley 1581 de 2012 y Decreto 1377 de 2013 (régimen general de protección de datos) | Se necesita: (1) Política de Tratamiento de Datos Personales publicada, (2) autorización expresa del usuario antes de capturar cualquier dato, (3) definir si los datos se almacenan o se procesan solo en el navegador del usuario (opción más simple y más segura: **procesar todo en el cliente, sin guardar nada en servidor**, para el calculador de prescripción) |
| Registro Nacional de Bases de Datos (RNBD) | Ley 1581/2012, reglamentado por la SIC | Solo aplica si el producto **almacena** datos personales de usuarios en una base de datos propia. Si el MVP no guarda historiales (ver arriba), esta obligación se evita en la primera versión |
| Ejercicio no autorizado de la profesión de abogado | Estatuto del Abogado (Decreto Ley 196 de 1971) y jurisprudencia relacionada — **verificar con detalle antes de lanzar, es el riesgo legal más sensible del proyecto** | El producto debe quedar claramente del lado de "información y plantillas genéricas", nunca "representación" o "asesoría personalizada". Cada pantalla que genere un documento debe repetir el descargo de responsabilidad. Si el proyecto crece, la alianza con un consultorio jurídico universitario (ver `00-fase0-planificacion/plan-fases.md`, Fase 4) da respaldo institucional real a esta línea |
| Accesibilidad web | Resolución 1519 de 2020 (MinTIC) — estándares de accesibilidad para sitios del Estado, buena práctica igual para un sitio dirigido a población vulnerable aunque no sea obligatorio para un proyecto privado | Contraste de color alto, tipografía grande por defecto, compatible con lectores de pantalla — dado que parte del público son adultos mayores |
| Términos de uso y descargo de responsabilidad | No hay una ley única — se redacta como contrato de adhesión, revisable por abogado antes de publicar | Debe decir explícitamente: no hay relación abogado-cliente, no se garantiza resultado, cada caso requiere verificación individual |

**Ninguna de estas obligaciones debe tomarse como cerrada con este documento** — antes de lanzar, la política de datos y los términos de uso deben pasar por revisión de un abogado (ideal: a través de la alianza con consultorio jurídico universitario ya contemplada en el roadmap).

## 4. Qué automatizar y qué NO automatizar

| Automatizar (bajo riesgo, alto valor) | NO automatizar todavía (alto riesgo) |
|---|---|
| Cálculo de fechas de prescripción según reglas ya verificadas en `marco-legal.md` | Generación de documentos legales por IA generativa sin plantilla fija y sin revisión |
| Rellenar plantillas existentes con los datos que el usuario escribe | Envío automático de la carta/tutela en nombre del usuario sin que él la revise y confirme |
| Recordatorios genéricos ("faltan X días para cumplir el plazo que calculaste") | Decisiones de "sí, tu deuda prescribió" presentadas como certeza legal — siempre en términos de probabilidad y con remisión a revisión humana |
| Checklist interactivo (versión web del `plantillas/00-checklist-autoevaluacion.md`) | Cualquier función de pago o cobro a los usuarios en la primera versión — mantenerlo gratuito refuerza la confianza y evita regulación adicional de comercio electrónico |

## 5. Roadmap de producto (continúa la numeración de fases del proyecto)

- **Fase 3 (actual, en curso):** cerrar los 4 puntos legales pendientes de `marco-legal.md`; revisar lenguaje claro de todo el contenido existente.
- **Fase 4:** publicación pública del repositorio como referencia de contenido (ya hecho — repo en GitHub); búsqueda de alianza con consultorio jurídico universitario para respaldo institucional y revisión legal de términos de uso.
- **Fase 5 — MVP de producto (web app / PWA):**
  - Sitio estático o ligero que muestre el contenido de `docs/` y `recursos-legales/` con buscador.
  - Calculador de prescripción (todo el cálculo en el navegador del usuario, sin guardar datos en servidor).
  - Generador de las 3 cartas de `plantillas/` a partir de un formulario simple, con descarga en PDF/Word.
  - Política de datos + términos de uso revisados por abogado antes de publicar el MVP.
- **Fase 6 — Iteración con usuarios reales:** feedback de los primeros usuarios (posiblemente a través del consultorio jurídico aliado), métricas de uso anónimas y agregadas (no historiales individuales), ajustes de contenido.
- **Fase 7 (opcional, solo si hay tracción):** evaluar app nativa/híbrida, integración WhatsApp, o expansión a otros temas de alfabetización legal financiera.

## 6. Stack técnico recomendado (consistente con proyectos previos del autor)

- **Frontend:** Next.js (React) como PWA — permite empezar 100% estático (el contenido ya existe en Markdown) y añadir el calculador/generador de cartas como componentes interactivos sin backend propio.
- **Sin base de datos en el MVP** si el cálculo y el llenado de plantillas ocurre en el navegador — esto simplifica drásticamente la carga regulatoria (ver sección 3) y el costo de infraestructura.
- **Si más adelante se necesita backend** (por ejemplo, para guardar contacto de consultorios jurídicos actualizado, o analítica agregada): Supabase, consistente con el patrón ya usado en otros proyectos del autor (ver `feedback_plantilla_estructura_carpetas` en memoria).
- **Hosting:** Vercel o similar — despliegue directo desde este mismo repositorio de GitHub.

## 7. Cómo medir si esto está funcionando (impacto, no solo tráfico)

- Descargas/generaciones de cartas (conteo agregado, sin datos personales).
- Testimonios voluntarios de casos resueltos (con consentimiento explícito, anonimizados igual que `casos-anonimizados/caso-001.md`).
- Alianzas activas con consultorios jurídicos (número de derivaciones).
- Cobertura de tipos de crédito documentados en `casos-anonimizados/` (para verificar que el patrón sigue siendo transversal, no solo el caso original).

## 8. Riesgo central a vigilar

El mayor riesgo de este proyecto **no es técnico, es regulatorio/reputacional**: la línea entre "herramienta educativa con plantillas" y "ejercicio no autorizado de la abogacía" debe mantenerse clara en cada pantalla del producto. Esto debe revisarse con un abogado real antes de la Fase 5 (MVP de producto), no después.
