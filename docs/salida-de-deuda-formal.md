# Estrategia de dos frentes: salir de la deuda de forma legal y formal

**Borrador — citas verificadas contra fuente oficial el 2026-07-15 (ver `recursos-legales/marco-legal.md`, secciones 7-10). Pendiente revisión final del autor.**

> Este documento une los dos frentes de este proyecto: el **frente defensivo** (qué hacer cuando ya te están cobrando una deuda vieja o de forma abusiva) y el **frente activo** (cómo salir de una deuda vigente, cumpliendo lo pactado, cuando ya no puedes pagarla en los términos originales). No es asesoría legal individual — ver descargo de responsabilidad en `docs/informe-situacion.md`.

## Por qué dos frentes

La mayoría de la gente en Colombia conoce **cero** herramientas legales frente a una deuda. Este proyecto ya cubría el frente defensivo (prescripción, límites a la cobranza). Pero hay un segundo frente igual de importante: **la deuda es válida y está vigente, pero las condiciones ya no son pagables** — para eso la ley colombiana también da caminos formales, no solo "pagar como se pueda" o "que te sigan cobrando de por vida".

```
                    ¿Tu deuda está vigente y es legítima?
                              /              \
                            NO                SÍ
                            |                  |
                    FRENTE DEFENSIVO      FRENTE ACTIVO
                 (prescripción, límites   (usura, modificación,
                  a la cobranza — ya      insolvencia — nuevo
                  cubierto en plantillas   en este documento)
                  01-03)
```

## Frente 1 — Defensivo (ya cubierto en este repositorio)

Ver `docs/informe-situacion.md` y `plantillas/01-03`. Resumen: verificar si la deuda prescribió (5 años acción ejecutiva / 3 años título valor), alegar la prescripción si aplica (no opera sola), y denunciar cobranza que exceda los límites de la Ley 2300/2023.

## Frente 2 — Activo: salir de una deuda vigente cumpliendo lo pactado

### Paso 1 — Comparar tu tasa de interés contra el techo legal (el "medidor de abuso")

La Superintendencia Financiera certifica periódicamente la **tasa de usura** = 1.5 veces el interés bancario corriente, por tipo de crédito. Para julio de 2026 es **28,79% efectivo anual** (cambia cada pocos meses — consultar el histórico en [superfinanciera.gov.co](https://www.superfinanciera.gov.co/publicaciones/10829/sala-de-prensacomunicados-de-prensa-interes-bancario-corriente-10829/) para la tasa vigente **en la fecha en que se pactó tu crédito**).

**Qué hacer:**
1. Ubica en tu contrato o pagaré la **tasa de interés efectiva anual (E.A.)** que te están cobrando.
2. Compárala contra la tasa de usura certificada para el período correspondiente.
3. Si tu tasa supera ese techo, cobrar por encima del límite es el **delito de usura** (Código Penal, art. 305 — prisión de 32 a 90 meses y multa). Documenta todo (contrato, pagaré, comprobantes) y evalúa denunciar ante la Fiscalía, la Policía, o la SIC.

**Esto no es solo defensa — es evidencia de negociación.** Si detectas que el interés cobrado excede o roza el límite legal, tienes una base objetiva y verificable para pedir una modificación de condiciones, no solo "pedir un favor" a la entidad.

### Paso 2 — Pedir la modificación/reestructuración del crédito (gratis por ley)

Si la deuda es legítima, la tasa está dentro de lo legal, pero ya no puedes pagar en los términos originales, tienes derecho a pedir que la entidad **modifique las condiciones según tu capacidad real de pago — sin costo**.

- Si no llevas mora consecutiva mayor a 60-90 días en los últimos 6 meses, la modificación **no cuenta como "reestructuración"** y no debería empeorar tu calificación de forma automática.
- Después de pagar puntual el tiempo requerido (9 meses microcrédito / 1 año consumo / 2 años vivienda o comercial), el crédito sale de "seguimiento especial".

**Qué hacer:** solicita por escrito la modificación de condiciones (puede adaptarse la plantilla `01-derecho-peticion-informacion-deuda.md` para pedir esto en lugar de solo información), indicando tu situación real de ingresos y por qué no puedes seguir pagando en los términos actuales.

### Paso 3 — Si ya debes a varios acreedores y no hay forma de pagar: Insolvencia de Persona Natural No Comerciante

Este es el mecanismo formal más potente que existe en la ley colombiana para "salir rápido y de forma ordenada" de varias deudas a la vez, **negociando con todos tus acreedores en un solo proceso**, no uno por uno.

**¿Aplica para ti?** Debes cumplir con estar en **cesación de pagos**:
- Mora de más de 90 días con **2 o más acreedores**, o
- 2 o más procesos ejecutivos en tu contra, y
- Mora en al menos el 30% de tu pasivo total.

**Qué logra:**
- Al admitirse la solicitud, **se suspenden los embargos y procesos ejecutivos en curso**.
- Se negocia un **plan de pago único**, realista, con todos tus acreedores a la vez, aprobado por la mayoría.
- Tres caminos posibles: negociación de deudas, convalidación de un acuerdo privado ya alcanzado, o liquidación patrimonial si no hay acuerdo.

**Dónde y cómo:**
- Se tramita en **Centros de Arbitraje y Conciliación de las Cámaras de Comercio**, notarías, o ante juez civil municipal según el caso.
- Puedes pedir asesoría gratuita en la **Personería, la Defensoría del Pueblo o un consultorio jurídico universitario** antes de iniciar.
- La solicitud debe explicar las causas de la cesación de pagos (desempleo, enfermedad, etc.) y traer la relación completa de tus deudas y acreedores.
- Dura **60 días hábiles, prorrogables 30 días más**. En centros públicos es gratuito (solo pagas gastos administrativos menores); en centros privados y notarías puede tener costo.

## Cómo se conectan los dos frentes en la práctica

| Tu situación | Qué frente usar |
|---|---|
| La deuda tiene años sin gestión de cobro, posible prescripción | Frente defensivo — `plantillas/01-02` |
| Te cobran fuera de horario, con amenazas, visitas no autorizadas | Frente defensivo — Ley 2300/2023, `plantillas/03` (tutela si falla la SIC) |
| El interés que te cobran parece exagerado | Frente activo, Paso 1 — comparar contra tasa de usura |
| La deuda es legítima pero ya no puedes pagarla en esos términos | Frente activo, Paso 2 — modificación gratuita |
| Debes a varios acreedores, te embargan, no hay forma de organizar los pagos | Frente activo, Paso 3 — Insolvencia de Persona Natural No Comerciante |

## Próximos pasos de este documento (para agregar al repositorio)

- [ ] `plantillas/04-comparador-tasa-usura.md` — checklist paso a paso para comparar tu tasa contra el techo legal.
- [ ] `plantillas/05-guia-insolvencia-persona-natural.md` — guía de requisitos y documentos para iniciar el proceso de insolvencia.
- [ ] Actualizar `plantillas/00-checklist-autoevaluacion.md` para enrutar al frente activo cuando la deuda es legítima pero impagable.
- [ ] Sumar este flujo de dos frentes al `docs/plan-lanzamiento-producto.md` como parte del alcance del futuro calculador (no solo prescripción, también usura y elegibilidad para insolvencia).
