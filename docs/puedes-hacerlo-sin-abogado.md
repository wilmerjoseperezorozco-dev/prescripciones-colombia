# De entender la ley a ejecutar el proceso: lo que puedes hacer sin abogado, hoy

**Borrador — citas verificadas contra fuente oficial el 2026-07-19 (ver `recursos-legales/marco-legal.md`, sección 11). Pendiente revisión final del autor.**

> Este es el documento puente del proyecto: no basta con saber que la ley te protege — hay que saber que **puedes ejecutar el trámite tú mismo, sin que el costo de un abogado sea la barrera**. La razón más común por la que un colombiano no usa estas herramientas no es que no existan: es que cree, equivocadamente, que necesita pagar un abogado para empezar. Eso no es cierto en la mayoría de los casos que cubre este proyecto.

## La regla general

En Colombia, el "derecho de postulación" (la obligación de actuar a través de abogado) tiene excepciones amplias, pensadas justamente para que la justicia sea accesible a quien no puede pagar representación legal. Cinco de esas excepciones son el corazón de este proyecto.

## Tabla de acción inmediata

| Mecanismo | ¿Necesitas abogado? | Umbral / condición | Plantilla lista |
|---|---|---|---|
| **Acción de tutela** | **No.** Puede presentarse sin ninguna formalidad, incluso verbalmente en casos urgentes (Decreto 2591/1991, art. 14) | Cuando se vulnera un derecho fundamental (petición, hábeas data, etc.) | [`plantillas/03-tutela-habeas-data.md`](../plantillas/03-tutela-habeas-data.md) |
| **Derecho de petición** | **No.** Nunca ha requerido abogado (Constitución, art. 23) | Cualquier solicitud de información a una entidad | [`plantillas/01-derecho-peticion-informacion-deuda.md`](../plantillas/01-derecho-peticion-informacion-deuda.md) |
| **Conciliación** en centro autorizado | **No** para solicitarla ni asistir (el conciliador sí debe ser abogado, tú no) | Cualquier conflicto conciliable — gratis en consultorios jurídicos universitarios y entidades públicas | Guía en `docs/salida-de-deuda-formal.md`, y como paso previo en [`plantillas/06`](../plantillas/06-demanda-sin-abogado-minima-cuantia.md) |
| **Proceso civil de mínima cuantía** (ej. excepción de prescripción, cobro de una deuda a tu favor) | **No**, puedes litigar en causa propia (Decreto 196/1971) | Pretensión menor a **40 SMLMV** | [`plantillas/02-excepcion-prescripcion.md`](../plantillas/02-excepcion-prescripcion.md), [`plantillas/06-demanda-sin-abogado-minima-cuantia.md`](../plantillas/06-demanda-sin-abogado-minima-cuantia.md) |
| **Demanda laboral de única instancia** | **No**, puede presentarse incluso verbalmente | Pretensión menor a **20 SMLMV** | [`plantillas/06-demanda-sin-abogado-minima-cuantia.md`](../plantillas/06-demanda-sin-abogado-minima-cuantia.md) |

## Lo que sigue necesitando apoyo especializado (para ser honestos)

- Procesos ejecutivos de **mayor cuantía** (más de 40 SMLMV) — ahí sí conviene un consultorio jurídico o abogado por la complejidad procesal.
- La **Insolvencia de Persona Natural No Comerciante** — no exige abogado obligatoriamente, pero por involucrar negociación con varios acreedores a la vez, este proyecto recomienda ir acompañado de un consultorio jurídico universitario o asesoría gratuita (ver `plantillas/05-guia-insolvencia-persona-natural.md`).
- Cualquier denuncia penal (ej. por usura) — la puedes presentar tú mismo ante Fiscalía o Policía, pero el desarrollo del proceso penal sí suele requerir acompañamiento.

## Por qué esto cambia la estrategia del proyecto

Antes, el proyecto explicaba **qué dice la ley**. Con esto, el proyecto explica **qué puedes hacer ahora mismo, tú solo, sin que el dinero sea la excusa**. Esta es la pieza que convierte la alfabetización legal en acción real — y es el argumento más fuerte contra el "monopolio de información" que describe el informe original (`docs/informe-situacion.md`, sección 4): las entidades que cobran saben que la mayoría de la gente cree que necesita plata para defenderse. No siempre es así.

## Próximos pasos

- [ ] Verificar el articulado exacto de la Ley 2220 de 2022 (reemplazó la Ley 640/2001) antes de citar un artículo específico sobre conciliación.
- [ ] Sumar este flujo "sin abogado" como una capa transversal del futuro calculador web (`docs/plan-lanzamiento-producto.md`): cada resultado del calculador debería decir explícitamente si el usuario necesita o no abogado para el siguiente paso.
