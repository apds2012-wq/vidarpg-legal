# VIDA RPG · Leyes de América (EE. UU., Canadá, México, Hispanoamérica)

Investigación del 2-11-2026. Supuesto de partida (BRIEF.md): desarrollador persona física en España, sin establecimiento fuera de España, app para adultos en Google Play, sin cuentas, partida solo en el teléfono, ingresos y usuarios sin documentar. Política leída: `politica-privacidad-es.txt` (13-10-2026, v2.17.1).

Reglas de este informe: cada afirmación lleva su fuente y la fecha en que se consultó. Lo que no se pudo leer en una fuente oficial va marcado **NO VERIFICADO**. Cuando la fuente es un resumen de un bufete o el texto de un tercero que reproduce la ley (FindLaw, Cornell LII, bufetes), se dice así. Brasil (LGPD y CDC) queda fuera: va en otro informe (`br-src/`).

Advertencia: esto es investigación, no asesoría jurídica. Antes de publicar los cambios, que los revise un abogado con colegiación en la jurisdicción que importe.

---

## 0. Tabla resumen

| # | Ley · país | ¿Se aplica a VIDA hoy? | Umbral o condición clave | ¿Representante local? | Qué falta en la política o en los términos |
|---|---|---|---|---|---|
| 1 | **CalOPPA** (Cal. Bus. & Prof. Code §22575-22579), EE. UU.-CA | **Probablemente sí** (no tiene umbral; ver §1.1) | Operador de un servicio en línea que recoge PII de consumidores residentes en California | No | Una frase sobre cómo responde a **Do Not Track**; una frase expresa de que **terceros (Google AdMob)** pueden recoger datos de actividad entre apps y a lo largo del tiempo; un apartado «Residentes de California» |
| 2 | **CCPA/CPRA** (Cal. Civ. Code §1798.100 y ss.) | **No**, salvo que se pase un umbral | Ingresos brutos > **26.625.000 $** (desde el 1-1-2025) · o comprar, vender o **compartir** datos de ≥ 100.000 consumidores u hogares de CA · o ≥ 50 % de los ingresos por vender o compartir | No | Nada obligatorio. Opcional: una frase de que no se venden datos y de que la publicidad personalizada se puede rechazar |
| 3 | **Leyes de privacidad de otros estados** (VA, CO, CT, TX, OR, etc.) | **No**, por umbral. Ojo con Connecticut desde el 1-7-2026 (ver §3) | Ver la tabla del §3 | No | Nada obligatorio. Recomendado: una frase de que no se venden datos sensibles |
| 4 | **COPPA** (15 U.S.C. 6501-6506; 16 CFR 312) | **No**: la app no se dirige a menores de 13 años | Servicio dirigido a menores de 13 años, o **conocimiento real** de que se recogen datos de un menor de 13 años | No | Decir «menores de 13 años» de forma expresa y qué se hace al saber que un menor ha usado la app |
| 5 | **Ley de Renovación Automática de California** (ARL, §17600-17606, reforma AB 2863 en vigor desde el 1-7-2025) | **Sí** en lo que toca al vendedor (PRO mensual y anual con prueba gratuita) | Oferta de renovación automática o de paso de gratis a pago a un consumidor de CA | No | En los Términos y en la pantalla de compra: condiciones de la renovación antes de pagar, el precio y la frecuencia, cómo cancelar (Google Play) y una explicación de la prueba de 7 días. El **recordatorio anual** y el aviso de **cambio de precio** recaen en parte en Google Play: ver §5 |
| 6 | **Regla «Click-to-Cancel» de la FTC** (16 CFR 425, enmienda de 2024) | **No está en vigor**: la anuló el 8.º Circuito el 8-7-2025 | — | — | Nada nuevo. La FTC reabrió el proceso con un ANPRM (DOF de EE. UU., 13-3-2026) |
| 7 | **ROSCA** (15 U.S.C. 8401-8405) | **Sí** (venta por internet con opción negativa a consumidores de EE. UU.) | Cobro por renovación automática o paso de gratis a pago | No | Las mismas tres cosas: condiciones materiales antes de pedir los datos de pago, consentimiento expreso, un medio sencillo para cancelar. Google Play las cubre en buena parte; los Términos deberían decirlas |
| 8 | **Washington My Health My Data Act** (RCW 19.373) | **Dudoso**, riesgo bajo (ver §8) | Entidad que determina los fines y medios del tratamiento de **datos de salud del consumidor**; sin umbral (la pequeña empresa solo tuvo una fecha más tardía) | No | Recomendado: un apartado breve «Datos de salud del consumidor (Washington y Nevada)» con un enlace desde la página de inicio del sitio legal |
| 9 | **Nevada SB 370** (NRS 603A.400-603A.550) | Mismo análisis que Washington | Sin umbrales; en vigor desde el 31-3-2024 (resúmenes secundarios) | No | Lo mismo que el punto 8 |
| 10 | **PIPEDA**, Canadá | **Probablemente sí** (conexión real y sustancial: la app se ofrece a canadienses) | Organización que recoge datos personales en una actividad comercial | No (pero tiene que designar una **persona responsable**) | Nombre o **cargo** y **dirección** de la persona responsable (4.8.2 a); aviso de que los datos pueden **tratarse en EE. UU.** (Cloudflare, RevenueCat, Google) y quedar al alcance de sus autoridades; derecho a reclamar ante el **Commissariat à la protection de la vie privée du Canada (CPVP)** |
| 11 | **Ley 25 de Quebec** (Ley P-39.1) | **Dudoso** sin establecimiento; lo prudente es cumplir en lo barato | Ejercer una empresa en el sentido del Código Civil de Quebec | No | Título y medio de contacto de la **persona responsable de la protección de los datos personales**, publicados en el sitio; aviso de que los datos se pueden comunicar **fuera de Quebec**; derecho a reclamar ante la **Commission d'accès à l'information (CAI)** |
| 12 | **Carta de la lengua francesa**, Quebec (art. 55) | Dudoso; **ya se cumple de hecho** (hay política y términos en francés) | Contrato de adhesión con una persona de Quebec | — | Conviene que la versión francesa sea completa y equivalente |
| 13 | **LFPDPPP 2025**, México (DOF 20-3-2025, última reforma DOF 14-11-2025) | **Dudoso** para un extranjero sin medios en México (la ley no dice nada del ámbito territorial); lo prudente es cumplir | — | No en la ley | **Aviso de privacidad** con: identidad y **domicilio** del responsable, los datos (y cuáles son sensibles), las finalidades (separando las que necesitan consentimiento), cómo limitar el uso, los **derechos ARCO** y el plazo de 20 días, y cómo se avisa de los cambios. Autoridad: **Secretaría Anticorrupción y Buen Gobierno** |
| 14 | **LFPC**, México, art. 76 bis VIII-IX (DOF 12-12-2025, vigente desde el 13-12-2025) | **Sí** en las suscripciones a consumidores de México | Servicio en línea con cobros automáticos que se repiten | No | Informar de la periodicidad, el **importe** y la **fecha** del cobro; consentimiento expreso; **aviso de renovación al menos 5 días naturales antes**; cancelación inmediata |
| 15 | **Ley 25.326**, Argentina | Dudoso (la ley no tiene artículo de ámbito territorial; NO VERIFICADO); riesgo bajo | — | No | Finalidad y destinatarios, identidad y **domicilio** del responsable, derechos de acceso, rectificación y supresión (art. 6); la autoridad (AAIP) |
| 16 | **Ley 24.240**, Argentina (consumo) | **Sí** en las ventas a consumidores argentinos | Venta a distancia o electrónica | No | **Revocación en 10 días corridos, irrenunciable** (art. 34) y **baja por el mismo medio** (art. 10 ter). Hay tensión con la renuncia de la UE para el contenido digital: ver §15 |
| 17 | **Ley 21.719**, Chile (en vigor el **1-12-2026**) | **Sí desde el 1-12-2026** (art. 1° bis c: ofrecer bienes o servicios a titulares en Chile, aunque sea gratis) | — | **No se encontró** obligación de representante en el texto | Lista del art. 14 ter: política con fecha y versión, correo para solicitudes, categorías y destinatarios, bases de licitud e intereses legítimos, medidas de seguridad, derechos (incluida la **portabilidad**), derecho a reclamar ante la **Agencia de Protección de Datos Personales**, transferencias a terceros países y sus garantías, plazos de conservación, fuente, retirada del consentimiento y decisiones automatizadas |
| 18 | **Ley 19.496**, Chile (consumo), art. 3° bis b) | **Sí**, salvo exclusión expresa | Contrato electrónico | No | **Retracto de 10 días**, «a menos que el proveedor haya dispuesto expresamente lo contrario»: los Términos tienen que excluirlo de forma expresa o reconocerlo |
| 19 | **Ley 1581/2012** y **Decreto 1377/2013**, Colombia | **Dudoso** (art. 2: solo si el tratamiento ocurre en Colombia o lo imponen normas o tratados internacionales) | — | No | Si se aplica: el tratamiento y su finalidad, los derechos, la **identificación, dirección y teléfono** del responsable (art. 12) |
| 20 | **RNBD**, Colombia | **No** | Solo sociedades y entidades sin ánimo de lucro con activos > 100.000 UVT (Decreto 090/2018, **NO VERIFICADO** en el texto oficial) | — | — |
| 21 | **Ley 1480/2011**, Colombia (consumo) | Retracto: dudoso (excepción 1 del art. 47). Art. 50: **no** (solo proveedores en territorio nacional) | — | — | Retracto de 5 días hábiles; excepción si la prestación del servicio empezó con acuerdo del consumidor |
| 22 | **Ley 29733** y **DS 016-2024-JUS**, Perú (reglamento en vigor desde el 30-3-2025) | **Sí** según los resúmenes (alcanza a no domiciliados que ofrecen bienes o servicios en Perú) | — | **Sí, según bufetes**: un representante en Perú (artículo **NO VERIFICADO** en el texto oficial) | Nombrar al representante; derechos ARCO; autoridad (ANPD) |
| 23 | **Ley 18.331** y **Ley 19.670**, art. 37, Uruguay | **Sí** (oferta de bienes o servicios a habitantes de Uruguay) | — | Solo en el caso de medios en el país usados para tránsito (art. 37) | Lista del art. 13 A-G: finalidad, destinatarios, identidad y **domicilio**, derechos, **transferencias internacionales** |
| 24 | **LOPDP 2021**, Ecuador | **Probablemente sí** (art. 3.3, copia del art. 3.2 del RGPD) | — | **Apoderado especial**, según la SPDP (guía técnica de la Res. SPDP-SPDP-2024-0002-R); **NO VERIFICADO** si alcanza a quien no es empresa | Representante o apoderado; autoridad: **Superintendencia de Protección de Datos Personales** |
| 25 | **Ley 7593/2025**, Paraguay | **Todavía no** (en vigor 24 meses después de su publicación: ~noviembre de 2027) | Tratamiento de datos de personas en Paraguay | NO VERIFICADO | Prever un apartado para 2027 |
| 26 | Costa Rica (Ley 8968), Panamá (Ley 81 de 2019), Rep. Dominicana (Ley 172-13) | **NO VERIFICADO** el ámbito sobre extranjeros | — | NO VERIFICADO | — |
| 27 | Guatemala, Bolivia, Venezuela | **NO VERIFICADO**: no se encontró una ley general de protección de datos en vigor | — | — | — |

---

## 1. Estados Unidos (federal y California)

### 1.1 CalOPPA: Cal. Bus. & Prof. Code §22575-22579

**Fuente.** El sitio oficial leginfo.legislature.ca.gov respondió 403 a WebFetch y a curl el 2-11-2026. Se leyó el texto reproducido por FindLaw (codes.findlaw.com, «current as of January 1, 2026»), consultado el 2-11-2026. Hay que cotejarlo con leginfo antes de citarlo.

**A quién se aplica.** Al «operator» (§22577(c)): el dueño de un sitio web o servicio en línea comercial que recoge y mantiene información personal identificable (PII) de consumidores residentes en California que lo usan o lo visitan. **No hay umbral de ingresos ni de usuarios.** Una app es un «online service». Un desarrollador extranjero no está excluido.

**¿Recoge VIDA «PII» según el §22577(a)?** La PII es la información identificable de una persona concreta que el operador **recoge en línea de esa persona** y **mantiene de forma accesible**. Incluye nombre, dirección, correo, teléfono, número de la Seguridad Social, «cualquier otro identificador que permita el contacto físico o en línea de una persona concreta» y la información que se mantiene junto a esos identificadores.

| Dato | ¿Lo recoge y mantiene el desarrollador? | ¿Es PII según el §22577? |
|---|---|---|
| Partida, hábitos, Health Connect | No: se queda en el teléfono | No |
| Consulta al Coach | La procesa el Worker y no la guarda | No (no se mantiene) |
| IP | Huella salada con la fecha, durante un día | Dudoso: una IP se puede ver como un identificador de contacto en línea; la política reconoce que la huella de una IPv4 se puede revertir |
| ID aleatorio de instalación | Huella diaria | Dudoso: no sirve para contactar a nadie |
| ID anónimo de RevenueCat + nº de pedido GPA + saldo | Sí, hasta 24 meses | Dudoso: no sirve para contactar a la persona, pero se mantiene vinculado a ella |
| **Correo** de quien escribe a vidarpgapp@gmail.com | Sí (bandeja de entrada) | **Sí**: es un correo. Pero se recibe por correo electrónico, no por la app |
| Identificador de publicidad y datos de AdMob | Los recoge **Google** a través del SDK integrado en la app | Es tercero; la ley pide revelarlo (§22575(b)(6)) |

**Conclusión: probablemente sí se aplica.** Lo prudente es tratarla como aplicable por tres razones: los identificadores que se mantienen (ID de RevenueCat con el número de pedido), la IP y el SDK de un tercero dentro de la app. Además, cumplirla cuesta poco. Que el apartado (b)(5) entre en juego depende de si el operador recoge datos de actividad entre sitios a lo largo del tiempo. VIDA no lo hace por sí mismo, pero AdMob sí, dentro de la app.

**Contenido obligatorio (§22575(b), resumen de FindLaw) y estado de la política actual:**

1. Categorías de PII y de terceros con los que se comparte: **cumplido** (secciones 8, 9, 11 y 12).
2. Proceso para revisar y pedir cambios, si existe: **cumplido** (sección 15).
3. Cómo se avisa de los cambios importantes: **cumplido a medias** (sección 18 dice dónde se publica, pero no «cómo se avisa»).
4. Fecha de efecto: **cumplido** («Última actualización»). Sería mejor escribir «Fecha de efecto».
5. Cómo responde a las señales **Do Not Track**: **FALTA**.
6. Si otros terceros pueden recoger datos de la actividad en línea del usuario a lo largo del tiempo y entre sitios: **implícito** en la sección 9, **sin decirlo con esas palabras**.

**Publicación visible («conspicuously post», §22577(b)):** en una app basta con un acceso razonable (Más → Privacidad y la ficha de Play). **Cumplido.** Plazo: solo hay infracción si no se corrige en los **30 días** siguientes al aviso de incumplimiento (§22575(a)).

### 1.2 CCPA/CPRA: Cal. Civ. Code §1798.140(d)

- **Umbral de ingresos.** El umbral de 25 M$ se actualizó a **26.625.000 $** con efecto desde el **1-1-2025** («publicado el 17-12-2024»). Fuente: CPPA, cppa.ca.gov/regulations/cpi_adjustment.html, consultada el 2-11-2026. La revisión es «cada año impar»; **no hay cifra publicada para 2027 (NO VERIFICADO)**. La cifra de 2026 es la misma de 2025.
- **Los otros dos umbrales** (100.000 consumidores u hogares; 50 % de los ingresos por vender o compartir) son los del texto de la CPRA. **NO VERIFICADO** su redacción exacta en leginfo (403).
- **Análisis.** El desarrollador no llega a 26,6 M$. Sin vender datos, el tercer umbral no se cumple. **Cuidado con el segundo**: «compartir» incluye dar datos para **publicidad comportamental entre contextos**. Si AdMob sirve anuncios personalizados a ≥ 100.000 consumidores de California en un año, podría discutirse que el desarrollador «comparte» sus datos. Hoy no se sabe el volumen, así que **se supone que no aplica**. Medida barata si crece: servir en EE. UU. anuncios no personalizados o respetar la señal GPC.
- **Si no aplica, la CCPA no impone nada.**

### 1.3 Otras leyes estatales de privacidad (resumen)

Fuentes: Virginia, texto oficial (law.lis.virginia.gov, §59.1-576 A, consultado el 2-11-2026). Indiana, Kentucky y Rhode Island: tabla de PBN Law «Applicability for the 2026 class» (1-8-2025). Connecticut: resúmenes de Hunton, FPF y Covington (2025) sobre la SB 1295, sin leer la Public Act 25-113. Texas: resúmenes de la Texas State Law Library, la Fiscalía de Texas y Hunton; **§541.107 sin leer en el texto oficial**. El resto sale del cuadro de Troutman Pepper (enero de 2025) y de lo que se recuerda de los textos legales: **NO VERIFICADO en el texto oficial de cada estado**.

| Estado | Se aplica si (por año natural, consumidores de ese estado) | ¿VIDA? |
|---|---|---|
| Virginia | ≥ 100.000 · o ≥ 25.000 y > 50 % de los ingresos por venta de datos | No |
| Colorado | ≥ 100.000 · o ≥ 25.000 y ingresos o descuentos por venta (NO VERIFICADO) | No |
| **Connecticut** (desde el **1-7-2026**, SB 1295) | ≥ **35.000** · o **cualquier tratamiento de datos sensibles** (salvo los usados solo para un pago) · o cualquier venta | **Revisar**: ver la nota de abajo |
| Utah | Ingresos ≥ 25 M$ **y** (≥ 100.000 o ≥ 25.000 y > 50 %) (NO VERIFICADO) | No |
| **Texas** (TDPSA, 1-7-2024) | Hace negocios en Texas, trata datos y **no es pequeña empresa según la SBA** | No (pequeña empresa). **Pero una pequeña empresa no puede vender datos sensibles sin consentimiento** (§541.107; NO VERIFICADO en el texto oficial). VIDA no vende datos |
| Nebraska | Como Texas (NO VERIFICADO) | No |
| Minnesota | ≥ 100.000 · o ≥ 25.000 y > 25 %; pequeña empresa de la SBA exenta salvo para vender datos sensibles (NO VERIFICADO) | No |
| Oregón | ≥ 100.000 · o ≥ 25.000 y ≥ 25 % (NO VERIFICADO) | No |
| Montana | Bajado a ≥ 25.000 · o ≥ 15.000 y > 25 % desde el 1-10-2025 (NO VERIFICADO) | No |
| Delaware, New Hampshire, Maryland | ≥ 35.000 · o ≥ 10.000 y > 20 % (DE, MD) / > 25 % (NH) (NO VERIFICADO) | No |
| Iowa, Tennessee, Nueva Jersey | Iowa ≥ 100.000 / 25.000 y 50 %; Tennessee ingresos > 25 M$ y ≥ 175.000; Nueva Jersey ≥ 100.000 / 25.000 con venta (NO VERIFICADO) | No |
| Indiana (1-1-2026) | ≥ 100.000 · o ≥ 10.000 y > 20 % | No |
| Kentucky (1-1-2026) | ≥ 100.000 · o ≥ 25.000 y > 50 % | No |
| Rhode Island (1-1-2026) | ≥ 35.000 (salvo los que solo sirven para un pago) · o ≥ 25.000 y > 50 % | No |

**Nota sobre Connecticut y los datos sensibles.** Desde el 1-7-2026, quien «controle o trate» **cualquier dato sensible** de residentes de Connecticut queda sujeto a la ley, sin umbral (resúmenes de la SB 1295). Hay dos casos en VIDA:

- **(a)** Los datos de **Health Connect**, los vicios y las caídas se tratan **solo en el teléfono**. ¿Los «trata» el desarrollador? El código es suyo, pero él no los recibe ni puede acceder. La lectura más natural es que **no hay tratamiento por el responsable** (no hay acceso ni conservación). Ninguna fuente lo resuelve: **NO VERIFICADO**.
- **(b)** El Coach **sí** recibe, de paso y sin guardarlo, «los vicios registrados» con su categoría y frecuencia (sección 8 de la política). Eso puede rozar los «datos de salud» (consumo de tabaco y alcohol, conducta sexual compulsiva) si se pueden vincular a una persona (IP o ID de instalación). **Riesgo bajo-medio.** Ver la propuesta del §8.

### 1.4 COPPA

- **Ámbito.** Operadores de servicios **dirigidos a menores de 13 años**, u operadores de servicios generales con **conocimiento real** de que recogen datos personales de un menor de 13 años. Fuente: FTC, ftc.gov/legal-library/browse/rules/childrens-online-privacy-protection-rule-coppa, consultada el 2-11-2026.
- **Reforma.** Publicada en el Federal Register el **22-4-2025** (90 FR 16970), en vigor el 23-6-2025, con cumplimiento obligatorio desde el **22-4-2026**. Fuentes secundarias: Hunton, Mondaq y NatLawReview, 2025-2026.
- **VIDA.** App para adultos, que no se dirige a menores. Sin conocimiento real, **COPPA no se aplica**. Riesgo: AdMob. Si un día la app se marca como dirigida a familias en Play, cambia todo.
- **Qué añadir.** «VIDA RPG no se dirige a menores de 13 años (ni a menores de 14 años en España) y no recoge a sabiendas datos de ellos. Si sabemos que un menor nos ha escrito o ha comprado créditos, borraremos lo que tengamos de él en el servidor.»

### 1.5 Ley de Renovación Automática de California (ARL, §17600-17606; AB 2863)

**Fuentes.** Leginfo devolvió 403. Se usaron Latham & Watkins, alerta n.º 3301 del 10-10-2024 (PDF leído), y Fenwick (2025), consultados el 2-11-2026. **El texto vigente del §17602 no se leyó en la fuente oficial: NO VERIFICADO.**

- **AB 2863** (cap. 515, Stats. 2024, firmada el 24-9-2024). Se aplica a los contratos celebrados, modificados o prorrogados **desde el 1-7-2025**.
- **Novedades:**
  - incluye el **paso de gratis a pago** (la prueba de 7 días del plan anual);
  - pide el **consentimiento expreso y afirmativo** a las condiciones de la renovación, y guardar la prueba **3 años** o 1 año tras el fin del contrato, lo que sea más largo;
  - el aviso inicial va **antes de confirmar los datos de facturación**, con el importe o el rango y la frecuencia;
  - **recordatorio anual** en los contratos anuales (producto, frecuencia y medio de cancelación);
  - aviso de **cambio de precio** entre **7 y 30 días** antes;
  - **cancelación por el mismo medio** (en línea si se contrató en línea);
  - prohibido tergiversar hechos materiales;
  - las ofertas para retener al cliente solo con un botón visible de «cancelar».
- El aviso para pruebas de **más de 31 días** (3 a 21 días antes de que acaben) venía de la AB 390 (2021). **NO VERIFICADO** si sigue en el texto vigente. A VIDA no le afecta: su prueba es de **7 días**.

**¿Se aplica a una suscripción vendida y renovada por Google Play?** La ARL obliga a la «empresa que hace la oferta» a un consumidor de California. El desarrollador hace la oferta (pantalla de PRO), aunque cobre y cancele Google. **No se encontró ninguna excepción para las tiendas de aplicaciones (NO VERIFICADO).** En la práctica:

- **Cancelación en línea:** la da Google Play (Centro de suscripciones). La política de Play exige además un acceso a la gestión o cancelación **dentro de la app** (Play Console Help, respuesta 9900533, consultada el 2-11-2026). Revisar que exista un enlace en Ajustes/PRO a `play.google.com/store/account/subscriptions`.
- **Consentimiento expreso:** lo recoge la hoja de compra de Google. Pero la ARL exige que las **condiciones** se muestren de forma clara y visible **antes**, en la pantalla de la app.
- **Recordatorio anual y aviso de cambio de precio:** **NO VERIFICADO** si Google Play envía el recordatorio anual que pide la ley. Play sí exige a los desarrolladores un aviso dentro de la app **30 días antes** de una subida de precio (Play Console Help). Como el desarrollador no tiene el correo del usuario, lo único que puede hacer él mismo es un **aviso dentro de la app** antes de la renovación anual. Eso cabe en las notificaciones locales, sin datos.

**Qué deben decir los Términos** (y, en resumen, la pantalla de PRO):

1. Que el plan **se renueva automáticamente** al final de cada periodo hasta que se cancele.
2. El **precio** y la **frecuencia** (5,99 €/mes; 39,99 €/año), con impuestos y en la moneda que muestre la tienda.
3. Que la prueba de **7 días** pasa a pago si no se cancela **antes de que termine**, y **cuándo** se cobrará.
4. **Cómo cancelar**: Google Play → Pagos y suscripciones → Suscripciones, con enlace directo; también desde Ajustes de la app.
5. Que al cancelar se conserva PRO **hasta el final del periodo pagado**.
6. Cómo se avisará de un **cambio de precio**.
7. Contacto.

### 1.6 Regla «Click-to-Cancel» de la FTC

- El **8.º Circuito la anuló entera** el **8-7-2025** (*Custom Communications, Inc. v. FTC*), por razones de procedimiento: faltó el análisis preliminar de impacto del §22 de la FTC Act. Desapareció la fecha de cumplimiento del **14-7-2025**. Fuentes: Greenberg Traurig y Sheppard Mullin (julio de 2025).
- Sigue en vigor la regla de 1973/2010, solo para los planes con aviso previo.
- La FTC publicó un **ANPRM** (aviso previo de propuesta de reglamento): nota de prensa del 11-3-2026, Federal Register del **13-3-2026** (doc. 2026-04952), comentarios hasta el 13-4-2026. Fuentes: ftc.gov y federalregister.gov, consultadas el 2-11-2026. **No hay nueva regla vinculante** (no se encontró propuesta posterior: NO VERIFICADO a fecha de hoy).

### 1.7 ROSCA: 15 U.S.C. 8403

**Fuente:** Cornell LII, consultada el 2-11-2026.

Es ilegal cobrar en una venta por internet con «opción negativa» salvo que se cumplan tres cosas:

1. revelar **todas las condiciones materiales** de forma clara y visible **antes** de recoger la información de facturación;
2. obtener el **consentimiento expreso e informado** antes de cobrar;
3. dar **mecanismos sencillos** para parar los cobros.

**Se aplica** a ventas a consumidores de EE. UU. La FTC puede actuar contra conductas extranjeras que afecten a consumidores de EE. UU. (US SAFE WEB Act, 15 U.S.C. 45(a)(4); **NO VERIFICADO** en el texto). Las medidas del §1.5 cubren también ROSCA.

### 1.8 Washington My Health My Data Act (RCW 19.373)

**Fuente:** app.leg.wa.gov, RCW 19.373.010 y .020, consultadas el 2-11-2026.

- **«Recoger»** es «comprar, alquilar, **acceder**, conservar, recibir, adquirir, inferir, derivar o **tratar de cualquier otro modo**» datos de salud del consumidor (.010(5)). **«Tratar»** es cualquier operación (.010(20)).
- **«Entidad regulada»** es la entidad que hace negocios en Washington o dirige productos a consumidores de Washington y que **determina los fines y medios** de recogerlos o tratarlos (.010(23)).
- La **pequeña empresa** (< 100.000 consumidores, o < 50 % de los ingresos y < 25.000 consumidores; .010(28)) **no está exenta**: solo tuvo una fecha de aplicación más tardía.
- **Datos de salud del consumidor**: información **vinculada o razonablemente vinculable** a un consumidor que identifica su estado de salud (.010(8)).

**Análisis para VIDA.**

- **Health Connect** (pasos, distancia, carreras) se trata solo en el teléfono. El desarrollador ni lo recibe ni puede acceder. La lectura razonable es que **no los «recoge» como entidad**: no hay acceso, conservación ni recepción suya.
- Pero «tratar de cualquier otro modo», junto con «determinar los medios» (su código), es muy amplio, y **no se encontró ninguna guía de la Fiscalía de Washington** sobre el tratamiento solo en el dispositivo (**NO VERIFICADO**).
- El caso del Coach (los vicios que viajan sin guardarse, junto a una IP) es el más expuesto.
- **Riesgo bajo.** Medida barata: el apartado que pide .020 (categorías recogidas y finalidad, fuentes, categorías compartidas y destinatarios, cómo ejercer los derechos), con **un enlace visible desde la página de inicio** del sitio legal (.020(1)(b)).

### 1.9 Nevada SB 370 (NRS 603A.400-603A.550)

Sin umbrales; en vigor desde el 31-3-2024. Exige una política de datos de salud, consentimiento para recoger o compartir y autorización escrita para vender. Fuentes secundarias: WilmerHale (14-6-2023) y DataGrail; **NO VERIFICADO en leg.state.nv.us**. Mismo análisis y la misma medida que Washington.

### 1.10 Otras

California «Shine the Light» (Civ. Code §1798.83): se aplica a empresas con **20 o más empleados** que comparten datos con terceros para su marketing directo. **NO VERIFICADO**; un autónomo sin empleados no entra.

---

## 2. Canadá

### 2.1 PIPEDA (L.C. 2000, c. 5)

- **Ámbito extraterritorial.** El CPVP aplica el criterio de la **conexión real y sustancial** con Canadá. La presencia física no hace falta. Factores (*A.T. v. Globe24h.com*, 2017 FC 114, según el resumen del CPVP): el **público objetivo**, el origen del contenido, la ubicación del operador y la del servidor. El CPVP lo usó contra Globe24h (2015-002), Clearview AI (2021-001), OpenAI (2026-002) y X/xAI (2026-004). Fuente: priv.gc.ca, consultada el 2-11-2026.
- **VIDA.** La app se ofrece en Play Canadá, en inglés y francés, con compras en dólares canadienses: **probablemente hay conexión**. Aun así, el volumen de datos que conserva el desarrollador es mínimo.
- **Principios del Anexo 1** (laws-lois.justice.gc.ca, P-8.6, página 7, consultada el 2-11-2026):
  - **4.1**: la organización designa a la persona o personas responsables del cumplimiento. **4.1.2**: su identidad se comunica a quien la pida. **4.1.3**: la organización responde de los datos que pasa a terceros para tratarlos y tiene que asegurar una **protección comparable** por contrato.
  - **4.8.2**: hay que poner a disposición (a) el **nombre o cargo y la dirección** de la persona responsable, a la que se envían quejas y preguntas; (b) cómo acceder a los datos; (c) qué tipos de datos se tienen y para qué; (d) folletos u otra información; (e) qué datos se dan a organizaciones vinculadas.
- **Transferencias.** Las directrices del CPVP de 2009 sobre tratamiento transfronterizo piden avisar de que los datos pueden tratarse en otro país y quedar al alcance de sus tribunales y autoridades. El sitio devolvió 503: **NO VERIFICADO hoy**.
- **Qué falta.** Una **dirección** del responsable (hoy solo pone «España» y un correo), un **cargo** («responsable de privacidad: el desarrollador, Alex Vida»), el aviso de **tratamiento en EE. UU.** con acceso posible de sus autoridades, y la vía de **queja ante el CPVP**.

### 2.2 Quebec: Ley sobre la protección de los datos personales en el sector privado (P-39.1, reformada por la Ley 25)

**Fuente.** legisquebec.gouv.qc.ca devolvió 403 (WebFetch y curl). Lo que sigue sale de resúmenes secundarios (Gowling WLG 2022, CookieYes, Clym) y de lo que se recuerda del texto: **NO VERIFICADO literalmente**.

- **Ámbito.** Quien «ejerce una empresa» en el sentido del art. 1525 del Código Civil de Quebec. Unas fuentes dicen que alcanza a quien trata datos de personas en Quebec aunque no esté allí; otras lo atan a ejercer la actividad en Quebec. **No hay una respuesta oficial** para un extranjero sin establecimiento: **dudoso**.
- **Art. 3.1.** La persona con la máxima autoridad es la **responsable de la protección de los datos personales**. Puede delegar por escrito. Su **título y sus datos de contacto se publican en el sitio web**.
- **Art. 8.** Al recoger los datos hay que informar de la finalidad, los medios, los derechos de acceso y rectificación y el de **retirar el consentimiento**, los terceros y la **posibilidad de que los datos se comuniquen fuera de Quebec**.
- **Art. 8.1.** Hay que avisar **antes** si se usa tecnología que permite **identificar, localizar o perfilar**, y de cómo activarla. Es pertinente para el ID de publicidad de AdMob.
- **Art. 8.2.** Política publicada **en el sitio** en términos claros.
- **Art. 17.** Antes de comunicar datos **fuera de Quebec**, una **evaluación de impacto** (EFVP) y un acuerdo escrito.
- **Qué falta (medida barata).** Título y contacto de la persona responsable; aviso de comunicación fuera de Quebec (EE. UU.: Cloudflare, RevenueCat, Google); aviso del art. 8.1 sobre AdMob (ya está en la sección 9, sin nombrar Quebec); vía de queja ante la **CAI**. La EFVP del art. 17 sería un documento interno (**no hay que publicarlo**).

### 2.3 Carta de la lengua francesa (art. 55, Ley 96, desde el 1-6-2023)

En un contrato de adhesión, hay que presentar **primero la versión francesa** y gratis; la de otro idioma solo obliga si la persona la pide de forma expresa tras ver la francesa. Hay una excepción para los contratos «en relaciones fuera de Quebec». Su alcance para unos términos en línea **no está resuelto**. Fuentes: Norton Rose Fulbright, Gowling (2023), Lavery. **NO VERIFICADO en el texto oficial.**

**VIDA** tiene la política y los términos en francés (sitio legal ES/EN/PL/FR/DE/IT/RU/PT): **en la práctica ya cumple**. Conviene que, con el sistema en francés, la app abra la versión FR.

---

## 3. México

### 3.1 LFPDPPP nueva (DOF 20-3-2025; última reforma DOF 14-11-2025)

**Fuente:** texto vigente de diputados.gob.mx/LeyesBiblio/pdf/LFPDPPP.pdf, leído el 2-11-2026.

- **Ámbito.** Art. 1: «de observancia general en todo el territorio nacional». Excluye solo a las sociedades de información crediticia y el uso **exclusivamente personal**. **La ley no tiene artículo de ámbito extraterritorial.** El reglamento de 2011 (art. 4) alcanzaba al responsable no establecido que usara medios situados en México. **NO VERIFICADO** si hay reglamento nuevo y qué dice. Por eso, para un desarrollador español sin medios en México la aplicación es **dudosa**.
- **Autoridad.** «Secretaría: Secretaría Anticorrupción y Buen Gobierno» (art. 2, fr. XV), que sustituye al INAI.
- **Aviso de privacidad** (art. 15). Contenido mínimo: I identidad y **domicilio** del responsable; II los datos tratados, **marcando los sensibles**; III las finalidades, **separando las que necesitan consentimiento**; IV las opciones para **limitar el uso o la divulgación**; V cómo ejercer los **derechos ARCO**; VI cómo se avisa de los cambios. Por medios electrónicos, un aviso **simplificado** (fracciones I-IV) con enlace al integral (art. 16 II).
- **ARCO.** Acceso, rectificación, cancelación y oposición (arts. 21-25). Respuesta en un **máximo de 20 días** (art. 31). Hay que designar a una persona o departamento de datos personales que tramite las solicitudes (art. 30, según la línea 489 del texto).
- **Datos sensibles.** Consentimiento expreso (art. 8).
- **Transferencias.** El art. 36 prevé casos sin consentimiento, por ejemplo una transferencia necesaria por un contrato en interés del titular.
- **Qué falta.** Una sección «México» con el formato de aviso de privacidad: el **domicilio** del responsable (hoy no hay dirección postal), los datos sensibles por su nombre (vicios y caídas en el teléfono; lo que viaja al Coach), las finalidades por separado, «derechos ARCO» con ese nombre y el **plazo de 20 días**, y la autoridad.

### 3.2 Ley Federal de Protección al Consumidor (LFPC; última reforma DOF 12-12-2025)

**Fuente:** diputados.gob.mx/LeyesBiblio/pdf/LFPC.pdf, leído el 2-11-2026.

- **Art. 76 bis** (transacciones por medios electrónicos):
  - III: dar **domicilio físico, números telefónicos** y otros medios de reclamación **antes** de la transacción;
  - V: informar de las condiciones, costes y cargos;
  - **VIII** (añadida el 12-12-2025): informar «de forma clara, destacada y accesible» de los **cobros automáticos que se repiten**, con su **periodicidad, monto y fecha de cobro**, con **consentimiento expreso e informado**, y, si hay renovación automática, **«notificar al menos con cinco días naturales de anticipación»** y permitir cancelar sin penalización;
  - **IX**: mecanismos para **cancelar de inmediato** la suscripción.
- **Vigencia:** desde el **13-12-2025** (transitorio único: al día siguiente de su publicación).
- **Art. 56.** Revocación en **5 días hábiles**, pero dentro del capítulo de **ventas a domicilio o fuera del establecimiento** (arts. 51-56). Que se aplique a una compra dentro de la app es **dudoso**. Para servicios no se aplica si la prestación está a 10 días hábiles o menos de la orden.
- **¿Se aplica a VIDA?** La LFPC alcanza a los proveedores que venden a consumidores en México. Que se pueda hacer cumplir frente a un extranjero es otra cuestión. **Riesgo real**: el aviso de 5 días antes de la renovación (fr. VIII). Google Play no lo garantiza (**NO VERIFICADO**) y el desarrollador no tiene el correo. **Solución: un aviso local dentro de la app 5 días antes de la renovación**, sin datos y con un enlace para cancelar.
- **NOM-151** (conservación de mensajes de datos): **NO VERIFICADO** que se aplique; no se investigó.

---

## 4. Hispanoamérica

### 4.1 Argentina

- **Ley 25.326** (Infoleg, texto actualizado, leído el 2-11-2026):
  - **art. 6**: informar antes, de forma expresa y clara, de (a) la finalidad y los destinatarios, (b) la existencia del archivo y la **identidad y domicilio** del responsable, (c) si responder es obligatorio u opcional, (d) las consecuencias, (e) los derechos de acceso, rectificación y supresión;
  - **art. 12**: prohíbe transferir a países sin protección adecuada (las excepciones no cubren el caso de un proveedor de EE. UU.; **NO VERIFICADO** cómo trata la AAIP las cláusulas tipo);
  - **art. 21**: inscriben en el registro las bases **públicas** y las **privadas destinadas a dar informes**. **Lectura**: una base privada que no da informes a terceros no estaría obligada por este artículo; hay una práctica más amplia de la AAIP (**NO VERIFICADO**). Para un extranjero, **NO VERIFICADO**.
  - **La ley no tiene artículo de ámbito territorial** (no se encontró en el texto).
- La **leyenda de la AAIP** (Disposición DNPDP 10/2008) **fue derogada** por la Resolución AAIP 14/2018 (fuente: argentina.gob.ar, normativa). **No hace falta ponerla.**
- **Ley 24.240** (Infoleg, leída el 2-11-2026):
  - **art. 33**: la venta por medios electrónicos es «venta por correspondencia y otras»;
  - **art. 34**: **revocación de 10 días corridos** desde la celebración, «**no puede ser dispensada ni renunciada**», y hay que informarla por escrito «en forma clara y notoria»;
  - **art. 10 ter**: **baja por el mismo medio** con el que se contrató;
  - **art. 35**: prohíbe cargos automáticos por algo que no se pidió.
- **Conflicto.** Los Términos de VIDA aplican la renuncia de la UE (consentimiento para el contenido digital y los consumibles). Para un consumidor argentino, el art. 34 la hace **irrenunciable**. Puede haber excepciones en el **Código Civil y Comercial, art. 1116** (contenido digital descodificado o descargado), pero **NO VERIFICADO**: no se leyó. **Propuesta**: reconocer en los Términos que las leyes de consumo del país del usuario pueden dar derechos que no se pueden excluir, y aceptar las devoluciones en esos plazos cuando la ley lo exija. Google Play tiene su propia política de reembolsos.

### 4.2 Chile

- **Ley 21.719** (leychile.cl, XML de la norma 1209272, versión del 5-2-2026, leída el 2-11-2026), que reforma la Ley 19.628:
  - **Vigencia** «el día primero del mes vigésimo cuarto» tras su publicación (DO del 13-12-2024), es decir, el **1-12-2026**.
  - **Art. 1° bis c)**: se aplica al responsable **no establecido** cuando sus tratamientos estén destinados a **ofrecer bienes o servicios a titulares en Chile**, «independientemente de si a éstos se les requiere un pago», o a monitorear su comportamiento. **VIDA está dentro.**
  - **Representante**: **no se encontró** en el texto ninguna obligación de designar representante para responsables extranjeros (búsqueda de «representante» y «designar»).
  - **Art. 14 ter** (deber de información y transparencia): hay que tener **permanentemente a disposición del público, en su sitio web**: (a) la política con **fecha y versión**; (b) la identificación del responsable y de su representante legal, y del encargado de prevención si lo hay; (c) el **domicilio postal, correo** o formulario para las solicitudes; (d) las categorías de datos, el universo de personas, los destinatarios, las finalidades, la **base de licitud** y, si es interés legítimo, **cuál**; (e) la política y las **medidas de seguridad**; (f) los derechos de acceso, rectificación, supresión, oposición y **portabilidad**; (g) el derecho a **recurrir ante la Agencia**; (h) las **transferencias** a terceros países y si son adecuados o con qué garantías; (i) el **periodo de conservación**; (j) la **fuente** de los datos; (k) la **retirada del consentimiento**; (l) las **decisiones automatizadas** y la lógica aplicada.
  - **Art. 4°**: derechos de acceso, rectificación, supresión, oposición, portabilidad y bloqueo.
  - **Menores**: niños son los menores de 14 años; los datos sensibles de adolescentes menores de 16 años necesitan el consentimiento de los padres.
- **Ley 19.496** (leychile.cl, norma 61438; el XML trae una **fechaVersión del 20-4-2021**: **puede no ser la versión consolidada vigente**):
  - **art. 3° bis b)**: **retracto de 10 días** en contratos electrónicos, «**a menos que el proveedor haya dispuesto expresamente lo contrario**»;
  - si no se envía la confirmación escrita del art. 12 A, el plazo pasa a **90 días**.
  - **Propuesta**: una cláusula expresa en los Términos (en la línea de la renuncia de la UE para el contenido digital), mostrada antes de comprar.

### 4.3 Colombia

- **Ley 1581/2012** (Secretaría del Senado, basedoc, leída el 2-11-2026; funcionpublica.gov.co devolvió 503 y error de certificado):
  - **art. 2**: se aplica al tratamiento **en territorio colombiano** o cuando al responsable **no establecido** «le sea aplicable la legislación colombiana en virtud de normas y tratados internacionales». Para un desarrollador en España, **dudoso**. La SIC ha sostenido una interpretación amplia cuando se recogen datos en Colombia (**NO VERIFICADO**: no se leyó ninguna resolución).
  - **art. 12**: informar del tratamiento y su finalidad, de que responder sobre datos sensibles es **opcional**, de los derechos, y de la **identificación, dirección física o electrónica y teléfono** del responsable.
- **Decreto 1377/2013** (compilado en el Decreto 1074/2015): política de tratamiento y aviso de privacidad. **NO VERIFICADO**: no se leyó.
- **RNBD**: obligatorio solo para sociedades y entidades sin ánimo de lucro con **activos > 100.000 UVT** (Decreto 090/2018). **NO VERIFICADO**: no se leyó, pero en cualquier caso una persona física no entra.
- **Ley 1480/2011** (leída el 2-11-2026):
  - **art. 47**: **retracto de 5 días hábiles** en ventas a distancia. Excepción 1: los «contratos de prestación de servicios cuya prestación haya comenzado con el acuerdo del consumidor». Devolución en 15 días en el comercio electrónico (Ley 2439/2024).
  - **art. 50** (deberes del comercio electrónico): solo para proveedores «**ubicados en el territorio nacional**», así que **no alcanza a VIDA**.

### 4.4 Perú

- **Ley 29733** y su reglamento nuevo, el **DS 016-2024-JUS** (publicado el 30-11-2024, **en vigor el 30-3-2025**), según CMS y Pérez-Llorca, consultados el 2-11-2026:
  - alcanza a los **no domiciliados** que ofrecen bienes o servicios a personas en Perú o las perfilan;
  - **obliga a designar un representante en Perú**, contacto de la ANPD, que puede aparecer en la política de privacidad;
  - el **oficial de datos personales** solo es obligatorio en el sector público, en el tratamiento a gran escala o con datos sensibles;
  - aviso de brechas.
  - **Artículos y texto oficial NO VERIFICADOS** (lpderecho.pe devolvió 403; El Peruano no se consultó).
- **Consumo (Ley 29571)**: **NO VERIFICADO** si hay un retracto general en el comercio electrónico.
- **Riesgo práctico** si no se nombra representante: bajo para un autónomo extranjero con pocos datos, pero **el incumplimiento es formal**.

### 4.5 Uruguay

- **Ley 18.331** (IMPO, leída el 2-11-2026):
  - **art. 13**: informar de (A) la finalidad y los destinatarios, (B) la existencia de la base y la **identidad y domicilio** del responsable, (C) si responder es obligatorio u opcional, en especial sobre datos sensibles, (D) las consecuencias, (E) los derechos de los arts. 14-16, (F) **la existencia o no de transferencias internacionales**, (G) las decisiones automatizadas;
  - **art. 29**: **toda base privada se inscribe** en el registro de la URCDP.
- **Ley 19.670, art. 37** (IMPO, leída el 2-11-2026): se aplica al responsable no establecido si el tratamiento tiene que ver con la **oferta de bienes o servicios a habitantes de la República** o con el análisis de su comportamiento. El **representante con domicilio** en Uruguay solo se pide en el caso de **medios en el país usados para tránsito**. **VIDA está dentro.** **NO VERIFICADO** si la inscripción del art. 29 se exige a un responsable extranjero (Decreto 64/020).

### 4.6 Ecuador

- **LOPDP** (RO del 26-5-2021). **Art. 3.3**: tratamiento de datos de **titulares que residen en Ecuador** por un responsable no establecido allí, cuando ofrece bienes o servicios o controla su comportamiento (gob.ec, según los resultados; la UCE señala que es copia del art. 3.2 del RGPD).
- La **SPDP** registra **apoderados especiales** de responsables no domiciliados, con residencia y domicilio en Ecuador (Res. SPDP-SPDP-2024-0002-R; gob.ec/spdp/tramites/registro-apoderados-especiales).
- **NO VERIFICADO**: si es obligatorio para todo responsable extranjero o solo para algunos, y si alcanza a una persona física.

### 4.7 Paraguay

- **Ley 7593/2025** «De protección de datos personales», promulgada el 27/28-11-2025 (BACN, bacn.gov.py; Ferrere; EY Paraguay).
- En vigor **24 meses después de su publicación**, hacia **noviembre de 2027**. Según EY, alcanza a responsables de fuera que traten datos de personas en Paraguay.
- **Artículos NO VERIFICADOS.**

### 4.8 Resto (una línea cada uno)

- **Costa Rica**: Ley 8968 (PRODHAB). Ámbito sobre extranjeros e inscripción: **NO VERIFICADO**.
- **Panamá**: Ley 81 de 2019 (ANTAI). Ámbito sobre extranjeros: **NO VERIFICADO**.
- **República Dominicana**: Ley 172-13. **NO VERIFICADO**.
- **Guatemala, Bolivia y Venezuela**: **NO VERIFICADO**. No se encontró una ley general de datos personales en vigor; puede haber protección constitucional (hábeas data).
- **El Salvador, Honduras y Nicaragua**: no investigados.

### 4.9 Retracto en compras a distancia: resumen y aplicación a una compra dentro de la app

| País | Plazo | ¿Se puede excluir? | ¿Se aplica a una compra dentro de la app por Google Play? | Fuente |
|---|---|---|---|---|
| Argentina | 10 días corridos (art. 34 Ley 24.240) | **No** («no puede ser dispensada ni renunciada») | Probablemente sí: venta electrónica a un consumidor. Excepciones del Código Civil y Comercial para el contenido digital: NO VERIFICADO | Infoleg, 2-11-2026 |
| Chile | 10 días (art. 3° bis b Ley 19.496) | **Sí**, «si el proveedor dispone expresamente lo contrario» | Sí, salvo exclusión expresa | leychile, versión de 2021 |
| Colombia | 5 días hábiles (art. 47 Ley 1480) | Excepción legal: servicio que empezó con el acuerdo del consumidor | Dudoso: un crédito o PRO empiezan a darse al instante y con acuerdo | Senado, 2-11-2026 |
| México | 5 días hábiles (art. 56 LFPC) | Para servicios, no se aplica si la prestación está a ≤ 10 días hábiles | Dudoso: artículo del capítulo de ventas fuera del establecimiento; la prestación es inmediata | diputados.gob.mx, 2-11-2026 |
| Perú | NO VERIFICADO | — | — | — |

**Qué deberían decir los Términos.** Hoy los Términos dicen «desistimiento de 14 días con consentimiento para los consumibles», el régimen de la UE.

1. Una cláusula de que, si la ley de consumo del país de residencia da derechos imperativos (que no se pueden excluir), **se respetan**.
2. Para Chile, la **exclusión expresa** del retracto en el contenido digital que se presta al instante, aceptada antes de pagar. Las casillas actuales ya pueden servir si se menciona.
3. Para Argentina, reconocer los **10 días** (o la excepción del Código Civil y Comercial si se verifica).
4. Recordar que los reembolsos de Google Play se rigen también por su política.

---

## 5. Propuesta de texto para añadir (en español; traducir a los ocho idiomas)

### 5.1 Política de privacidad: sección nueva «20. Información adicional según tu país»

> **20.1 Quién es el responsable y cómo contactar.** El responsable de tus datos, y la persona encargada de la protección de los datos personales, es Alex Vida, desarrollador independiente, [domicilio postal: calle, ciudad, código postal], España. Correo: vidarpgapp@gmail.com. Respondemos en un plazo máximo de 20 días.
>
> **20.2 Dónde se tratan los datos que salen del teléfono.** Los pocos datos que salen del teléfono (sección 8, el Coach IA; 9, los anuncios; 11 y 12, las compras y los créditos) los tratan proveedores en Estados Unidos: Cloudflare, Inc.; RevenueCat, Inc.; y Google (en el EEE, Google Ireland Limited). Allí pueden quedar al alcance de los tribunales y las autoridades de ese país según su ley. Las transferencias desde el Espacio Económico Europeo se basan en las cláusulas contractuales tipo de la UE y en el Data Privacy Framework. Cuando la ley de tu país lo pide, esto se te comunica antes de enviar nada. No hay ninguna transferencia si no usas esas funciones.
>
> **20.3 Datos sensibles.** VIDA no vende ningún dato, tampoco los sensibles. Tus datos de actividad física, tus caídas y tus respuestas a la guía se quedan en tu teléfono. Lo único que puede viajar y rozar la salud es la categoría y la frecuencia de los vicios que registras, dentro de una consulta al Coach que tú pides. El servidor no lo guarda.
>
> **20.4 Estados Unidos.**
> - **Do Not Track.** La aplicación no rastrea tu actividad en otros sitios ni apps. Como no existe una norma común para esas señales, la aplicación no responde a ellas. Lo que decide qué anuncios ves es tu elección en Ajustes → Anuncios y la configuración del identificador de publicidad de Android.
> - **Rastreo por terceros.** Solo si pides ver un anuncio bonificado, Google AdMob puede recoger, a través de su componente en la app, datos sobre tu uso de esta y de otras apps a lo largo del tiempo, según su política. VIDA no lo hace.
> - **California.** VIDA no vende tus datos personales ni los comparte para publicidad comportamental con fines propios. Esta política está en vigor desde la fecha que figura arriba. Si cambia algo importante, te avisaremos dentro de la aplicación antes de que el cambio tenga efecto.
> - **Datos de salud del consumidor (Washington, Nevada y otros estados).** VIDA no recoge en ningún servidor tus datos de actividad física, que se tratan solo en tu teléfono. Datos que se pueden considerar de salud: los vicios que registras (categoría y frecuencia), que solo viajan si pides una consulta al Coach, para darte la respuesta, y que no se guardan ni se comparten con nadie. Fuente: tú. Puedes pedir información o el borrado en vidarpgapp@gmail.com.
> - **Menores.** La app no se dirige a menores de 13 años y no recoge a sabiendas sus datos. Si sabemos que un menor ha comprado créditos, borraremos sus datos del servidor.
>
> **20.5 Canadá y Quebec.** La persona responsable de la protección de los datos personales es la del punto 20.1. Puedes reclamar ante el Commissariat à la protection de la vie privée du Canada o, en Quebec, ante la Commission d'accès à l'information. Tus datos pueden comunicarse fuera de Quebec (punto 20.2). Solo si pides un anuncio, Google usa un identificador que permite perfilarte; tú decides si los anuncios son personalizados (sección 9).
>
> **20.6 México.** Este apartado y la política completa son el aviso de privacidad integral. Puedes ejercer tus derechos ARCO (acceso, rectificación, cancelación y oposición) escribiendo a vidarpgapp@gmail.com, y te responderemos en un máximo de 20 días. Las finalidades que necesitan tu consentimiento son los anuncios personalizados y el Coach IA. La autoridad es la Secretaría Anticorrupción y Buen Gobierno.
>
> **20.7 Chile (desde el 1-12-2026), Argentina, Uruguay, Colombia, Perú y Ecuador.** Tienes derecho de acceso, rectificación, supresión, oposición, portabilidad y bloqueo, y a retirar tu consentimiento cuando quieras. La base de cada tratamiento está en su sección: tu petición expresa (Coach, compras y códigos), tu consentimiento (anuncios personalizados) y el interés legítimo en frenar el abuso (las huellas diarias). Conservación: un día para las huellas y 24 meses sin actividad para el saldo de créditos. La app no toma decisiones automatizadas con efectos jurídicos sobre ti. Puedes reclamar ante la autoridad de tu país: Agencia de Protección de Datos Personales (Chile), Agencia de Acceso a la Información Pública (Argentina), Unidad Reguladora y de Control de Datos Personales (Uruguay), Superintendencia de Industria y Comercio (Colombia), Autoridad Nacional de Protección de Datos Personales (Perú) y Superintendencia de Protección de Datos Personales (Ecuador). [Perú y Ecuador: representante o apoderado, si se designa.]

Además, en la sección 18 («Cambios en esta política»): «Si cambia algo importante, te avisaremos dentro de la aplicación al abrirla y antes de que el cambio tenga efecto». Y poner la etiqueta «**Fecha de efecto**» junto a «Última actualización».

### 5.2 Términos de uso: suscripciones y consumo fuera de la UE

> **Renovación automática.** PRO mensual (5,99 €/mes) y PRO anual (39,99 €/año), o el precio equivalente que te muestre Google Play en tu moneda, con impuestos, **se renuevan automáticamente** al final de cada periodo y se cobran en tu cuenta de Google Play hasta que canceles. **Prueba gratuita:** el plan anual incluye 7 días gratis. Si no cancelas antes de que terminen, el primer año se cobra el día en que acaba la prueba. **Cancelar:** en cualquier momento, en Google Play → Pagos y suscripciones → Suscripciones, o desde Ajustes → PRO → «Gestionar suscripción» dentro de la app. Conservas PRO hasta el final del periodo pagado. **Recordatorios:** la app te avisará dentro del propio teléfono antes de cada renovación anual, al menos 5 días antes, con su importe, su fecha y cómo cancelar. Si el precio cambia, te avisaremos dentro de la app al menos 30 días antes. **Consentimiento:** al pulsar «Suscribirse» aceptas estas condiciones de renovación, que se muestran antes de la hoja de pago.
>
> **Si vives fuera de la Unión Europea.** Si la ley de consumo de tu país te da derechos que no se pueden excluir por contrato (por ejemplo, el plazo de revocación de 10 días en Argentina o la cancelación por el mismo medio), los respetamos, y nada de estos Términos los limita. **Chile:** de acuerdo con el artículo 3° bis b) de la Ley 19.496, el derecho de retracto no se aplica a las compras de contenido digital que empiezan a prestarse al instante y que aceptas expresamente antes de pagar. Lo puedes pedir igualmente a Google Play según su política de reembolsos.

### 5.3 Cambios en la app (no son texto legal, pero los piden las leyes)

1. **Aviso local antes de la renovación anual**, al menos 5 días antes (México, LFPC 76 bis VIII), sin datos y con enlace al Centro de suscripciones de Play. También sirve como «recordatorio anual» de la ARL de California. Es una notificación local: no cambia la política de privacidad.
2. **Enlace «Gestionar suscripción»** en Ajustes/PRO a `https://play.google.com/store/account/subscriptions` (política de Play y ARL: cancelación en línea). **Comprobar que exista.**
3. En la pantalla de PRO, **antes** de la hoja de Google: el precio, la frecuencia, que se renueva sola, la prueba y cuándo se cobra, y cómo cancelar (ARL §17602, ROSCA, LFPC VIII).
4. Sitio legal: un **enlace visible desde la página de inicio** al apartado de datos de salud del consumidor (RCW 19.373.020(1)(b)).
5. Abrir la versión **FR** de los textos legales con el sistema en francés (Quebec).

### 5.4 Pendiente de decisión del propietario (no lo puede resolver la investigación)

- **Domicilio postal** público (lo piden PIPEDA 4.8.2, la LFPDPPP 15-I, la Ley 25.326 art. 6, la Ley 18.331 art. 13, la Ley 21.719 art. 14 ter c y la LFPC 76 bis III). Hoy la política solo pone «España». Un apartado de correos o un domicilio profesional puede servir: **NO VERIFICADO** en cada país.
- **Representante en Perú** (DS 016-2024-JUS) y **apoderado en Ecuador**: coste frente a riesgo. Con datos mínimos, el riesgo práctico es bajo, pero no nombrarlo es un incumplimiento formal.
- **Evaluación de impacto** del art. 17 de la ley de Quebec para las comunicaciones a EE. UU.: es un documento interno breve.

---

## 6. Fuentes consultadas (2-11-2026)

- FindLaw, Cal. Bus. & Prof. Code §22575 y §22577 (texto «al 1-1-2026»): codes.findlaw.com/ca/business-and-professions-code/bpc-sect-22575/ y …-22577/. Leginfo devolvió 403.
- CPPA, ajuste por IPC: https://cppa.ca.gov/regulations/cpi_adjustment.html
- Virginia Code §59.1-576: https://law.lis.virginia.gov/vacode/title59.1/chapter53/section59.1-576/
- PBN Law, «Applicability for the 2026 class» (1-8-2025): https://pbnlaw.com/webfiles/State-Data-Privacy-Laws_Applicability-Triggers_2026-class.pdf.pdf
- Troutman Pepper, U.S. State Comprehensive Privacy Laws Chart (enero de 2025): https://www.troutman.com/wp-content/uploads/2024/12/U.S.-State-Comprehensive-Privacy-Laws-Chart-January-2025-revised-2.pdf
- Connecticut SB 1295: Hunton https://www.hunton.com/privacy-and-information-security-law/connecticut-amends-the-connecticut-data-privacy-act · FPF https://fpf.org/blog/the-connecticut-data-privacy-act-gets-an-overhaul-again/
- Texas TDPSA: https://texasattorneygeneral.gov/consumer-protection/file-consumer-complaint/consumer-privacy-rights/texas-data-privacy-and-security-act · https://sll.texas.gov/spotlight/2024/07/texas-data-privacy-and-security-act
- FTC COPPA: https://www.ftc.gov/legal-library/browse/rules/childrens-online-privacy-protection-rule-coppa · Hunton https://www.hunton.com/privacy-and-cybersecurity-law-blog/coppa-rule-amendment-compliance-deadline-approaches
- ARL AB 2863: Latham & Watkins, alerta 3301 (10-10-2024) https://lw.com/admin/upload/SiteAttachments/In-California-New-Automatic-Renewal-and-Continuous-Service-Requirements-Signed-Into-Law.pdf · Fenwick https://fenwick.com/insights/publications/california-tightens-requirements-for-automatically-renewing-subscriptions
- Click-to-Cancel: Greenberg Traurig https://www.gtlaw.com/en/insights/2025/7/eighth-circuit-vacates-ftcs-click-to-cancel-rule · ANPRM de la FTC https://www.ftc.gov/news-events/news/press-releases/2026/03/ftc-seeks-public-comment-response-advance-notice-proposed-rulemaking-regarding-negative-option · https://www.federalregister.gov/documents/2026/03/13/2026-04952/rule-concerning-the-use-of-prenotification-negative-option-plans
- ROSCA 15 U.S.C. 8403: https://www.law.cornell.edu/uscode/text/15/8403
- Google Play, suscripciones: https://support.google.com/googleplay/android-developer/answer/9900533
- Washington RCW 19.373.010 y .020: https://app.leg.wa.gov/RCW/default.aspx?cite=19.373.010 · …=19.373.020
- Nevada SB 370: WilmerHale https://www.wilmerhale.com/en/insights/blogs/wilmerhale-privacy-and-cybersecurity-law/20230614-nevada-legislature-passes-consumer-health-data-privacy-bill · NRS 603A https://www.leg.state.nv.us/nRs/NRS-603A.html (no leído)
- PIPEDA, Anexo 1: https://laws-lois.justice.gc.ca/eng/acts/P-8.6/page-7.html · CPVP Globe24h https://www.priv.gc.ca/en/opc-actions-and-decisions/investigations/investigations-into-businesses/2015/pipeda-2015-002/ · Issue sheets https://www.priv.gc.ca/en/privacy-and-transparency-at-the-opc/proactive-disclosure/opc-parl-bp/ethi_20231025/is_20231025/
- Quebec, Ley 25 (secundarias): https://gowlingwlg.com/en/insights-resources/articles/2022/how-well-do-you-know-quebec-s-law-25 · Carta de la lengua francesa: https://nortonrosefulbright.com/en/knowledge/publications/78e479b4/charter-of-the-french-language-mutual-agreement-contracts-containing-standard-clauses
- México LFPDPPP: https://www.diputados.gob.mx/LeyesBiblio/pdf/LFPDPPP.pdf · LFPC: https://www.diputados.gob.mx/LeyesBiblio/pdf/LFPC.pdf
- Argentina Ley 25.326: https://servicios.infoleg.gob.ar/infolegInternet/anexos/60000-64999/64790/texact.htm · Ley 24.240: https://servicios.infoleg.gob.ar/infolegInternet/anexos/0-4999/638/texact.htm · Res. AAIP 14/2018: https://www.argentina.gob.ar/normativa/nacional/resoluci%C3%B3n-14-2018-307621/texto
- Chile Ley 21.719: https://www.leychile.cl/Consulta/obtxml?opt=7&idNorma=1209272 · Ley 19.496: https://www.leychile.cl/Consulta/obtxml?opt=7&idNorma=61438
- Colombia Ley 1581: http://www.secretariasenado.gov.co/senado/basedoc/ley_1581_2012.html · Ley 1480: http://www.secretariasenado.gov.co/senado/basedoc/ley_1480_2011_pr001.html
- Perú DS 016-2024-JUS: CMS https://cms.law/en/per/publication/nuevo-reglamento-de-proteccion-de-datos-personales · Pérez-Llorca https://www.perezllorca.com/es-pe/actualidad/articulos/se-aprueba-nuevo-reglamento-de-la-ley-de-proteccion-de-datos-personales/
- Uruguay Ley 18.331: https://www.impo.com.uy/bases/leyes/18331-2008 · Ley 19.670: https://www.impo.com.uy/bases/leyes/19670-2018
- Ecuador LOPDP: https://www.gob.ec/regulaciones/ley-organica-proteccion-datos-personales-0 · apoderados especiales: https://www.gob.ec/spdp/tramites/registro-apoderados-especiales
- Paraguay Ley 7593/2025: https://www.bacn.gov.py/leyes-paraguayas/12924/ley-n-75932025--de-proteccin-de-datos-personales-en-la-repblica-del-paraguay · Ferrere https://ferrere.com/es/novedades/paraguay-adopta-su-ley-de-proteccion-de-datos-personales/
