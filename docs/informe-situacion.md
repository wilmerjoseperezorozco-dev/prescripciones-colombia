# El ciclo silencioso de la cobranza en Colombia: qué pasa después de que el fondo de garantías ya cobró

**Borrador v0.2 — citas legales verificadas contra fuente oficial el 2026-07-15 (ver detalle en `recursos-legales/marco-legal.md`); quedan 4 puntos menores por cerrar antes de publicar. Pendiente revisión final del autor.**

> Este documento es un informe educativo elaborado por investigadores ciudadanos, no un despacho de abogados. Cada afirmación legal está respaldada por la norma citada en [`recursos-legales/marco-legal.md`](../recursos-legales/marco-legal.md).

## 1. La situación en una frase

Miles de colombianos siguen pagando, o siendo demandados y amenazados por, deudas donde **la entidad financiera original ya recuperó su pérdida** gracias a un fondo de garantías — y aun así el cobro continúa, muchas veces años después, sobre personas que no saben que tienen derechos para defenderse.

## 2. ¿Cómo funciona el ciclo? (explicado sin tecnicismos)

1. Una persona toma un crédito (libranza, microcrédito, crédito de consumo, tarjeta) respaldado por un **fondo de garantías** (el más conocido a nivel nacional es el Fondo Nacional de Garantías — FNG).
2. Si la persona incumple, la entidad financiera reclama al fondo el pago de la parte garantizada — el fondo no garantiza el 100% del crédito, sino un porcentaje. [Verificado — reglamento operativo FNG]
3. El fondo paga ese siniestro a la entidad — **no** al deudor, ni cancela la deuda del deudor. El fondo **se subroga**: por ley, adquiere el derecho de cobrar al deudor lo que pagó. [Verificado — reglamento operativo FNG, figura de pago con subrogación]
4. A partir de ahí, la cartera puede quedar en manos del propio fondo, o ser cedida a un tercero de gestión de activos. **Dato encontrado en esta investigación**: al menos en el programa especial "Unidos por Colombia", el FNG puede ceder la cartera pagada por garantías, sin costo, a CISA (Central de Inversiones S.A., entidad estatal de gestión de activos) — *este hallazgo está pendiente de confirmar si aplica a otros programas de garantía además de ese*.
5. Empieza (o continúa) el cobro al deudor — por años, en algunos casos con llamadas, visitas, o procesos judiciales — **sin que a la persona se le explique con claridad** en qué momento empezó a deberle a un tercero distinto del banco original, ni que existen plazos legales que pueden jugar a su favor.

## 3. "¿Por qué la deuda no baja aunque yo pague?"

Esta es la pregunta que más golpea a las familias afectadas. Las razones, ya verificadas contra norma:

- **Los intereses moratorios siguen corriendo** sobre el saldo mientras la deuda esté en mora, y pueden crecer más rápido que los abonos parciales.
- **Quien cobra ahora no es quien te prestó.** Si la cartera fue cedida o el fondo se subrogó, cada pago puede estarse aplicando bajo condiciones distintas a las del crédito original, y esto no siempre se comunica con claridad.
- **La deuda no desaparece sola con el tiempo, aunque legalmente sí deja de ser exigible.** La **prescripción de la acción ejecutiva es de 5 años**, y si nadie actúa, se transforma en acción ordinaria por 5 años más — 10 años en total desde el origen (Código Civil, art. 2536, modificado por la Ley 791 de 2002). Si la deuda está documentada en un pagaré o letra, la acción cambiaria directa prescribe en solo **3 años** desde el vencimiento (Código de Comercio, art. 789). Pero — y esto es clave — **la prescripción no opera automáticamente**: la ley dice textualmente que *"el que quiera aprovecharse de la prescripción debe alegarla; el juez no puede declararla de oficio"* (Código Civil, art. 2513). Si nadie la alega, el proceso sigue como si la deuda estuviera vigente, aunque legalmente ya no lo esté.

**Este último punto es el corazón del problema**: la ley sí protege al deudor con el paso del tiempo, pero esa protección es "silenciosa" — no actúa por sí sola. Si la persona no sabe que existe, o no tiene cómo alegarla, sigue pagando o siendo perseguida por una deuda que un juez, si se lo pidieran, probablemente declararía prescrita.

## 4. El patrón de monopolio sobre la población vulnerable

No es que exista necesariamente una sola empresa controlando todo el mercado — el patrón es otro tipo de "monopolio": **el monopolio de la información**.

- Las entidades que cobran conocen exactamente los plazos de prescripción, las reglas de reporte a centrales de riesgo y los límites legales a la cobranza.
- La persona deudora, en especial en zonas con poco acceso a asesoría jurídica gratuita, generalmente no los conoce.
- Esa asimetría de información es la que permite que, dentro de un marco que en el papel es legal, se ejerza presión (llamadas insistentes, visitas, amenazas de embargo, mensajes intimidantes) sobre personas que — si conocieran sus derechos — podrían responder, negociar o incluso hacer declarar prescrita la obligación.

Este proyecto no busca acusar a una entidad puntual sin pruebas — busca **cerrar esa asimetría de información** para que la persona vulnerable llegue a la misma mesa con el mismo conocimiento que quien la está cobrando.

## 5. A quién está dirigido este informe

- Personas con deudas de varios años en mora que no saben si aún son exigibles.
- Adultos mayores con libranza, grupo con exposición reconocida a la cobranza intensiva — motivo por el cual la Ley 2300 de 2023 exige autorización expresa y previa del consumidor incluso para el canal de contacto usado en microcrédito, y prohíbe las visitas domiciliarias salvo autorización expresa.
- Familias en municipios con poco o nulo acceso a un abogado.

## 6. Qué puede hacer una persona en esta situación

Plantillas completas y listas para adaptar en [`plantillas/`](../plantillas):

1. **Pedir por escrito** (derecho de petición, [`plantillas/01-derecho-peticion-informacion-deuda.md`](../plantillas/01-derecho-peticion-informacion-deuda.md)) a quien está cobrando: quién es el actual titular de la deuda, desde cuándo, y el historial completo de pagos. **Este fue el mecanismo que en la práctica funcionó primero**, antes de que hubiera un proceso judicial.
2. Verificar la fecha de la última gestión de cobro o pago, para calcular si el término de prescripción ya se cumplió (5 años acción ejecutiva / 3 años título valor / 10 años acción ordinaria — art. 2536 Código Civil y art. 789 Código de Comercio).
3. Si es demandado, **alegar la excepción de prescripción** dentro del proceso ([`plantillas/02-excepcion-prescripcion.md`](../plantillas/02-excepcion-prescripcion.md)) — no ignorar la demanda esperando que "se venza sola". **Los plazos judiciales son cortos: buscar apoyo de un consultorio jurídico o abogado de inmediato.**
4. Verificar y, si aplica, reclamar la actualización o retiro del reporte en centrales de riesgo una vez la obligación esté extinta o superado el plazo de permanencia (máximo 4 años tras el pago, o el doble del tiempo de mora si esta fue menor a 2 años — Ley 1266 de 2008, art. 13).
5. Denunciar prácticas de cobranza que excedan lo permitido por la Ley 2300 de 2023 (contacto fuera de horario, más de un canal por semana, visitas no autorizadas, contacto con referencias) ante la SIC o la SFC. **Advertencia práctica**: el portal de reclamaciones de la SIC ha fallado de forma reiterada según la experiencia de este proyecto — si eso ocurre, la alternativa es la acción de tutela ([`plantillas/03-tutela-habeas-data.md`](../plantillas/03-tutela-habeas-data.md)), que se presenta directamente ante cualquier juzgado, sin costo y sin necesidad de abogado.

## 7. Lo que este informe NO es

- No es asesoría legal para un caso puntual — cada situación tiene detalles (tipo de crédito, si ya hubo sentencia, si hubo algún pago reciente) que cambian el análisis.
- No acusa a ninguna entidad financiera, fondo o firma de cobranza específica de actuar ilegalmente sin evidencia documental verificada.
- No sustituye a un consultorio jurídico universitario, la Defensoría del Pueblo, o un abogado.

## 8. Próximos pasos de este proyecto

- [x] Verificar las citas legales principales contra fuente oficial (ver `recursos-legales/marco-legal.md`).
- [x] Publicar plantillas de derecho de petición, excepción de prescripción y tutela (Fase 1).
- [ ] Cerrar 4 puntos legales menores pendientes (arts. 2539-2540 CC, circular SFC de cobranza, alcance de la cesión de cartera FNG→CISA, estado del portal SIC).
- [ ] Documentar 2-3 casos anonimizados que ilustren el patrón paso a paso, cubriendo distintos tipos de crédito (Fase 2).
- [ ] Publicar el repositorio y este informe públicamente, bajo licencia abierta, tras revisión final del autor.

---

*Elaborado por investigadores ciudadanos independientes en Barranquilla, Atlántico, Colombia. Proyecto sin fines de lucro orientado a la alfabetización legal y financiera de la población vulnerable.*
