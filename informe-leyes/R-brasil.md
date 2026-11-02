# Brasil · LGPD y normas conexas aplicadas a VIDA RPG

Fecha de consulta de todas las fuentes: **02-11-2026**. Hechos de la app: `BRIEF.md`; política revisada: `politica-privacidad-es.txt` (versión 2.17.1, 13-10-2026).

**Fuentes y su fiabilidad.** `planalto.gov.br` devolvió «Acesso Negado» / 503 (bloqueo automático) en todos los intentos. Por eso los textos de las leyes se han leído en la **Legislação Informatizada de la Câmara dos Deputados** (`www2.camara.leg.br/legin`, oficial; la versión «norma atualizada» incluye las reformas con su nota) y en la Imprensa Nacional (`in.gov.br`, DOU) y `gov.br/anpd` para las resoluciones. Las citas en portugués de abajo son literales de esas páginas.

**Novedad que la política tiene que reflejar (verificada):** la **Lei nº 15.352, de 25-02-2026** (conversión de la MP 1.317/2025) convierte la ANPD en **«Agência Nacional de Proteção de Dados»** (la sigla sigue siendo ANPD) y cambia la redacción del art. 5 VIII y XIX de la LGPD. Fuente: LGPD compilada, Câmara (abajo) y Lei 15.352, publicação original: https://www2.camara.leg.br/legin/fed/lei/2026/lei-15352-25-fevereiro-2026-798731-publicacaooriginal-178208-pl.html

Fuente base de la LGPD (todos los artículos citados): Lei nº 13.709, de 14-08-2018, texto actualizado de la Câmara: https://www2.camara.leg.br/legin/fed/lei/2018/lei-13709-14-agosto-2018-787077-normaatualizada-pl.html

---

## 1. LGPD (Lei 13.709/2018)

### 1.1 Art. 3: aplicación extraterritorial
- Texto: «aplica-se a qualquer operação de tratamento realizada por **pessoa natural** ou por pessoa jurídica [...] independentemente [...] do país de sua sede [...], desde que: [...] II - a atividade de tratamento tenha por objetivo a **oferta ou o fornecimento de bens ou serviços** [...] de indivíduos localizados no território nacional; ou III - os dados pessoais [...] tenham sido coletados no território nacional. § 1º Consideram-se coletados no território nacional os dados pessoais cujo titular nele se encontre no momento da coleta.» (inciso II con la redacción de la Lei 13.853/2019).
- **¿Se aplica a VIDA? Sí.** La app se ofrece en portugués de Brasil por Google Play y cobra en la tienda brasileña; el inciso II alcanza a un controlador persona física y extranjero. Además, los datos que salen del teléfono de alguien que está en Brasil se «recogen en el territorio nacional» (§ 1º, inciso III). Las excepciones del art. 4 (uso particular sin fines económicos, etc.) no cubren a un desarrollador que vende.
- **Lo que hoy falta en la política:** no dice que la LGPD se aplica a las personas usuarias en Brasil. Todo el apartado de derechos se apoya solo en el RGPD.

### 1.2 Art. 7 y art. 11: bases legales
- Art. 7 (datos personales), incisos que interesan: «I - mediante o fornecimento de **consentimento** pelo titular»; «II - para o cumprimento de obrigação legal ou regulatória pelo controlador»; «V - quando necessário para a **execução de contrato** [...] do qual seja parte o titular, a pedido do titular»; «VI - para o exercício regular de direitos em processo judicial, administrativo ou arbitral»; «IX - quando necessário para atender aos **interesses legítimos** do controlador ou de terceiro, exceto no caso de prevalecerem direitos e liberdades fundamentais do titular». El art. 10 § 2º exige transparencia cuando la base es el interés legítimo.
- Art. 11 (datos sensibles; el art. 5 II incluye «dado referente à saúde»): «I - quando o titular [...] consentir, de **forma específica e destacada**, para finalidades específicas»; II, sin consentimiento solo en los supuestos tasados (obligación legal, ejercicio de derechos, protección de la vida, tutela de la salud por profesionales, «g) garantia da prevenção à fraude e à segurança do titular, nos processos de identificação e autenticação de cadastro em sistemas eletrônicos»).
- Art. 8: el consentimiento se da «por escrito ou por outro meio que demonstre a manifestação de vontade»; § 5º «pode ser revogado a qualquer momento [...] por procedimento gratuito e facilitado».
- **Aplicación a VIDA (interpretación, no lo dice ninguna norma ni la ANPD):**
  - Coach IA: lo pide la persona y se le presta → art. 7 V (contrato). **Pero** el resumen que viaja incluye «los vicios registrados» (tabaco, alcohol…) y hábitos. Es razonable que la ANPD lo vea como «dado referente à saúde» (art. 5 II). Si es así, la única base práctica es el **art. 11 I: consentimiento específico y destacado**, y la ejecución de contrato no sirve para datos sensibles. Recomendación prudente: una casilla o pantalla de consentimiento propia antes de la primera consulta (al menos para Brasil), revocable.
  - Huella salada de IP e ID de instalación (antiabuso, 1 día): art. 7 IX (interés legítimo), con la información del art. 10 § 2º. El art. 11 II g no encaja, porque no hay «cadastro».
  - Anuncios AdMob a petición: consentimiento (art. 7 I), o la ejecución de lo que se pide. Ojo con el **Marco Civil art. 7 VII** (punto 5): no se pueden dar a terceros datos ni registros de acceso «salvo mediante consentimento livre, expresso e informado». La vía segura es el consentimiento. No está verificado que Google UMP muestre un aviso LGPD en Brasil (NO VERIFICADO).
  - Compras, créditos y códigos: art. 7 V (contrato) y, para conservar los registros de compra y defenderse de reclamaciones, art. 7 VI.
  - Health Connect y la foto del avatar no salen del teléfono, así que el desarrollador no los trata. Aun así conviene decirlo, como ya hace la política.
- **Lo que falta:** la política no nombra **ninguna base legal**. La LGPD no lo exige con esas palabras en el art. 9, pero el art. 9 § 3º y el art. 10 § 2º lo hacen necesario en la práctica, y la ANPD lo espera. Falta también el consentimiento destacado si los vicios cuentan como datos de salud.

### 1.3 Art. 9: información al titular
- Texto: «O titular tem direito ao acesso facilitado às informações sobre o tratamento de seus dados, que deverão ser disponibilizadas de forma **clara, adequada e ostensiva** acerca de [...]: I - finalidade específica do tratamento; II - forma e duração do tratamento [...]; III - identificação do controlador; IV - informações de contato do controlador; V - informações acerca do uso compartilhado de dados pelo controlador e a finalidade; VI - responsabilidades dos agentes que realizarão o tratamento; e VII - direitos do titular, com **menção explícita aos direitos contidos no art. 18**». § 1º: el consentimiento es nulo si la información fue «enganosa ou abusiva» o no se dio «previamente com transparência». § 3º: si el tratamiento es condición del servicio, se informa «com destaque».
- **Aplicación:** se aplica entero.
- **Lo que hoy cumple la política:** finalidad (I), forma y en parte la duración (II), contacto (IV) y con quién se comparte (V; Cloudflare, Google, RevenueCat).
- **Lo que falta:** (VI) las **responsabilidades** de cada agente: quién es controlador y quién operador (Cloudflare y RevenueCat, operadores; Google AdMob y Google Play, en buena parte controladores independientes según sus propias condiciones). (VII) la **lista explícita del art. 18**: hoy la política solo enumera los derechos del RGPD. (II) la duración de cada dato en una tabla: la huella de 1 día, los créditos 24 meses, el resto nada. (III) la identificación: «Alex Vida, desarrollador independiente, España». Para el art. 9 basta probablemente con eso, pero ver el Decreto 7.962 en el punto 7.

### 1.4 Art. 18: derechos (lista exacta) y cómo se ejercen
- Texto del caput: «O titular dos dados pessoais tem direito a obter do controlador, [...] a qualquer momento e mediante requisição:
  - I - confirmação da existência de tratamento;
  - II - acesso aos dados;
  - III - correção de dados incompletos, inexatos ou desatualizados;
  - IV - anonimização, bloqueio ou eliminação de dados desnecessários, excessivos ou tratados em desconformidade com o disposto nesta Lei;
  - V - portabilidade dos dados a outro fornecedor de serviço ou produto, mediante requisição expressa, de acordo com a regulamentação da autoridade nacional [...];
  - VI - eliminação dos dados pessoais tratados com o consentimento do titular, exceto nas hipóteses previstas no art. 16 desta Lei;
  - VII - informação das entidades públicas e privadas com as quais o controlador realizou uso compartilhado de dados;
  - VIII - informação sobre a possibilidade de não fornecer consentimento e sobre as consequências da negativa;
  - IX - revogação do consentimento, nos termos do § 5º do art. 8º desta Lei.»
- Párrafos:
  - «§ 1º O titular dos dados pessoais tem o direito de **peticionar** em relação aos seus dados contra o controlador **perante a autoridade nacional**.»
  - «§ 2º O titular pode **opor-se** a tratamento realizado com fundamento em uma das hipóteses de dispensa de consentimento, em caso de descumprimento ao disposto nesta Lei.»
  - «§ 3º Os direitos [...] serão exercidos mediante requerimento expresso do titular ou de representante legalmente constituído, a agente de tratamento.»
  - § 4º: si no se puede atender de inmediato, se responde diciendo que no se es agente de tratamiento (indicando cuál, si se puede) o dando las razones de hecho o de derecho.
  - «§ 5º O requerimento [...] será atendido **sem custos** para o titular, nos prazos e nos termos previstos em regulamento.»
  - § 6º: comunicar a quien se compartió la corrección o eliminación.
  - «§ 8º O direito a que se refere o § 1º deste artigo também poderá ser exercido perante os **organismos de defesa do consumidor**.»
- **Aplicación:** sí. En la práctica casi todo se resuelve en el dispositivo (exportar, editar, reiniciar), y para los créditos, por correo con el número de pedido. Eso vale, pero hay que presentarlo **con los nombres de la LGPD**.
- **Lo que falta:**
  - confirmación de que hay tratamiento (I);
  - anonimización y bloqueo (IV);
  - información sobre con quién se comparte (VII; se puede remitir a la sección correspondiente);
  - información sobre no consentir y sus consecuencias (VIII: sin consentimiento no hay Coach ni anuncio, y el resto de la app funciona igual);
  - revocación (IX);
  - oposición (§ 2º);
  - gratuidad (§ 5º);
  - reclamación ante la ANPD (§ 1º) y ante los Procon u otros organismos de consumo (§ 8º).
  
  Hoy la política solo menciona a la AEPD o a «la autoridad de control de tu país».

### 1.5 Art. 41: encarregado
- Texto: «O controlador deverá indicar encarregado [...]. § 1º A identidade e as informações de contato do encarregado deverão ser divulgadas publicamente [...]. § 3º A autoridade nacional poderá estabelecer normas complementares [...] inclusive hipóteses de **dispensa** [...] conforme a natureza e o porte da entidade ou o volume de operações». § 2º I: el encarregado debe «aceitar reclamações e comunicações dos titulares, prestar esclarecimentos e adotar providências».
- La **Resolução CD/ANPD nº 18, de 16-07-2024** (DOU 17-07-2024), regulamento do encarregado, dice:
  - art. 3 § 3º: «Os Agentes de Tratamento de Pequeno Porte dispensados de indicar encarregado devem disponibilizar um **canal de comunicação** com o titular de dados, nos termos do art. 11» de la Res. 2/2022;
  - art. 13: «O encarregado deverá ser capaz de comunicar-se com os titulares e com a ANPD [...] **em língua portuguesa**»;
  - art. 9 § 1º I: si se nombra, hay que publicar su «nome completo».
  - Fuente: https://www.in.gov.br/en/web/dou/-/resolucao-cd/anpd-n-18-de-16-de-julho-de-2024-572632074 . Según la lista de la ANPD, está vigente y sin cambios.
- **Aplicación:** si VIDA es «agente de pequeño porte» (punto 2), **no tiene que nombrar encarregado**, pero sí tener un canal (vidarpgapp@gmail.com sirve). Si no lo es (alto riesgo), tendría que nombrarlo y publicar su nombre completo, y debería poder atender en portugués.
- **Lo que falta:** decir que el canal de privacidad atiende también a titulares de Brasil y en portugués, y, si se acoge a la dispensa, decirlo de forma expresa.

### 1.6 ¿Hace falta un representante en Brasil? Art. 61
- Texto: «Art. 61. A **empresa estrangeira** será notificada e intimada de todos os atos processuais previstos nesta Lei, independentemente de procuração [...], na pessoa do agente ou representante ou pessoa responsável por sua filial, agência, sucursal, estabelecimento ou escritório **instalado no Brasil**.»
- **Conclusión, CONFIRMADA en el texto:** la LGPD **no tiene una figura equivalente al art. 27 del RGPD**. Ningún artículo obliga a nombrar un representante. El art. 61 solo dice a quién se notifica cuando la empresa extranjera ya tiene filial, agencia o establecimiento en Brasil; no crea la obligación de tenerlos. Además habla de «empresa estrangeira», y VIDA es una persona física sin presencia en Brasil. El art. 41 (encarregado) es otra cosa: es un canal, no un representante legal, y además está la dispensa para los pequeños.
- **Ojo, distinto:** el **ECA Digital (art. 40) SÍ exige un representante legal en Brasil** a los proveedores incluidos en su art. 1 (punto 8).

### 1.7 Art. 33 y Resolução CD/ANPD nº 19/2024: transferencia internacional
- **Art. 33** (mecanismos): «I - para países ou organismos internacionais que proporcionem grau de proteção [...] adequado»; «II - [...] b) cláusulas-padrão contratuais»; «VIII - quando o titular tiver fornecido o seu consentimento específico e em destaque para a transferência, com informação prévia sobre o caráter internacional da operação»; «IX - quando necessário para atender as hipóteses previstas nos incisos II, V e VI do art. 7º» (obligación legal, contrato, ejercicio de derechos).
- **Res. CD/ANPD nº 19, de 23-08-2024** (DOU 23-08-2024; rectificada en el DOU de 18-08-2025), Regulamento de Transferência Internacional y cláusulas-padrão. Fuente: https://www.gov.br/anpd/pt-br/acesso-a-informacao/institucional/atos-normativos/regulamentacoes_anpd/resolucao-cd-anpd-no-19-de-23-de-agosto-de-2024
  - Plazo, art. 2 parágrafo único: «Os agentes de tratamento que utilizam cláusulas contratuais [...] deverão incorporar as cláusulas-padrão contratuais aprovadas pela ANPD [...] no prazo de até **12 (doze) meses**, contados da data de publicação». **El plazo venció en agosto de 2025** (doce meses desde el 23-08-2024; el día exacto, 22 o 23, depende de cómo se cuente).
  - Definiciones (art. 3): el exportador puede estar «no território nacional **ou em país estrangeiro**». El art. 6 dice: «A **coleta internacional** de dados não caracteriza transferência internacional», y la define como la coleta «efetuada diretamente pelo agente de tratamento localizado no exterior». Según el art. 7 II, las reglas de transferencia se aplican cuando el tratamiento tiene por objeto ofrecer servicios a personas en Brasil.
  - Transparencia, art. 17 § 2º: el controlador «deverá ainda **publicar em sua página na Internet** documento contendo informações **em língua portuguesa**, em linguagem simples [...] sobre a realização da transferência internacional», con al menos: forma, duración y finalidad; **país de destino**; identificación y contacto del controlador; uso compartido; responsabilidades y medidas de seguridad; derechos y cómo ejercerlos, «incluindo canal de fácil acesso e o direito de peticionar contra o controlador perante a ANPD». Se puede integrar «de forma destacada» en la política (§ 3º). Art. 17 caput y § 1º: entregar las cláusulas al titular que las pida en **15 días**.
- **Res. CD/ANPD nº 32, de 26-01-2026** (DOU 27-01-2026): la ANPD reconoce **la Unión Europea (y el EEE) como adecuada** a efectos del art. 33 I. Fuente: https://www.in.gov.br/web/dou/-/resolucao-n-32-de-26-de-janeiro-de-2026-683334547 . La lista de resoluciones de la ANPD no muestra ninguna otra decisión de adecuación: **EE. UU. no es adecuado para Brasil** (https://www.gov.br/anpd/pt-br/acesso-a-informacao/institucional/atos-normativos/regulamentacoes_anpd).
- **Aplicación a VIDA (interpretación):**
  - Del teléfono en Brasil al controlador en España: o es «coleta internacional» (art. 6) o, si se considera transferencia, España está cubierta por la adecuación de la UE (Res. 32/2026).
  - Al Worker de Cloudflare (EE. UU.): el teléfono envía directamente a un operador en el extranjero que trabaja para el controlador. Hay buenos argumentos para llamarlo «coleta internacional» (art. 6), pero la ANPD no lo ha resuelto para este caso. Si cuenta como transferencia del controlador (exportador en España) a su operador en EE. UU., hace falta un mecanismo: las **cláusulas-padrão de la ANPD**, o el art. 33 IX (necesaria para el contrato, art. 7 V; no sirve para datos sensibles) o el VIII (consentimiento específico y destacado). **Comprobado: la DPA de Cloudflare (v6.4, en vigor desde el 03-04-2026) no menciona Brasil, la LGPD, la ANPD ni las cláusulas brasileñas** (https://www.cloudflare.com/cloudflare-customer-dpa/). Por tanto, con Cloudflare **no hay cláusulas-padrão de la ANPD**.
  - RevenueCat: su DPA (en vigor desde agosto de 2026) **menciona la LGPD pero no la ANPD ni sus cláusulas**; las SCC que lleva son las de la UE, el Reino Unido y Suiza (https://www.revenuecat.com/dpa/).
  - Google (AdMob): Google publica un «LGPD Controller Addendum» y cláusulas tipo para la LGPD (https://business.safety.google/adscontrollerterms/lgpd/ , https://business.safety.google/applicablesccs/). **NO VERIFICADO** que reproduzcan íntegras las cláusulas del Anexo II de la Res. 19/2024 ni que cubran AdMob en concreto.
  - Google Play: Google trata los datos de compra como su propio controlador. Su marco no se ha comprobado (NO VERIFICADO).
- **Lo que falta en la política:**
  1. Un bloque «Transferencias internacionales (LGPD)» en portugués con el contenido del art. 17 § 2º: países de destino (España y la UE; EE. UU.), finalidad, duración, mecanismo de cada destinatario y el derecho de peticionar ante la ANPD.
  2. Decir que se entregan las cláusulas a quien las pida, en 15 días.
  3. Decidir el mecanismo con Cloudflare y RevenueCat: proponerles las cláusulas-padrão de la ANPD (sin cambios) o apoyarse en el art. 33 IX/VIII y explicarlo.
  
  Hoy la política solo cita las SCC de la UE y el DPF, que **no sirven para la LGPD**.

---

## 2. Resolução CD/ANPD nº 2/2022: agentes de tratamiento de pequeño porte
Fuentes: DOU de 28-01-2022, ed. 20, sec. 1 (https://www.in.gov.br/en/web/dou/-/resolucao-cd/anpd-n-2-de-27-de-janeiro-de-2022-376562019) y el texto consolidado de la ANPD, «alterado pela Resolução CD/ANPD nº 15, de 2024», con la página modificada el 16-09-2026 (https://www.gov.br/anpd/pt-br/acesso-a-informacao/institucional/atos-normativos/regulamentacoes_anpd/resolucao-cd-anpd-no-2-de-27-de-janeiro-de-2022). La lista de la ANPD la da como «Vigente com alterações pela Resolução CD/ANPD nº 15, de 24 de abril de 2024». La Res. 15/2024 **solo cambia el art. 14 II** (remite al Regulamento de Comunicação de Incidente). La Res. 18/2024 no la modifica, pero la cita y confirma la dispensa (art. 3 § 3º). **No se ha encontrado ninguna otra revisión hasta el 02-11-2026.**

- **Definición, art. 2 I (literal):** «agentes de tratamento de pequeno porte: microempresas, empresas de pequeno porte, startups, pessoas jurídicas de direito privado, inclusive sem fins lucrativos, nos termos da legislação vigente, **bem como pessoas naturais e entes privados despersonalizados** que realizam tratamento de dados pessoais, assumindo obrigações típicas de controlador ou de operador». **Sí: incluye a las personas naturales y a los entes despersonalizados.** El art. 1 parágrafo único excluye el tratamiento «por pessoa natural para fins exclusivamente particulares e não econômicos» (no es el caso de VIDA, que vende).
- **Exclusiones, art. 3:** no se benefician quienes «I - realizem tratamento de **alto risco** para os titulares [...]; II - aufiram receita bruta superior ao limite estabelecido no art. 3º, II, da Lei Complementar nº 123, de 2006 [...]; ou III - pertençam a grupo econômico [...] cuja receita global ultrapasse os limites».
  - **El umbral:** el art. 3 II de la LC 123/2006, en la redacción de la LC 155/2016, dice «receita bruta superior a R$ 360.000,00 [...] e igual ou inferior a **R$ 4.800.000,00**» por año natural (https://www2.camara.leg.br/legin/fed/leicom/2016/leicomplementar-155-27-outubro-2016-783850-normaatualizada-pl.html). **NO VERIFICADO** en el texto compilado de la LC 123 (la página de la Câmara dio 404) que ninguna ley posterior lo haya cambiado.
- **Alto riesgo, art. 4:** tiene que darse **a la vez al menos un criterio general y uno específico**.
  - Generales: «a) tratamento de dados pessoais em **larga escala**; ou b) tratamento [...] que possa **afetar significativamente** interesses e direitos fundamentais».
  - Específicos: «a) uso de **tecnologias emergentes ou inovadoras**; b) vigilância [...]; c) decisões tomadas unicamente com base em tratamento automatizado [...] inclusive [...] definir o perfil [...] de saúde [...]; ou d) utilização de **dados pessoais sensíveis** ou de dados pessoais de crianças, de adolescentes e de idosos».
  - § 1º: «larga escala [...] quando abranger **número significativo** de titulares, considerando-se, ainda, o volume de dados [...], a duração, a frequência e a extensão geográfica». **La norma no da ninguna cifra**; no se ha encontrado un umbral numérico de la ANPD (NO VERIFICADO que exista).
  - § 2º: el criterio de «afetar significativamente» abarca, por ejemplo, impedir un servicio, la discriminación, los fraudes financieros o el robo de identidad.
- **¿Puede quedar VIDA fuera del régimen de los pequeños? (interpretación)** VIDA cumple **criterios específicos**: el Coach IA es una tecnología emergente (a) y quizá trate datos sensibles (d), si los vicios cuentan como salud. Lo que decide es el **criterio general**. Mientras el número de usuarios brasileños del Coach sea modesto y la huella dure un día, es defendible que **no** hay «larga escala» ni un efecto «significativo» y que VIDA es **pequeño porte**. Si crece mucho en Brasil, el riesgo cambia. El art. 5 dice que, si la ANPD lo pide, hay que **probar** que se encaja (arts. 2 y 3) **en 15 días**, y el art. 16 permite a la ANPD exigir las obligaciones dispensadas.
- **Persona física extranjera (interpretación, la norma no dice nada expreso):**
  - El art. 2 I no exige registro en Brasil para las «pessoas naturais». Solo lo exige para las ME y EPP (inciso II: «devidamente registrados»).
  - El límite de ingresos del art. 3 II se mide en reales; para un extranjero habría que convertir sus ingresos. La norma no dice si cuentan todos o solo los de Brasil.
  - Lectura razonable: un autónomo español con ingresos por debajo de R$ 4,8 M al año y sin alto riesgo puede acogerse. **Ningún texto de la ANPD lo confirma para extranjeros.**
- **Lo que gana el pequeño porte:**
  - **Art. 11:** «não são obrigados a indicar o encarregado [...]. § 1º O agente [...] que não indicar um encarregado **deve disponibilizar um canal de comunicação** com o titular».
  - **Art. 14:** plazo **en dobro** para: «I - [...] solicitações dos titulares [...] art. 18, §§ 3º e 5º»; II - la comunicación de incidentes (desde la Res. 15/2024, según su reglamento); «III - no fornecimento de declaração clara e completa, prevista no art. 19, II» (es decir, **30 días** en lugar de 15); IV - los plazos ante la ANPD.
  - **Art. 15:** la declaración simplificada del art. 19 I (que para los demás es «imediatamente») puede darse «no prazo de até quinze dias».
  - **Art. 9:** registro de operaciones simplificado. **Art. 12-13:** medidas de seguridad esenciales y una política de seguridad simplificada.
  - El art. 6 deja claro que la dispensa «não isenta» de las bases legales, los principios ni los derechos de los titulares.
- **Lo que debería decir la política:** que se atiende por el canal vidarpgapp@gmail.com, que es el canal del art. 11 § 1º de la Res. 2/2022, y que el desarrollador se considera agente de pequeño porte y no ha nombrado encarregado. Esto último es opcional, pero evita dudas.

## 3. Cómo reclamar ante la ANPD
- **LGPD art. 55-J V:** la ANPD tiene que «apreciar petições de titular contra controlador **após comprovada pelo titular a apresentação de reclamação ao controlador não solucionada** no prazo estabelecido em regulamentação».
- **Res. CD/ANPD nº 1, de 28-10-2021** (Regulamento de Fiscalização; vigente con rectificaciones de la Res. 4/2023; https://www.gov.br/anpd/pt-br/acesso-a-informacao/institucional/atos-normativos/regulamentacoes_anpd/resolucao-cd-anpd-no1-2021):
  - art. 2 V: «petição de titular: comunicação feita à ANPD pelo titular [...] de uma solicitação apresentada ao controlador e não solucionada no prazo estabelecido em regulamentação»;
  - art. 25 § 1º: la petición «deverá ser acompanhada de comprovação de que foi previamente submetida ao controlador e não solucionada no prazo [...], **admitida a autodeclaração** do titular quando não for possível apresentar outro meio de prova»;
  - art. 26: las peticiones «serão analisadas de forma agregada».
- **Canal oficial:** el servicio «Abrir requerimento relacionado à LGPD» del portal gov.br, con **inicio de sesión de la cuenta gov.br**, para elegir «Petição de Titular» o «Denúncia»; hay que adjuntar la «Comprovação de contato prévio com o controlador». URL: https://www.gov.br/pt-br/servicos/abrir-requerimento-relacionado-a-lgpd . La página de la ANPD sobre la petición de titular (https://www.gov.br/anpd/pt-br/canais_atendimento/cidadao-titular-de-dados/peticao-de-titular-contra-controlador-de-dados) devolvió **401**: no se pudo leer en origen. Que desde el 01-01-2025 el único canal sea el «Sistema de Requerimentos» (y no el SEI) lo dice una noticia de la ANPD que solo se ha visto en el resumen del buscador (**NO VERIFICADO** en su texto).
- Alternativa legal: la petición también puede presentarse ante los **organismos de defesa do consumidor** (art. 18 § 8º).
- **Lo que tiene que decir la política:** que en Brasil se puede peticionar ante la ANPD (Agência Nacional de Proteção de Dados), con el enlace de gov.br, **después de haber escrito antes al contacto** y no haber recibido solución en plazo; y que también cabe acudir a los Procon y otros organismos de consumo.

## 4. Plazos de respuesta al titular
- **Art. 19 LGPD:** confirmación de existencia o acceso «I - em formato simplificado, **imediatamente**; ou II - por meio de declaração clara e completa, que indique a origem dos dados, a inexistência de registro, os critérios utilizados e a finalidade do tratamento [...], fornecida no prazo de até **15 (quinze) dias**, contado da data do requerimento». § 3º: si la base es el consentimiento o el contrato, el titular puede pedir una copia electrónica íntegra (según el reglamento de la ANPD). Para los demás derechos, el art. 18 § 5º remite a «prazos [...] previstos em regulamento». **En la lista de la ANPD (consultada el 02-11-2026) no hay ningún reglamento de derechos del titular que fije ese plazo general.**
- **Pequeño porte (Res. 2/2022):** declaración completa en **30 días** (art. 14 III, el doble de 15); simplificada en **15 días** (art. 15); el resto de solicitudes del art. 18, «em dobro» (art. 14 I), del plazo que fije un reglamento que aún no existe.
- **Por transferencias:** entregar las cláusulas en 15 días (Res. 19/2024 art. 17 § 1º). No consta que se doble para los pequeños.
- **Propuesta para la política:** «Respondemos en un plazo máximo de 15 días» (vale para todos los casos y no hace falta acogerse al doble), o «15 días, y en el caso de la declaración completa del art. 19 II, hasta 30 días como agente de pequeño porte». Lo más simple y prudente es **15 días**.

## 5. Marco Civil da Internet (Lei 12.965/2014)
Fuente: https://www2.camara.leg.br/legin/fed/lei/2014/lei-12965-23-abril-2014-778630-normaatualizada-pl.html
- **Art. 11:** «Em qualquer operação de coleta, armazenamento, guarda e tratamento de registros, de dados pessoais [...] por provedores de conexão e de aplicações de internet em que pelo menos um desses atos ocorra em território nacional, deverão ser obrigatoriamente respeitados a legislação brasileira [...]. § 2º O disposto no caput aplica-se mesmo que as atividades sejam realizadas por **pessoa jurídica** sediada no exterior, desde que oferte serviço ao público brasileiro [...]».
  - Para VIDA: la recogida desde un teléfono en Brasil ocurre en el territorio (caput), así que la ley brasileña se aplica. El § 2º habla de personas jurídicas, pero el caput no distingue.
- **Art. 7:** derechos del usuario.
  - «VII - não fornecimento a terceiros de seus dados pessoais, inclusive registros de conexão, e de acesso a aplicações de internet, **salvo mediante consentimento livre, expresso e informado** ou nas hipóteses previstas em lei»;
  - «VIII - informações claras e completas sobre coleta, uso, armazenamento, tratamento e proteção de seus dados pessoais»;
  - «IX - consentimento expresso [...] de forma destacada das demais cláusulas contratuais»;
  - «X - exclusão definitiva dos dados pessoais [...] a seu requerimento, ao término da relação».
  - Para VIDA, sobre todo el **VII y el IX** en los anuncios (Google recibe la IP y el identificador de publicidad) y en el Coach. Refuerzan la idea de un consentimiento expreso y destacado.
- **Art. 15:** «O provedor de aplicações de internet **constituído na forma de pessoa jurídica** e que exerça essa atividade de forma organizada, profissionalmente e com fins econômicos deverá manter os respectivos registros de acesso a aplicações de internet [...] pelo prazo de **6 (seis) meses**». § 1º: una orden judicial puede obligar a otros proveedores (los que no están en el caput) a guardar registros concretos.
  - **¿Aplica a una persona física? No, según la letra:** el caput se limita a la persona jurídica. VIDA (autónomo persona física) **no tiene obligación general de guardar 6 meses** los registros de acceso. Eso es coherente con la huella de 1 día. Quedan a salvo la orden judicial (§ 1º) y el requerimiento cautelar (§ 2º). Si algún día el desarrollador se constituye en sociedad, habría que revisarlo (y además entraría en tensión con «no guarda nada»).
- **Art. 8 parágrafo único II:** «São nulas de pleno direito as cláusulas [...] que: [...] II - em contrato de adesão, **não ofereçam como alternativa** ao contratante a adoção do **foro brasileiro** para solução de controvérsias decorrentes de serviços prestados no Brasil.» **Afecta a los Términos:** si solo dicen «ley y tribunales españoles», esa cláusula de foro es nula frente a un usuario de Brasil. Hay que añadir que el usuario en Brasil puede acudir al foro brasileño (véase también el CDC art. 101 I: la acción «pode ser proposta no domicílio do autor»).

## 6. Lengua
- **LGPD:** el art. 9 exige información «clara, adequada e ostensiva», **sin mencionar el portugués**: la LGPD por sí misma no dice el idioma.
- **Sí lo dicen otras normas:**
  - **CDC art. 31:** «A oferta e apresentação de produtos ou serviços devem assegurar informações corretas, claras, precisas, ostensivas e **em língua portuguesa** sobre suas características, [...] preço, garantia, prazos [...]» (Lei 8.078/1990, https://www2.camara.leg.br/legin/fed/lei/1990/lei-8078-11-setembro-1990-365086-normaatualizada-pl.html). Afecta a las condiciones de compra: PRO, la prueba, la renovación y los créditos.
  - **Res. ANPD 19/2024 art. 17 § 2º:** el documento sobre transferencias internacionales «em língua portuguesa».
  - **Res. ANPD 18/2024 art. 13:** el encarregado se comunica «em língua portuguesa».
- **Para VIDA:** la web legal tiene selector PT (consta en el fichero). Hay que comprobar que la política, los Términos y los textos de compra en PT están **completos e iguales al español**, y que el nuevo apartado LGPD existe también en PT. Recomendación: que el canal acepte peticiones en portugués.

## 7. Consumo
- **CDC art. 49 (arrepentimiento de 7 días)**, decisión del propietario: no se añade. Texto: «O consumidor pode desistir do contrato, no prazo de **7 dias** a contar de sua assinatura ou do ato de recebimento do produto ou serviço, sempre que a contratação [...] ocorrer **fora do estabelecimento comercial**», con devolución inmediata. **Riesgo, en dos líneas:** la doctrina y los Procon aplican el art. 49 a las compras por internet, y en el CDC no hay una excepción expresa para el contenido digital ya consumido. No reconocerlo expone a reclamaciones en los Procon y ante la ANPD/consumo, aunque en la práctica los reembolsos de Play los gestiona Google (su política de reembolsos, NO VERIFICADA aquí).
- **Decreto 7.962/2013** (comercio electrónico), texto de la publicación original: https://www2.camara.leg.br/legin/fed/decret/2013/decreto-7962-15-marco-2013-775557-publicacaooriginal-139266-pe.html . La ficha del Senado no muestra cambios posteriores, pero **NO VERIFICADO** en un texto compilado actual.
  - **Art. 2:** los sitios y medios electrónicos de oferta deben mostrar «em local de destaque»: «I - nome empresarial e número de inscrição do fornecedor, **quando houver**, no Cadastro Nacional de Pessoas Físicas ou no Cadastro Nacional de Pessoas Jurídicas»; «II - **endereço físico** e eletrônico»; III-VI: características, gastos añadidos, condiciones completas de la oferta y restricciones.
  - Art. 4: resumen del contrato antes de contratar, confirmación inmediata, contrato conservable, atención electrónica y «V [...] parágrafo único [...] manifestação do fornecedor [...] em até **cinco dias**».
  - Art. 5: informar de cómo ejercer el arrepentimiento.
- **¿Se aplica a un proveedor extranjero que vende por Google Play? DUDA ABIERTA (interpretación):** el decreto regula el CDC para la «contratação no comércio eletrônico» con consumidores en Brasil. Nada lo limita a proveedores establecidos allí, y el CPF/CNPJ se pide «quando houver», cosa que un extranjero sin inscripción no tiene. Que en la tienda el vendedor formal, o «merchant of record», sea Google o el desarrollador es un hecho de Google Play que **no se ha verificado** (NO VERIFICADO). Si el vendedor es el desarrollador, falta al menos la **dirección física** (art. 2 II): hoy los textos solo dicen «España». Mostrar la dirección exige pensar en la privacidad del propietario, por ejemplo con un domicilio profesional; decisión suya. El plazo de 5 días para las demandas por el canal (art. 4 parágrafo único) también aplicaría.

## 8. ECA Digital (Lei 15.211, de 17-09-2025)
Fuentes: publicación original (DOU, ed. extra A, 17-09-2025), https://www2.camara.leg.br/legin/fed/lei/2025/lei-15211-17-setembro-2025-797997-publicacaooriginal-176498-pl.html ; ficha con sus cambios, https://www2.camara.leg.br/legin/fed/lei/2025/lei-15211-17-setembro-2025-797997-norma-pl.html ; reglamento: **Decreto 12.880, de 18-03-2026** (en vigor al publicarse, art. 54), https://www2.camara.leg.br/legin/fed/decret/2026/decreto-12880-18-marco-2026-798813-publicacaooriginal-178481-pe.html .
- **Vigencia: 17-03-2026.** La Lei 15.352/2026, art. 19, añade el «Art. 41-A. Esta Lei entra em vigor em 17 de março de 2026» y su art. 20 revoca la MP 1.319/2025. La ficha registra además una **Lei 15.504, de 15-09-2026**, que añade un art. 36-A: **contenido NO VERIFICADO**.
- **Ámbito, art. 1:** «aplica-se a todo produto ou serviço de tecnologia da informação **direcionado** a crianças e a adolescentes no País **ou de acesso provável por eles**, independentemente de sua localização, desenvolvimento, [...] oferta». Parágrafo único: el acceso es probable cuando hay «I - suficiente probabilidade de uso e **atratividade** [...]; II - considerável **facilidade ao acesso** e utilização [...]; e III - significativo grau de risco à privacidade, à segurança ou ao desenvolvimento biopsicossocial [...]». El art. 2 I incluye expresamente las «aplicações de internet» y los «jogos eletrônicos».
- **¿Afecta a VIDA? DUDA SERIA (interpretación).**
  - A favor de que no: VIDA «no se dirige a menores» y no tiene red social ni chat entre usuarios.
  - En contra: es un **juego de rol con arte pixel, gratis, sin cuentas ni control de edad**, así que tiene atractivo y facilidad de acceso para adolescentes (incisos I y II). El inciso III (riesgo significativo) es más discutible: no hay interacción entre usuarios, pero sí un Coach IA, compras y anuncios. La redacción («as seguintes situações», I, II «e» III) sugiere que hacen falta los tres. Las guías de despachos lo leen de varias formas y **no hay criterio de la ANPD que se haya podido verificar**.
- **Si se aplicara** (obligaciones verificadas en el texto):
  - arts. 3, 5-8: protección por defecto y gestión de riesgos;
  - art. 14: recibir la señal de edad que den la tienda o el sistema (art. 12) e impedir el acceso a contenidos inadecuados para la edad;
  - arts. 16-18: supervisión parental, también para «restringir compras e transações financeiras» (art. 18 II);
  - art. 22: prohibido el perfilado para publicidad a menores;
  - art. 20: prohibidas las «caixas de recompensa» de pago y aleatorias en juegos para menores o de acceso probable. Los cofres de VIDA no se compran y los créditos no son aleatorios, así que no parece afectar.
  - **Art. 40: «deverão manter representante legal no País»** con poderes para recibir citaciones y notificaciones.
  - Decreto 12.880, art. 9 parágrafo único: considera mecanismos de uso compulsivo «III - a oferta de **recompensas pelo tiempo de uso**» y «IV - o aparecimento de **notificações excessivas**». Las rachas, los cofres de constancia y los recordatorios merecen una revisión, en clave de riesgo. Art. 11: a los asistentes de lenguaje natural (el Coach) les exige transparencia sobre su carácter automatizado y una evaluación de riesgos.
  - Sanciones (art. 35 II): sin facturación en Brasil, «multa de R$ 10,00 [...] até R$ 1.000,00 [...] por usuário cadastrado», con tope de R$ 50 M por infracción. La autoridad es la ANPD (según la ficha de la Câmara, Decreto 12.622/2025).
- **Recomendación:** dejar documentado en un informe interno **por qué VIDA no es de «acceso probable»**: público adulto declarado; clasificación por edades en Play para adultos, si es así (NO VERIFICADO); sin interacción entre usuarios; sin publicidad perfilada a menores. Valorar además una puerta de edad declarada y usar la señal de edad de Google Play cuando exista. Que la política diga con claridad que la app es para mayores de 18 años. Si el propietario concluye que sí aplica, el representante en Brasil (art. 40) es obligatorio y caro: es una decisión suya.

---

## Propuesta de apartado LGPD para la política (español, esquemático; va también en PT, y en PT es obligatorio el bloque de transferencias)

**«Si estás en Brasil (LGPD — Lei nº 13.709/2018)»**

1. **Quién trata tus datos (controlador):** Alex Vida, desarrollador independiente (persona física), España. Sin establecimiento en Brasil. Se considera agente de tratamiento de pequeño porte (Res. CD/ANPD nº 2/2022) y no ha nombrado encarregado. **Canal de comunicación** para titulares y para la ANPD: vidarpgapp@gmail.com, en portugués o en español.
2. **Qué datos, para qué y con qué base** (art. 7 y 11):
   - Coach IA: el resumen de objetivos, hábitos y vicios y el código de país, para responder lo que pides. Base: tu **consentimiento específico y destacado** antes de la primera consulta, porque los vicios pueden revelar datos de salud (art. 11 I), y la ejecución del servicio pedido (art. 7 V). Revocable cuando quieras: dejando de usar el Coach, sin que pierdas nada más.
   - Antiabuso: huella salada de la IP y un ID aleatorio de instalación, durante 1 día. Base: interés legítimo (art. 7 IX) en evitar abusos del servicio gratuito.
   - Anuncios bonificados que pides: Google AdMob recibe la IP, el identificador de publicidad y datos del dispositivo. Base: consentimiento (art. 7 I; Marco Civil art. 7 VII). Sin él no hay anuncio y el resto funciona igual.
   - Compras, créditos y códigos: el recibo, el ID anónimo de RevenueCat, el número de pedido, las fechas y el saldo. Base: ejecución del contrato (art. 7 V) y defensa en reclamaciones (art. 7 VI).
   - Health Connect, la foto y la partida: nunca salen del teléfono, así que el desarrollador no los trata.
3. **Cuánto tiempo:** el contenido del Coach no se guarda; la huella, 1 día; el saldo y el registro de créditos, hasta 24 meses sin actividad o hasta que pidas el borrado; de lo demás, nada en servidores propios. Google y RevenueCat conservan los datos según sus propias políticas (enlaces).
4. **Con quién se comparte y qué responsabilidad tiene cada uno** (art. 9 V-VI): Cloudflare, Inc. (EE. UU.), operador que aloja el servidor y el modelo de IA; RevenueCat, Inc. (EE. UU.), operador de compras; Google (AdMob y Google Play), que trata como controlador independiente lo que recibe para el anuncio o el cobro. No se venden datos.
5. **Transferencias internacionales** (art. 33; Res. ANPD 19/2024 art. 17): destinos, la **España y la UE**, reconocida como adecuada por la ANPD (Res. CD/ANPD nº 32/2026), y **EE. UU.** (Cloudflare, RevenueCat, Google), con su mecanismo: cláusulas-padrão de la ANPD donde las haya (Google; *pendiente con Cloudflare y RevenueCat*) o, si no, la necesidad para prestar el servicio pedido (art. 33 IX) y tu consentimiento específico (art. 33 VIII). Para cada uno: finalidad, duración y medidas de seguridad. Copia de las cláusulas a quien la pida, **en 15 días**.
6. **Tus derechos (art. 18), con su nombre:** confirmación de que hay tratamiento; acceso; corrección; anonimización, bloqueo o eliminación de lo innecesario, excesivo o ilícito; portabilidad; eliminación de lo tratado con consentimiento; información de con quién se compartió; información sobre la posibilidad de no consentir y sus consecuencias; revocación del consentimiento; oposición (art. 18 § 2º). Gratis (art. 18 § 5º).
7. **Cómo ejercerlos y en qué plazo:** casi todo dentro de la app (exportar, editar, reiniciar, desinstalar). Para los créditos u otra cosa, por correo a vidarpgapp@gmail.com, con el número de pedido `GPA.…` si toca: es lo único que permite saber de quién es el saldo, porque no hay cuentas. Respuesta en **15 días como máximo**.
8. **Reclamación:** si no te contestamos en plazo o no te convence la respuesta, puedes presentar una **petição de titular ante la ANPD (Agência Nacional de Proteção de Dados)** en https://www.gov.br/pt-br/servicos/abrir-requerimento-relacionado-a-lgpd, adjuntando la prueba de que nos escribiste (Res. CD/ANPD nº 1/2021, art. 25 § 1º), o acudir a los organismos de defensa del consumidor (Procon) (art. 18 § 8º).
9. **Menores:** la app es solo para mayores de 18 años; no se tratan conscientemente datos de menores (LGPD art. 14; ver ECA Digital, punto 8).

**Pendientes para los Términos o para la decisión del propietario:**
- **foro brasileño como alternativa** en los Términos (Marco Civil art. 8 parágrafo único II; CDC art. 101 I);
- condiciones de compra completas en PT (CDC art. 31);
- **dirección física** del proveedor si se le considera vendedor (Decreto 7.962 art. 2 II);
- mecanismo de transferencia con Cloudflare y RevenueCat (cláusulas ANPD);
- análisis documentado del ECA Digital («acesso provável», representante del art. 40);
- arrepentimiento de 7 días (CDC art. 49): riesgo asumido por decisión del propietario.
