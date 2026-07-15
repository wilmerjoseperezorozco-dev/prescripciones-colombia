# Fase 0 — Planificación (sin código)

## 1. Problema a resolver

Personas y familias en Colombia (caso base: el propio investigador y sus padres) enfrentan procesos de cobro — judiciales y extrajudiciales — por créditos que:

- Estaban respaldados por un **fondo de garantías** (tipo FNG u otro fondo de garantía de cartera).
- El fondo garante ya pagó el siniestro (la pérdida) a la entidad financiera original tras el incumplimiento.
- La cartera queda luego en manos de un tercero (firma de cobranza, cesionario o el propio fondo subrogado) que continúa cobrando al deudor, en algunos casos con **prescripción ya cumplida** o con prácticas de cobranza que exceden los límites legales (amenazas, intimidación, presión psicológica).

La población más afectada es la que **no conoce sus derechos**: no sabe que una deuda puede prescribir, no sabe que existen límites legales a la cobranza extrajudicial, y no sabe cómo defenderse en un proceso ejecutivo.

## 2. Población afectada (hipótesis a validar con datos públicos)

- Deudores de microcrédito, libranza, crédito de consumo y tarjeta de crédito en municipios con bajo acceso a asesoría jurídica (foco inicial: Atlántico / Barranquilla y área metropolitana, luego escalable a nivel nacional). **Confirmado por experiencia del autor: el patrón se repite en distintas entidades y distintos tipos de crédito — no es un caso aislado de un solo producto financiero.**
- Adultos mayores (pensionados con libranza) — grupo con alta exposición a cobranza agresiva según reportes de la SIC.
- Personas con deudas de más de 3-5 años en mora que desconocen la figura de la prescripción, y que en general **no saben qué es un derecho de petición ni una tutela** — esta ignorancia básica del mecanismo de defensa es, según la experiencia del autor, la barrera más grande, más que el desconocimiento de la ley en sí.

## 3. Impacto esperado

- Reducción de pagos indebidos por deudas ya prescritas.
- Disminución de reportes negativos indebidos en centrales de riesgo (más allá del plazo legal de permanencia).
- Empoderamiento para presentar excepciones de prescripción en procesos ejecutivos.
- Visibilización pública (informe) del patrón: fondo de garantías paga → cartera se cede/gestiona → cobranza persiste sin informar al deudor sus derechos.

## 4. Riesgos y precauciones (por qué esto se hace con cuidado)

| Riesgo | Mitigación |
|---|---|
| Afirmar datos legales incorrectos en un documento público | Toda cifra/plazo debe citar norma exacta, verificada en fuente oficial antes de publicar |
| Nombrar entidades específicas sin evidencia sólida → riesgo de difamación | V1 del informe es genérica/educativa, sin nombrar entidades; casos reales solo se documentan anonimizados |
| Dar "asesoría legal" que sustituya a un abogado | El repo aclara que es educativo, remite a consultorios jurídicos/Defensoría del Pueblo para casos puntuales |
| Generalizar de 1-2 casos personales a "todo el sistema" | El informe distingue explícitamente entre patrón general (con fuente) y experiencia personal (marcada como tal) |
| Publicar antes de revisión | Nada se publica a GitHub hasta que el usuario lo revise y apruebe explícitamente |

## 5. Marco de "por qué no se baja la deuda" (a desarrollar en el informe)

Hipótesis a verificar y explicar con norma:
1. Intereses moratorios y capitalización pueden hacer que el saldo crezca más rápido de lo que se abona si los pagos son parciales o tardíos.
2. Cuando el fondo de garantías paga el siniestro al banco, el banco ya recuperó su pérdida — pero el deudor sigue debiendo el saldo, ahora a quien tenga la cartera (el fondo subrogado o quien la compró/gestiona).
3. La cartera castigada muchas veces se vende con descuento a firmas de cobranza, que buscan recuperar el 100% del valor nominal (no lo que pagaron por ella), generando presión para cobrar el máximo posible antes de que prescriba.
4. Mientras no haya excepción de prescripción alegada formalmente (no opera de oficio en materia civil/comercial en muchos casos), la deuda sigue siendo exigible aunque hayan pasado los años.

**Nota:** el punto 4 es la razón técnica central de por qué "no se cae la deuda sola" — la prescripción debe alegarse, no ocurre automáticamente. Este es el mensaje educativo más importante del proyecto.

## 6. Entregables de Fase 0

- [x] Estructura de carpetas del repositorio.
- [x] Este plan de fases.
- [x] `recursos-legales/marco-legal.md` con normas citadas, verificado contra fuente oficial (Fase 3, 2026-07-15).
- [x] `docs/informe-situacion.md` — informe público, v0.3.
- [x] Definición de licencia y política de contribución.

## 7. Fases siguientes (resumen)

- **Fase 1 — Infraestructura (hecha):**
  - [x] `plantillas/00-checklist-autoevaluacion.md` — guía de qué plantilla usar según la situación del deudor.
  - [x] `plantillas/01-derecho-peticion-informacion-deuda.md` — mecanismo priorizado según la experiencia real del autor (funcionó antes de que hubiera demanda).
  - [x] `plantillas/02-excepcion-prescripcion.md` — para cuando ya hay proceso judicial notificado (con advertencia de plazos cortos).
  - [x] `plantillas/03-tutela-habeas-data.md` — alternativa cuando el derecho de petición no se responde o el portal de la SIC falla (barrera práctica real reportada por el autor).
  - [x] Repo público en GitHub: https://github.com/wilmerjoseperezorozco-dev/prescripciones-colombia
  - [x] Licencia definida: CC BY-SA 4.0 (contenido), MIT (software futuro) — ver `LICENSE.md`.
- **Fase 2 — Estados vacíos / casos piloto (hecha):**
  - [x] `casos-anonimizados/00-plantilla-caso-vacia.md` — plantilla para que cualquier lector documente su propio caso.
  - [x] `casos-anonimizados/caso-001.md` — caso del investigador, anonimizado (sin fechas/montos/entidad exactos, solo el patrón: 3-5 años de mora, derecho de petición antes de demanda, obstáculo con el portal SIC).
  - [ ] Sumar 1-2 casos adicionales de otros tipos de crédito cuando estén disponibles.
- **Fase 3 — Preentrega (hecha, 2026-07-15):**
  - [x] Verificadas todas las citas legales contra fuente oficial (Función Pública, Superfinanciera, SUIN-Juriscol, fng.gov.co, CISA).
  - [x] Corrección importante: se retiró la referencia a la Circular Externa 026/2019 SFC (no trataba de cobranza) — la Ley 2300/2023 quedó como norma central de cobranza.
  - [x] Confirmado el alcance real de la cesión FNG→CISA: limitado al programa "Unidos por Colombia" (Decreto 264/2024), no generalizable a todos los programas de garantía — corregido en el informe.
  - [x] Confirmado texto literal de arts. 2539-2540 del Código Civil (interrupción de la prescripción).
  - [ ] Único punto que queda intrínsecamente abierto (no por falta de verificación, sino porque cambia con el tiempo): reconfirmar el estado del portal de la SIC justo antes de publicar la web app.
- **Fase 3.5 — Frente activo (hecha, 2026-07-15):** ampliación del alcance del proyecto de "solo defensa" a "defensa + salida activa de deuda", pedida explícitamente por el autor ("atacar los dos frentes").
  - [x] `recursos-legales/marco-legal.md`, secciones 7-10: tasa de usura y delito de usura (Código Penal art. 305), Insolvencia de Persona Natural No Comerciante (CGP Título IV, Ley 2445/2025), derecho a modificación/reestructuración gratuita de crédito, puntaje/score Datacrédito — todo verificado contra fuente oficial.
  - [x] `docs/salida-de-deuda-formal.md` — documento central que conecta frente defensivo + frente activo con árbol de decisión.
  - [x] `plantillas/04-comparador-tasa-usura.md` — checklist para comparar la tasa del usuario contra el techo legal certificado.
  - [x] `plantillas/05-guia-insolvencia-persona-natural.md` — guía de requisitos, documentos y dónde tramitar la insolvencia.
  - [x] `plantillas/00-checklist-autoevaluacion.md` actualizado para enrutar entre ambos frentes.
- **Fase 4 — Iteración**: canal de retroalimentación, posible alianza con consultorios jurídicos universitarios (ver referencia CUC ya usada en LegalTech Avatares), revisión legal externa antes de construir la web app.
- **Fase 5+ — Producto**: ver `docs/plan-lanzamiento-producto.md` para el plan de web app (PWA); el alcance del futuro calculador debe ampliarse para cubrir también el frente activo (usura, elegibilidad de insolvencia), no solo prescripción.
