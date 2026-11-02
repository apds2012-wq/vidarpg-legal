# VIDA RPG · Europa y alrededores: qué leyes se aplican y qué falta en la política

Investigación del 2 de noviembre de 2026. Punto de partida: `BRIEF.md` y la política de privacidad en español (versión 2.17.1, 13-10-2026).
Regla: cada afirmación lleva su fuente y la fecha de consulta (2-11-2026, salvo que se diga otra). Lo que no se pudo comprobar en una fuente oficial o fiable va marcado **NO VERIFICADO**. Esto es investigación, no asesoramiento jurídico: antes de publicar, que lo revise un abogado.

Fuentes que no se pudieron leer: EUR-Lex devolvió páginas vacías, Fedlex solo carga con JavaScript, la tarifa del ICO dio 403 y la página de Garant salió con la codificación rota. Esos textos se tomaron de espejos fiables (legislation.gov.uk para la versión «UE retenida» de la Directiva 2011/83, justement.ch para la nLPD, consultant.ru), de páginas de la autoridad o de despachos. En cada caso se dice cuál.

---

## 0. Tabla resumen

| País / ley | ¿Se aplica a VIDA? | ¿Representante local? | ¿Registro o notificación? | Lo que hoy falta en la política o los términos | Grado de certeza |
|---|---|---|---|---|---|
| **UE · RGPD art. 13** | Sí (responsable establecido en España) | No (está en la UE). Sin DPD obligatorio (no hay observación sistemática a gran escala ni art. 9 a gran escala; art. 37) | No | Bases jurídicas por tratamiento, interés legítimo, papel de cada destinatario, garantías de RevenueCat y de Google, plazos de RevenueCat/Google, derecho a retirar el consentimiento, el derecho de oposición destacado, si dar los datos es obligatorio, que no hay decisiones automatizadas, art. 9 en el Coach, dirección del responsable (§1.1) | Alto (texto del RGPD conocido; lectura de la política hecha aquí) |
| **UE · Reglamento de IA 2024/1689 art. 50.1** | Sí: VIDA es **proveedor** de un sistema de IA (el Coach) que interactúa con personas | No (proveedor en la UE) | No | Avisar dentro de la app, a más tardar en la primera interacción, de que el Coach / el Sabio es una IA; el rol del Sabio puede «ocultarlo». Vigente desde el **2-8-2026, sin aplazamiento** del Omnibus. Art. 50.2 (marcado legible por máquina) desde el **2-12-2026** para los sistemas ya en el mercado | Medio-alto (fuentes secundarias coinciden; el Reglamento ómnibus, 2026/1744, no se leyó en el DOUE) |
| **UE · Directiva 2011/83 art. 6.1.c + TRLGDCU** | Sí (venta a distancia a consumidores: PRO, programas, créditos) | — | — | Hace falta la **dirección geográfica** del establecimiento; con solo un correo no basta. El teléfono es obligatorio solo «si existe» (STJUE C-649/17) | Alto |
| **España · LSSI art. 10** | Sí: una app con compras es un servicio de la sociedad de la información; el prestador está establecido en España (art. 2) | — | — | **Nombre, domicilio, correo y NIF** de forma permanente, fácil, directa y gratuita | Alto (BOE) |
| **UE · Directiva 2023/2673 (botón de desistimiento, art. 11 bis Dir. 2011/83)** | Probable, en los contratos que se celebran a través de la interfaz de la app (compras con la hoja de Google Play): **zona gris** | — | — | Una «función de desistimiento» visible en la app, con acuse en soporte duradero. Aplicable desde el **19-6-2026**. **España no la ha transpuesto** (consulta: oct. 2026); otros Estados sí (Alemania: § 356a BGB) | Medio |
| **UE · DSA 2022/2065 arts. 11-12** | **No**: VIDA no es un servicio intermediario (no aloja ni difunde contenido de terceros) | No | No | Nada | Alto |
| **Reino Unido · UK GDPR** | Sí (art. 3.2: ofrece servicios a residentes del Reino Unido) | **Sí, con probabilidad** (art. 27). La excepción del tratamiento «ocasional» es estrecha y el servicio es continuo. La DUAA 2025 **no** suprimió el art. 27 | Tasa del ICO: **dudosa** para responsables de fuera del Reino Unido (NO VERIFICADO) | Una sección para el Reino Unido: representante (nombre y dirección), el ICO (desde el 30-9-2026, Information Commission) y las transferencias según el régimen del Reino Unido | Medio-alto |
| **Reino Unido · DMCC Act 2024, contratos de suscripción** | Sí, en la suscripción PRO para consumidores del Reino Unido (si cae sobre el desarrollador o sobre Google: NO VERIFICADO) | — | — | Desde el **1-1-2027** (si el Parlamento aprueba el reglamento): información previa, **recordatorios** antes de cada renovación y del final de la prueba, salida fácil y desistimiento de 14 días en cada renovación | Medio (fuente: despacho, 20-10-2026) |
| **Suiza · nLPD (RS 235.1)** | Sí (afecta a personas en Suiza) | **No**: el art. 14 exige gran escala, regularidad y **alto riesgo** a la vez | No (el registro de actividades solo para algunos; la exención de menos de 250 empleados queda NO VERIFICADO) | Art. 19.4: nombrar el **Estado de destino** (EE. UU.) y la garantía (Swiss-US DPF / cláusulas tipo); la autoridad suiza es el **PFPDT/FDPIC** | Alto (justement.ch, EDÖB) |
| **Noruega, Islandia, Liechtenstein** | Sí, el RGPD por el Acuerdo EEE | No | No | Nada aparte; «la autoridad de tu país» ya los cubre | Alto (decisión del Comité Mixto: NO VERIFICADO en esta sesión) |
| **Turquía · KVKK 6698** | **Riesgo real**: la ley no fija un ámbito territorial y la Autoridad la aplica a extranjeros que dan servicio en Turquía | **Sí, para inscribirse en VERBIS** (representante: persona jurídica turca o ciudadano turco). La exención de menos de 50 empleados y 100 M TRY **probablemente no vale para los extranjeros** (las fuentes no coinciden) | VERBIS; además, notificar los contratos tipo de transferencia en 5 días hábiles (art. 9, desde el 1-6-2024) | Aviso del art. 10 (identidad, representante, finalidades, destinatarios y el porqué, forma y base de la recogida, derechos del art. 11). **Alternativa: no distribuir en Turquía** | Medio |
| **Rusia · 152-FZ** | **Sí sobre el papel** (art. 1.1, desde el 1-9-2022: extranjeros que tratan datos de ciudadanos rusos por contrato o consentimiento) | No se pide representante | Notificación a Roskomnadzor (art. 22) y de transferencias (art. 12); localización (art. 18.5, reforzada el 1-7-2025) | La política rusa debería tener la forma del art. 18.1; la localización no se puede cumplir con Cloudflare. **Alternativa: Coach y códigos apagados con la región RU, o no distribuir en Rusia** | Medio |
| **Rusia · 236-FZ («landing law»)** | **No**: umbral de más de 500 000 usuarios al día en Rusia | — | — | Nada | Alto |
| Serbia · ZZPL 2018 | Probable (copia el RGPD) | **Sí, probable** (art. 44, como el art. 27 del RGPD; excepción ocasional, estrecha) | NO VERIFICADO | Representante | Medio |
| Moldavia · Ley 195/2024 | Probable, desde el **23-8-2026** | **Sí** (representante por escrito si se ofrecen servicios a personas en Moldavia) | NO VERIFICADO | Representante | Bajo-medio |
| Montenegro · ley 133/2026 | Desde el **19-3-2027** (según fuente secundaria) | Sí, con excepción ocasional y de bajo riesgo | NO VERIFICADO | Vigilar | Bajo |
| Georgia · ley de 2023 | Probable | Representante para extranjeros, **salvo los de la UE** (según fuente secundaria) | NO VERIFICADO | Nada, si la exención UE se confirma | Bajo |
| Ucrania, Kazajistán, Bielorrusia, Albania, Macedonia del Norte, Bosnia y Herzegovina, Armenia, Azerbaiyán | NO VERIFICADO | NO VERIFICADO | Kazajistán: localización (Ley 94-V, art. 12.2), que la doctrina aplica a quien está establecido allí | — | Bajo |

---

## 1. Unión Europea

### 1.1 RGPD art. 13: huecos concretos en la política actual

La política es muy completa en **qué** datos salen y **a dónde**, pero le faltan varias menciones obligatorias del art. 13.1 y 13.2. Repasado contra el texto del artículo:

| Art. 13 | Lo que pide | Lo que dice hoy la política | Hueco |
|---|---|---|---|
| 1.a | Identidad y **datos de contacto** del responsable | «Alex Vida, desarrollador independiente, España» y el correo (§19) | Falta la dirección postal: el RGPD no la nombra, pero la LSSI y la Directiva 2011/83 sí (§1.3). Comprobar que «Alex Vida» es el nombre legal completo |
| 1.b | Contacto del DPD | No hay | Basta con decir «No hay delegado de protección de datos: no es obligatorio (art. 37)». No es estrictamente necesario, pero evita preguntas |
| 1.c | Fines **y base jurídica de cada tratamiento** | Solo en los códigos (§11: «darte el acceso… e interés legítimo») | **Falta en el Coach, los anuncios, las compras, los créditos, los antiabuso (huellas de IP e ID), la recuperación de créditos y la descarga de la música.** Propuesta en el §1.6 |
| 1.d | **Intereses legítimos** concretos, cuando son la base | Implícito («frenar el abuso») | Nombrarlos: evitar abusos y el agotamiento del cupo común, la seguridad del servicio y evitar el doble descuento |
| 1.e | Destinatarios o categorías | Cloudflare, Google (AdMob, Play), RevenueCat | Decir su **papel**: Cloudflare, encargado; RevenueCat, encargado (comprobar su DPA); Google AdMob, **responsable independiente** de lo que recoge su SDK (comprobar las condiciones de Google sobre responsables) |
| 1.f | Transferencias a terceros países y **garantías**, y **cómo obtener una copia** | Cloudflare: cláusulas tipo + DPF | **Faltan RevenueCat (EE. UU.)**, Google (DPF / cláusulas tipo) y la forma de pedir una copia de las garantías |
| 2.a | **Plazo** de conservación o criterio | Créditos: 24 meses; huellas: un día; justificantes en el teléfono | Falta cuánto guarda **RevenueCat** el recibo y el ID anónimo (remitir a su política, o fijarlo en su panel) y el criterio de Google (sus políticas). Decir que las devoluciones y los datos fiscales se guardan lo que pida la ley, si el desarrollador los tiene (en Google Play los tiene Google: comprobar) |
| 2.b | Derechos: acceso, rectificación, supresión, limitación, **oposición** y portabilidad | Están en el §15 | **El derecho de oposición al tratamiento por interés legítimo** tiene que mencionarse **de forma explícita y separada** (art. 21.4). Falta la oposición a las huellas antiabuso |
| 2.c | **Retirar el consentimiento** cuando es la base, sin afectar a lo anterior | Solo «cambiar tu elección» de los anuncios | Una frase general: «Cuando la base es tu consentimiento (anuncios personalizados; el Coach, si hay datos del art. 9), puedes retirarlo cuando quieras: Ajustes → Anuncios → Privacidad de los anuncios, o apagar el Coach. Lo hecho antes sigue siendo lícito» |
| 2.d | Derecho a reclamar ante una autoridad | Sí (AEPD o la de tu país) | Correcto. Opcional: el enlace a la AEPD |
| 2.e | Si dar los datos es **un requisito legal o contractual**, si es obligatorio y **qué pasa si no se dan** | No se dice como tal (se entiende que todo es opcional) | Una frase: «Ningún dato es obligatorio por ley. Para el Coach, las compras, los créditos y los códigos hacen falta los datos descritos; sin ellos esa función no está disponible y el resto de la app funciona igual» |
| 2.f | **Decisiones automatizadas**, incluida la elaboración de perfiles (art. 22) | No se dice | «VIDA no toma decisiones automatizadas con efectos jurídicos ni significativos (art. 22). Las propuestas del Coach son sugerencias que tú aceptas o no. El rango, la clase de personaje, el perfil de afinidad y la red de crisis se calculan en el teléfono y no deciden nada sobre ti». Las 'decisiones' de cupo y antiabuso (dar o negar una consulta) son de bajo impacto: mencionarlas por transparencia |

Otros huecos fuera del art. 13 que conviene tratar:
- **Categorías especiales (art. 9) en el Coach.** El resumen que viaja lleva «los vicios registrados» (beber, fumar, una caída propia con su categoría), objetivos corporales y de forma física y, con la red de crisis, señales de autolesión o conducta alimentaria si están en el texto. Eso puede revelar **datos de salud**. Aunque viaje seudonimizado (ID aleatorio e IP), el Worker lo trata. Si se considera dato de salud, hace falta una excepción del art. 9.2; la única que encaja es el **consentimiento explícito** (art. 9.2.a). **Propuesta**: una casilla de consentimiento explícito la primera vez que se usa el Coach, o quitar los vicios del resumen, o argumentar por escrito que no son datos de salud. Es el hueco **de más riesgo** (lectura propia del RGPD, sin fuente externa en esta sesión).
- **Edad de consentimiento en España: 14 años** (LOPDGDD art. 7). La política dice «para adultos». Basta, pero en la ficha de Play la clasificación de edad debería ir en la misma línea (NO VERIFICADO aquí).
- **Seudonimización (art. 11)**: está bien explicada. Conviene decir que, si no se puede identificar a la persona, algunos derechos solo se ejercen con el número de pedido GPA (ya se dice para los créditos).

Fuente: RGPD, Reglamento (UE) 2016/679, arts. 9, 11, 13, 21, 22, 37 (texto oficial en eur-lex.europa.eu; no se pudo descargar el 2-11-2026 y se cita del texto conocido. **Comprobar las citas literales contra EUR-Lex antes de publicar**).

### 1.2 Reglamento de IA (UE) 2024/1689, art. 50.1

- **Qué pide**: los proveedores garantizan que los sistemas de IA destinados a interactuar directamente con personas físicas se diseñen de modo que esas personas **sepan que interactúan con una IA**, salvo que sea evidente para una persona razonablemente informada (art. 50.1). La información se da de forma clara, **a más tardar en la primera interacción** (art. 50.5) (texto del art. 50 tal como lo resumen FPF y aiactblog.nl; DOUE no leído).
- **¿Es VIDA proveedor?** Lectura propia: VIDA integra un modelo de uso general (Gemma, en Workers AI) en un sistema que pone en servicio con su nombre («Coach IA»), así que es **proveedor del sistema** que interactúa con quien juega. El art. 50.1 se aplica.
- **El riesgo concreto**: desde la 2.16, el Coach es **un diálogo de rol con el Sabio**, un personaje del juego. Si el cuadro del Sabio no dice que la respuesta la escribe una IA, deja de ser «evidente». **Propuesta**: una marca visible en el cuadro del Sabio cuando habla el Coach (por ejemplo «Respuesta generada por IA») y una frase en la primera consulta, en los ocho idiomas.
- **Fecha y Omnibus**: el «AI Omnibus» se publicó en el DOUE el 24-7-2026 (FPF, 28-7-2026, act. 5-8-2026) como **Reglamento (UE) 2026/1744**, en vigor el 27-7-2026 según Usercentrics y otras fuentes secundarias. **El art. 50 en general NO se aplazó: se aplica desde el 2-8-2026.** Solo el **art. 50.2** (marcado legible por máquina del contenido sintético) pasa al **2-12-2026** para los sistemas ya en el mercado. Los de alto riesgo pasan al 2-12-2027 (anexo III) y al 2-8-2028 (anexo I).
  - Fuentes: FPF, «The AI Act implementation timeline: what changes under the AI Omnibus?» (fpf.org, consultado el 2-11-2026); aiactblog.nl, «Article 50 transparency obligations… not been postponed»; Gibson Dunn; Usercentrics. **El texto del DOUE (OJ L 2026/1744) no se leyó: comprobarlo.**
- **Art. 50.2** (lectura propia, para comprobar): obliga a los **proveedores** de sistemas que generan **texto** sintético a marcarlo en formato legible por máquina, con excepciones (función de ayuda a la edición estándar, entre otras). El Coach genera texto, así que hay que mirar si desde el **2-12-2026** hace falta un marcado técnico (metadatos) en las respuestas. **NO VERIFICADO si la excepción cubre un asistente como este.**
- **En la política**: añadir en el §8 una frase del tipo «El Coach IA es un sistema de inteligencia artificial: sus respuestas las genera un modelo de lenguaje, también cuando te habla el Sabio».

### 1.3 Información precontractual y datos del prestador: Directiva 2011/83 art. 6, TRLGDCU y LSSI art. 10

- **Directiva 2011/83 art. 6.1.c**, tras la Directiva (UE) 2019/2161: la **dirección geográfica** donde está establecido el comerciante y **su teléfono y su correo**; además, si ofrece otros medios de comunicación en línea, también esos (texto de la 2019/2161 art. 4, en legislation.gov.uk, consultado el 2-11-2026).
  - STJUE de 10-7-2019, **C-649/17, Amazon EU**: no se puede imponer el teléfono **en todo caso**. Hay que ofrecer un medio de comunicación directo y eficaz, y el teléfono solo «si se dispone de él» (comunicado de prensa del TJUE cp190089, curia.europa.eu).
  - **Conclusión**: **el correo NO basta para la dirección geográfica**, que es una mención separada y obligatoria. Sirve una dirección profesional o de domiciliación (lectura propia: la norma pide «dirección geográfica del establecimiento», no el domicilio particular, pero un autónomo sin local suele tener que dar el suyo fiscal o una de domiciliación; **consultar a un abogado**).
  - En España la incorpora el **TRLGDCU art. 97.1** (RDL 1/2007): mencionado en el `BRIEF`; el texto del art. 97 no se descargó del BOE en esta sesión (**NO VERIFICADO literal**).
- **LSSI (Ley 34/2002) art. 10.1** (BOE, texto consolidado, act. 23-1-2025; art. 10 modificado por última vez el 10-5-2014): el prestador da acceso permanente, fácil, directo y gratuito a: a) **nombre o denominación social; residencia o domicilio** (o un establecimiento permanente en España) y **correo** u otro medio de comunicación directa y efectiva; b) datos registrales (si los hay); e) **NIF**; f) precios claros con impuestos; g) códigos de conducta.
  - **¿Se aplica a una app?** Sí, lectura propia: la LSSI se aplica a los prestadores establecidos en España (art. 2.1) y una app que vende suscripciones y contenidos a distancia, a petición del usuario, es un servicio de la sociedad de la información (Anexo a; el Anexo no se pudo leer entero en esta sesión, NO VERIFICADO literal). Los servicios no remunerados entran si son actividad económica.
  - **Hueco**: hoy no se publican **domicilio ni NIF**. Hay que añadirlos en una página «Aviso legal / Datos del prestador» del sitio legal y en Más → Privacidad o Términos dentro de la app.

### 1.4 Directiva (UE) 2023/2673, la «función de desistimiento» (art. 11 bis de la Dir. 2011/83)

- **Qué pide**: en los contratos a distancia celebrados **a través de una interfaz en línea**, una función de desistimiento **fácil de encontrar y bien visible** («desistir del contrato aquí» o similar), una confirmación y un **acuse de recibo en soporte duradero**; además, la información precontractual dice que existe y dónde está. Se transponía antes del **19-12-2025** y se aplica desde el **19-6-2026** (iubenda; Ecija; OCU, nota del 19-6-2026).
- **España**: **no transpuesta** a la fecha de las fuentes. La OCU lo denunció en junio de 2026; Grant Thornton (mayo de 2026) la ligaba al anteproyecto de ley de crédito al consumo que modifica el TRLGDCU; Menorca.info (18-7-2026) dice que aún no está; la Comisión abrió un procedimiento de infracción contra España y otros 20 Estados (Ecija). **No se encontró en el BOE una norma de transposición posterior a julio de 2026: comprobar en el BOE.** Alemania la transpuso como § 356a BGB (scandiweb, fuente comercial).
- **¿Afecta a VIDA?** Zona gris (lectura propia):
  - La compra se cierra en la hoja de Google Play, pero la empieza la interfaz de la app, y en las compras dentro de una app el desarrollador suele ser el comerciante frente al consumidor. Que Google sea el «revendedor» a efectos de IVA no lo resuelve (NO VERIFICADO el papel exacto de Google en las condiciones de Play para el EEE).
  - Mientras España no la transponga, la directiva no obliga directamente al particular en relaciones entre privados. Pero **a un consumidor alemán o francés se le pueden aplicar sus normas nacionales imperativas** (Reglamento Roma I, art. 6, cuando la actividad se dirige a su país: lectura propia).
  - Ya existe el derecho de desistimiento de 14 días con su excepción para el contenido digital consumido (arts. 103.m y 98.7 TRLGDCU, citados en la ficha del proyecto).
  - **Propuesta barata**: en Ajustes → Compras, un botón «Desistir de un contrato» que abra un formulario (producto, número de pedido GPA, fecha) y mande un correo con copia al usuario como acuse en soporte duradero; avisarlo en la pantalla de compra y en los Términos. Para PRO, «Cancelar la suscripción» enlaza a Google Play: cancelar no es lo mismo que desistir, y los Términos deben distinguirlos.

### 1.5 DSA, Reglamento (UE) 2022/2065, arts. 11-12

- Los puntos de contacto (art. 11, para las autoridades; art. 12, para los destinatarios) se aplican a los **prestadores de servicios intermediarios**: mera transmisión, memoria caché y alojamiento de datos (art. 3.g).
- **VIDA no lo es** (lectura propia): no aloja contenido de terceros ni lo difunde. El Worker procesa la consulta y devuelve la respuesta a la misma persona, sin guardar nada. **No se aplica.** Solo cambiaría si un día hubiera contenido compartido entre usuarios. (Texto del DSA no descargado en esta sesión; definiciones de memoria del texto oficial: **comprobar contra EUR-Lex**.)

### 1.6 España, otras leyes
- La «Ley 7/2024» del encargo: **no se identificó** ninguna ley española de ese número que afecte a esto, y no se inventa. LOPDGDD (LO 3/2018): edad de 14 años (art. 7) y el deber de información por capas (art. 11), que la política ya cumple en la práctica. (Texto no descargado en esta sesión.)

### 1.7 Propuesta de bases jurídicas para el §8-§12 de la política (para que la valide un abogado)

| Tratamiento | Base propuesta (art. 6 RGPD) |
|---|---|
| Consulta al Coach (resumen + país) | 6.1.b, prestar el servicio que pides; si hay datos de salud, **9.2.a, consentimiento explícito** |
| Huellas de IP e ID, contadores, topes | 6.1.f, interés legítimo en frenar el abuso y repartir un cupo común; **derecho de oposición** |
| Código de país para la derivación de crisis | 6.1.b o, mejor, 6.1.d (interés vital) solo si salta la red; si no, 6.1.b |
| Anuncios bonificados | Google es responsable de su SDK; consentimiento (6.1.a / ePrivacy, art. 22.2 LSSI) mediante UMP para los personalizados; los no personalizados, según lo que Google declare |
| Compras, PRO, programas (RevenueCat) | 6.1.b, contrato |
| Saldo de créditos, pedidos, 24 meses | 6.1.b y 6.1.f (prueba de la compra y del gasto, devoluciones) |
| Recuperar créditos | 6.1.b |
| Códigos | 6.1.b y 6.1.f (ya está) |
| Correos de privacidad y desistimiento | 6.1.c, obligación legal |

---

## 2. Reino Unido

### 2.1 UK GDPR art. 27, representante
- **Texto vigente** (legislation.gov.uk, «latest available (revised)», consultado el 2-11-2026): cuando se aplica el art. 3.2, el responsable **designa por escrito un representante en el Reino Unido** (27.1). No hace falta (27.2.a) si el tratamiento es **ocasional**, no incluye a gran escala categorías especiales ni datos penales y no es probable que entrañe un riesgo; ni (27.2.b) si es una autoridad pública.
- **DUAA 2025**: **no suprimió el art. 27**. Su última modificación es del **30-9-2026** (S.I. 2026/386 y 2026/1015): cambia una palabra del apartado 4, lo de «the Commission». Un comentario de Fieldfisher que lo daba por «en blanco» **no coincide con el texto oficial**.
- **Autoridad**: desde el **30-9-2026** el Information Commissioner es la **Information Commission**, que sigue usando la marca ICO (gov.uk, «Information Commission succeeds the ICO as UK's data protection regulator»; LexisNexis, 11-9-2026).
- **¿Se aplica a VIDA?** El art. 3.2.a sí: la app se ofrece a residentes del Reino Unido en inglés y con precios. Sobre la excepción (lectura propia, que coincide con la guía 3/2018 del CEPD sobre el art. 27 del RGPD, no releída en esta sesión): «ocasional» se lee de forma estrecha, y un servicio permanente (Coach, saldo de créditos guardado 24 meses, códigos) difícilmente lo es, aunque los datos sean mínimos y seudonimizados. **Conclusión: hace falta representante, con probabilidad**, salvo que se defienda por escrito que el tratamiento propio en el servidor es ocasional y de bajo riesgo. Un representante comercial cuesta poco al año (NO VERIFICADO el precio).
- **Tasa de protección de datos** (Data Protection (Charges and Information) Regulations 2018, reg. 2): la paga todo «data controller» salvo que todo su tratamiento esté exento (legislation.gov.uk). **No queda claro si alcanza a los responsables de fuera del Reino Unido**: una respuesta del ICO a una petición de información (registro de divulgación, mayo de 2025) **retuvo** su guía interna sobre eso, y la página del ICO dio 403. **NO VERIFICADO**. Va en la lista de dudas para el abogado o para el representante.
- **En la política**: un apartado «Reino Unido»: el representante (nombre y dirección, si se designa), la autoridad («Information Commission (ICO), ico.org.uk») y que las transferencias desde el Reino Unido a EE. UU. van por la UK Extension del DPF o por el IDTA/Addendum (comprobar qué firma cada proveedor: **NO VERIFICADO**).

### 2.2 DMCC Act 2024, Parte 4, cap. 2: contratos de suscripción
- **Fecha**: según Wiggin (seguimiento de la DMCC, act. 20-10-2026), el proyecto de **Consumer Subscription Contracts (Cancellation and Information) Regulations 2026** se presentó al Parlamento. **Si se aprueba, entra en vigor el 1-1-2027** y se aplica a los contratos celebrados desde esa fecha. Antes se habló de la primavera de 2026, del otoño de 2026 y de la primavera de 2027 (Taylor Wessing, abril de 2026). **No se comprobó en gov.uk: confirmarlo.**
- **Qué exige** (Wiggin, resumen del 2-4-2026; Osborne Clarke): información clara antes del contrato, **recordatorios** periódicos antes de cada renovación automática (y antes de que una prueba gratuita pase a ser de pago), una **salida sencilla** y **desistimiento de 14 días** también tras cada renovación, con reembolso total o proporcional.
- **¿Se aplica a PRO vendido por Google Play?** Sí al tipo de contrato (renovación automática, contenido digital o servicio). **No está claro quién es el «trader»** frente al consumidor, si el desarrollador o Google, ni si las tiendas tienen un régimen propio en el reglamento: **NO VERIFICADO**. Lo prudente es preparar: (a) la información previa en la pantalla de PRO (precio, frecuencia, cuándo cobra la prueba, cómo cancelar); (b) un recordatorio dentro de la app antes del cobro de la prueba anual y antes de cada renovación (Google Play ya manda algunos correos, pero no se ha comprobado que cumplan); (c) en los Términos, el desistimiento de 14 días tras la renovación para el Reino Unido.

---

## 3. Suiza: nLPD (RS 235.1, en vigor desde el 1-9-2023)
- **Art. 14** (justement.ch, texto en inglés de la versión oficial): los responsables privados con sede o domicilio en el extranjero designan representante en Suiza si tratan datos de personas en Suiza y el tratamiento: a) está ligado a una oferta de bienes o servicios o a la observación del comportamiento en Suiza; b) **es a gran escala**; c) **es regular**; d) **presenta un riesgo elevado** para la personalidad. El encabezado («the following requirements») indica que son **cumulativos**, igual que el Onlinekommentar del art. 14-15. **VIDA no cumple b) ni d) → no necesita representante.** (Art. 15: deberes del representante, solo si existe.)
- **Art. 16-17**: una comunicación al extranjero es libre si el Consejo Federal reconoce un nivel adecuado (anexo 1 de la OPDo). Para **EE. UU.**, solo las **empresas certificadas** en el **Swiss-US DPF**, desde el **15-9-2024** (EDÖB, 15-8-2024; Consejo Federal, decisión del 14-8-2024). Si no, cláusulas tipo (art. 16.2). Comprobar que Cloudflare, RevenueCat y Google están certificados también en la parte suiza del DPF (**NO VERIFICADO**).
- **Art. 19.4**: si los datos se comunican al extranjero, hay que decir **el Estado** o el organismo internacional de destino y, en su caso, **la garantía del art. 16.2** (texto citado por la EDÖB y justement.ch). Basta con nombrar grupos de países (Onlinekommentar del art. 19). **Hueco**: la política dice «fuera del Espacio Económico Europeo», pero no nombra **Estados Unidos** ni la garantía de cada proveedor.
- **Art. 21** (decisiones individuales automatizadas): basta con la misma frase de «no hay» del RGPD (texto del art. 21 no leído en esta sesión).
- **Autoridad**: el Préposé fédéral / **PFPDT (FDPIC / EDÖB)**. Ante él no hay una «reclamación» al estilo del RGPD, sino una denuncia que puede abrir una investigación (lectura propia, sin fuente en esta sesión). En la política: «En Suiza, el Préposé fédéral à la protection des données et à la transparence (PFPDT), edoeb.admin.ch».

## 4. Noruega, Islandia y Liechtenstein
- El RGPD se aplica por el Acuerdo EEE (decisión del Comité Mixto del EEE n.º 154/2018, en vigor el 20-7-2018: **NO VERIFICADO en esta sesión**). Responsable establecido en España → **ni representante ni registro**. Autoridades: Datatilsynet (NO), Persónuvernd (IS), Datenschutzstelle (LI). «La autoridad de tu país» ya los cubre; nombrarlas es opcional.

## 5. Turquía: KVKK n.º 6698
- **Ámbito**: la ley **no tiene un artículo de ámbito territorial**. La Autoridad la aplica a los extranjeros con el representante del art. 11 del Reglamento del Registro (BOE turco n.º 30286) y con la decisión 2019/10 de brechas (Rona Legal, 2026, fuente de despacho).
- **VERBIS** (kvkk.gov.tr, «Veri Sorumluları Siciline Kayıt İstisnaları», 31-1-2018): **en principio, todo responsable se inscribe antes de tratar**, y el Consejo puede eximir. Exenciones según fuentes secundarias: decisión 2018/87, modificada por la **2023/1154** (6-7-2023): menos de **50 empleados** y balance de menos de **100 M TRY**, salvo que la actividad principal sea con categorías especiales; decisión **2025/1572** (4-9-2025, efecto el 1-10-2025, fecha que no coincide entre fuentes) para categorías especiales: menos de 10 empleados y 10 M TRY. **Las fuentes no coinciden sobre si estas exenciones valen para los responsables de fuera de Turquía**; la mayoría dice que **no** (Konsorsiyum, Rona Legal, Halil Bakırcı). **NO VERIFICADO en kvkk.gov.tr.**
- **Representante**: el extranjero se inscribe por medio de un **representante** que sea persona jurídica establecida en Turquía o ciudadano turco (Rona Legal; Prighter).
- **Art. 10, deber de informar**: identidad del responsable y **de su representante**, finalidad, a quién se transfieren y para qué, **forma y causa jurídica de la recogida**, y los derechos del art. 11 (Rona Legal).
- **Art. 9, transferencias (Ley 7499, BOE turco del 12-3-2024; en vigor el 1-6-2024)**: adecuación, o garantías adecuadas (contrato tipo **notificado a la Autoridad en 5 días hábiles**), o excepciones ocasionales. El consentimiento expreso de antes solo valió hasta el 1-9-2024 (Mondaq; Erdem & Erdem). Multa por no notificar: 90 308-1 806 177 TRY en 2026 (cifra de despacho, NO VERIFICADO oficial).
- **Conclusión**: cumplir de verdad (representante, VERBIS, contratos tipo con Cloudflare y RevenueCat notificados, aviso en turco) es caro para un particular. La app no está en turco ni se anuncia en Turquía, pero la KVKK no tiene un criterio de «dirigirse a». **Alternativa razonable: quitar Turquía de los países de distribución en Play Console** o apagar ahí las funciones que salen del teléfono. Si se mantiene, añadir el aviso del art. 10.

## 6. Rusia
### 6.1 152-FZ «О персональных данных»
- **Ámbito sobre extranjeros**: **art. 1, parte 1.1** (añadida por la 266-FZ del 14-7-2022; en vigor el 1-9-2022): la ley se aplica al tratamiento de datos de **ciudadanos rusos** por personas jurídicas o físicas **extranjeras** sobre la base de un **contrato** del que el ciudadano es parte, de otros acuerdos o de su **consentimiento** (consultant.ru, ed. del 26-7-2026).
- **¿Trata VIDA «datos personales» de ciudadanos rusos?** El art. 3 define el dato personal como cualquier información relativa, directa o indirectamente, a una persona determinada o determinable (definición conocida, no releída en esta sesión). Con una lectura amplia, **la IP**, aunque solo se guarde una huella de un día, y el **ID aleatorio de instalación** pueden serlo. El resumen del Coach va ligado a ese ID durante la petición. Los usos del Coach y de los códigos se hacen según los Términos (un contrato). **Riesgo: aplicable sobre el papel**, aunque el volumen es pequeño, se seudonimiza y no hay compras ni anuncios en Rusia.
- **Obligaciones que chocarían**:
  - **Art. 18.5, localización**: el registro, la sistematización, la acumulación, el almacenamiento… de los datos de ciudadanos rusos, con bases de datos **en Rusia**. Desde el **1-7-2025** (23-FZ del 28-2-2025) se refuerza y prohíbe usar bases en el extranjero para eso; Minciffry dice que no regula la transferencia de lo ya recogido en Rusia (ComNews, 30-6-2025; Konsu Group). **El Worker en Cloudflare no puede cumplirlo.** Multas para personas jurídicas de 6 a 18 M RUB (ComNews).
  - **Art. 22**: notificar a Roskomnadzor antes de tratar (con excepciones); **art. 12**: notificar las transferencias transfronterizas (266-FZ) (Gorodissky; PGP Law).
  - **Art. 18.1, parte 2**: publicar la política del operador. La política rusa ya está publicada, pero no tiene la estructura que pide Roskomnadzor (finalidades, categorías, bases, plazos y destrucción por tratamiento) (NO VERIFICADO el formato exacto).
  - En la práctica, lo que hace Roskomnadzor contra los extranjeros que no cumplen es **bloquear** el recurso (Gorodissky). No se encontró ningún caso contra un desarrollador pequeño (NO VERIFICADO).
- **Propuesta**: (a) **apagar el Coach y el canje de códigos** cuando la región del sistema sea RU (como ya se hace con anuncios y compras), dicho con honestidad; ojo, la región no es la ciudadanía, así que reduce el riesgo pero no lo elimina; o (b) **no distribuir en Rusia**; o (c) aceptar el riesgo por escrito. Con (a), la política rusa dice que desde Rusia no sale ningún dato.
### 6.2 236-FZ, la «landing law» (1-7-2021)
- Se aplica a los extranjeros con un recurso (también una app) de **más de 500 000 usuarios al día** en Rusia (medido según la metodología de Roskomnadzor del 16-7-2021) **y** alguna de estas condiciones: contenido en ruso, publicidad dirigida a Rusia, tratamiento de datos de usuarios en Rusia o cobros desde Rusia (Unicon). La 290-FZ del 31-7-2025 añadió las plataformas digitales intermediarias registradas, aunque tengan ≤ 500 000 usuarios (consultant.ru), algo que no es VIDA. **No se aplica a VIDA.**

## 7. Otros países (una línea cada uno)
- **Serbia**, Ley de protección de datos (Službeni glasnik 87/2018): **art. 44, representante** para los responsables de fuera de Serbia, copiado del art. 27 del RGPD, con la excepción del tratamiento ocasional (estrecha en la práctica). No designarlo es una falta (art. 95) (Žunić; ZS Law; CMS). **Probable.** Registro: NO VERIFICADO.
- **Ucrania**, Ley 2297-VI (2010): representante NO VERIFICADO; registro: solo notificación al Comisionado para tratamientos de riesgo (NO VERIFICADO).
- **Kazajistán**, Ley 94-V (2013): **localización** (art. 12.2, desde el 1-1-2016), que la doctrina aplica a quien está establecido allí (Morgan Lewis 2024; Lexology). Representante: NO VERIFICADO.
- **Bielorrusia**, Ley 99-Z (2021): NO VERIFICADO (representante y registro).
- **Georgia**, Ley de protección de datos (2023, en vigor el 1-3-2024: fecha NO VERIFICADO): «representante especial» para los extranjeros que usan medios técnicos en Georgia, **salvo los de la UE** o de países con nivel UE (Global Legal Post, fuente secundaria).
- **Moldavia**, Ley 195/2024: en vigor el **23-8-2026**; representante por escrito para los no establecidos que ofrecen servicios en Moldavia (DLA Piper; MyData-TRUST). **Probable.** Exención ocasional: NO VERIFICADO.
- **Albania**, Ley 124/2024: NO VERIFICADO.
- **Macedonia del Norte**, Ley de protección de datos (2020): representante NO VERIFICADO (es copia del RGPD; probable art. 27 equivalente, sin confirmar).
- **Bosnia y Herzegovina**: NO VERIFICADO.
- **Montenegro**, ley 133/2026: en vigor el 19-9-2026, aplicable desde el **19-3-2027**; representante por escrito con excepción ocasional y de bajo riesgo (Rona Legal; Yeandel: fuentes secundarias).
- **Armenia** y **Azerbaiyán**: sin cláusula de localización de datos personales según un resumen secundario (Siberson). Representante: NO VERIFICADO.

---

## 8. Qué añadir: propuesta en español (para los ocho idiomas)

**A. En la política de privacidad**
1. **§19 Responsable** → «Alex [apellidos legales], autónomo, NIF [●], [dirección geográfica o de domiciliación], España. Contacto: vidarpgapp@gmail.com. No hay delegado de protección de datos: no es obligatorio en este caso.»
2. **Nueva sección «Bases jurídicas y plazos»**, con la tabla del §1.7 (tratamiento → base → plazo → destinatario y su papel → país y garantía).
3. **Transferencias**: «Cloudflare, Inc., RevenueCat, Inc. y Google LLC están en **Estados Unidos**. Garantías: Data Privacy Framework UE-EE. UU. (y sus extensiones del Reino Unido y de Suiza) y cláusulas contractuales tipo. Puedes pedir una copia en vidarpgapp@gmail.com.» (comprobar la certificación de cada uno).
4. **Derechos**: añadir, en un párrafo aparte, «**Derecho de oposición**: puedes oponerte a los tratamientos basados en interés legítimo (las huellas antiabuso)…»; «**Retirar el consentimiento**: …»; «No está obligado a darnos datos…»; «No hay decisiones automatizadas con efectos jurídicos (art. 22)…».
5. **Coach**: «El Coach IA es un sistema de inteligencia artificial: sus respuestas las escribe un modelo de lenguaje, también cuando te habla el Sabio» (Reglamento de IA, art. 50.1). Y, si se mantienen los vicios en el resumen, el **consentimiento explícito** para los datos que puedan revelar salud (art. 9.2.a RGPD).
6. **Apartados por país**:
   - **Reino Unido**: representante (si se designa), Information Commission (ICO) y las garantías propias del Reino Unido.
   - **Suiza**: el Estado de destino (EE. UU.) con su garantía (art. 19.4 nLPD) y el PFPDT; «no estamos obligados a designar representante (art. 14 nLPD)».
   - **Turquía** (si no se excluye): el aviso del art. 10 KVKK.
   - **Rusia**: el estado real (lo que sale o no sale con la región RU) y la estructura del art. 18.1 152-FZ.
   - **Serbia y Moldavia**: representante, si se decide mantener la distribución allí.
7. **Plazos de RevenueCat y Google**: remitir a sus políticas con enlace, o fijar el plazo de RevenueCat en su panel y escribirlo.

**B. En los términos de uso y en la app**
1. **Aviso legal (LSSI art. 10)**: nombre, domicilio, NIF y correo, en el sitio legal y dentro de la app (Más → Aviso legal).
2. **Función de desistimiento** (Dir. 2023/2673): botón en Ajustes → Compras, con formulario y acuse en soporte duradero; mencionarlo antes de comprar; distinguir **cancelar** la suscripción de **desistir** del contrato.
3. **Reino Unido (desde el 1-1-2027)**: recordatorio dentro de la app antes del fin de la prueba de 7 días y de cada renovación; información previa de la suscripción en la pantalla de PRO; el desistimiento de 14 días tras la renovación para el Reino Unido.
4. **Marca de IA** en el cuadro del Sabio cuando habla el Coach, y comprobar si el art. 50.2 obliga a un marcado legible por máquina desde el 2-12-2026.

**C. Decisiones para el propietario**
- ¿Designar un representante en el **Reino Unido** (probable), en **Serbia** y en **Moldavia**, o quitar Serbia y Moldavia de la distribución?
- ¿**Turquía**: excluirla de Play o cumplir con VERBIS y su representante?
- ¿**Rusia**: apagar Coach y códigos con RU, no distribuir o aceptar el riesgo?
- ¿Vicios en el resumen del Coach: consentimiento explícito o fuera?

---

## Fuentes (consultadas el 2-11-2026)
- UK GDPR art. 27, texto vigente: https://www.legislation.gov.uk/eur/2016/679/article/27
- Data Protection (Charges and Information) Regulations 2018, reg. 2: https://www.legislation.gov.uk/uksi/2018/480/regulation/2
- Information Commission: https://www.gov.uk/government/news/information-commission-succeeds-the-ico-as-uks-data-protection-regulator · https://www.lexisnexis.co.uk/legal/news/duaa-2025-provisions-establishing-new-information-commission-come-into-force-on-30-september-2026
- ICO, divulgación sobre la tasa para extranjeros (2025): https://cy.ico.org.uk/about-the-ico/our-information/disclosure-log/2025/05/ic-389257-h7r0/
- DMCC, seguimiento de Wiggin: https://www.wiggin.co.uk/insight/digital-markets-competition-and-consumer-act-tracker/ · Taylor Wessing: https://www.taylorwessing.com/en/insights-and-events/insights/2026/04/subscription-contracts · Osborne Clarke: https://www.osborneclarke.com/insights/uk-digital-markets-competition-and-consumers-act-subscription-contracts-regime-take-shape
- AI Omnibus: https://fpf.org/blog/the-ai-act-implementation-timeline-what-changes-under-the-ai-omnibus/ · https://www.aiactblog.nl/en/posts/article-50-transparency-deadline-2-august-2026 · https://www.gibsondunn.com/eu-ai-act-omnibus-agreement-postponed-high-risk-deadlines-and-other-key-changes/ · https://usercentrics.com/knowledge-hub/eu-ai-act-high-risk-delay-article-50-transparency-consent/
- Directiva 2019/2161 art. 4 (art. 6.1.c): https://legislation.gov.uk/eudr/2019/2161/article/4/adopted/data.pdf · STJUE C-649/17: https://curia.europa.eu/jcms/upload/docs/application/pdf/2019-07/cp190089en.pdf
- LSSI (BOE): https://www.boe.es/buscar/act.php?id=BOE-A-2002-13758
- Directiva 2023/2673: https://www.iubenda.com/es/blog/la-nueva-funcion-de-desistimiento-online-que-significa-la-directiva-ue-2023-2673-para-tu-empresa/ · https://www.ocu.org/organizacion/prensa/notas-de-prensa/2026/normabotondesistimiento190626 · https://www.ecija.com/actualidad-insights/nuevas-reglas-de-la-ue-relativas-al-desistimiento-en-los-contratos-celebrados-a-traves-de-interfaces-en-linea/ · https://www.grantthornton.es/contentassets/cc8a632b25b64dc0b9867edd24506591/0526_legal_novedades_mayo_grant-thornton.pdf · https://www.menorca.info/actualidad/dudas-respuestas/2026/07/18/2667119/union-europea-cambia-normas-obliga-paginas-webs-poner-boton-cancelacion-visible-para-compras-online.html
- nLPD art. 14: https://justement.ch/en/doc/act/ch/235_1/chap_2/sec_2/art_14 · art. 19: https://justement.ch/en/doc/act/ch/235_1/chap_3/art_19 · EDÖB, transferencias: https://www.edoeb.admin.ch/en/cross-border-transfer-of-personal-data · Swiss-US DPF: https://www.edoeb.admin.ch/en/15082024-new-swiss-us-data-privacy-framework · Onlinekommentar: https://onlinekommentar.ch/en/kommentare/dsg15 · https://onlinekommentar.ch/en/kommentare/dsg19
- KVKK: https://www.kvkk.gov.tr/Icerik/2044/Veri-Sorumlulugu-Siciline-Kayit-Istisnalari · https://www.ronalegal.com/en/blog/turkey-data-protection-law-6698-kvkk-foreign-companies-verbis-transfers-fines-2026 · https://konsorsiyumlegal.com/en/glossary/verbis/ · https://halilbakirci.av.tr/en/verbis-foreign-company-turkey-data-controller-representative/ · https://www.erdem-erdem.av.tr/en/insights/public-announcement-regarding-the-standard-contract-notification-module
- 152-FZ (consultant.ru, ed. del 26-7-2026): https://www.consultant.ru/document/cons_doc_LAW_61801/d44bdb356e6a691d0c72fef05ed16f68af0af9eb/ · localización 2025: https://www.comnews.ru/content/239935/2025-06-30/2025-w27/1009/1-iyulya-personalnye-dannye-rossiyan-nelzya-budet-khranit-za-rubezhom · https://konsugroup.com/en/news/new-requirements-personal-data-protection-russia-2025-07/ · 266-FZ: https://www.gorodissky.com/publications/articles/navigating-amendments-to-russian-personal-data-law/ · https://pgplaw.com/analytics-and-brochures/alerts/roskomnadzor-razyasnil-operatoram-poryadok-napravleniya-uvedomleniy-ob-obrabotke-personalnykh-dannykh/
- 236-FZ: https://www.unicon.ru/en/insights/publication/Overview_of_the_Federal_Law_No_236_FZ · 290-FZ: https://www.consultant.ru/document/cons_doc_LAW_511087/30b3f8c55f65557c253227a65b908cc075ce114a/
- Serbia: https://zuniclaw.com/en/data-protection-representative-for-serbia/ · https://cms.law/en/int/expert-guides/the-impact-of-gdpr-in-non-eu-countries/serbia
- Moldavia: https://www.dlapiperdataprotection.com/?t=law&c=MD · Montenegro: https://www.ronalegal.com/en/blog/montenegro-data-protection-law-133-2026-what-changes · Georgia: https://www.globallegalpost.com/lawoverborders/data-protection-law-guide-1072382791/georgia-273882423 · Kazajistán: https://www.morganlewis.com/-/media/files/publication/outside-publication/article/2024/data-localization-laws-overview-kazakhstan.pdf · Cáucaso: https://www.siberson.com/central-asia-caucasus-data-security-compliance.html
