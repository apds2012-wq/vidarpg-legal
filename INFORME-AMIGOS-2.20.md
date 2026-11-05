# Informe · web legal para «Amigos» (2.20)

Fecha: 5 de noviembre de 2026 · rama `claude/amigos-legal-datos-14htil` (desde `origin/claude/quitar-12-paises`, cuyo cambio se conserva) · **sin publicar ni fusionar**.
Fuentes: `docs/diseno/AMIGOS-2.20.md` y `docs/diseno/amigos/API.md` (rama `claude/amigos-servidor` de `apds2012-wq/vida`, leídos el 05-11-2026) y las decisiones del propietario. Donde el diseño y las decisiones difieren, mandan las decisiones (nombre libre con filtro, solo PRO, premio de un mes, sin casilla de edad).

## 1. Qué cambia en cada página (8 idiomas)

| Página | Cambio |
|---|---|
| **Política de privacidad** | Fecha 5-11-2026 y versión 2.20.0. **Sección nueva «12 bis. Amigos y retos compartidos»** (qué sale, qué no, quién lo ve, códigos, solo PRO, premio y RevenueCat, nombres, denuncias y bloqueos, plazos, dónde se guarda). Ajustes en: descripción, entrada, §1 resumen, §2 datos locales, §3 dónde se guardan, §4 lo que no hace, §7 exportar, §8 el Coach nunca recibe lo de Amigos, §14 permisos, §15 derechos, §16 menores (18+, «Restringir el acceso de menores»), §17 desinstalar, §20.1 (3 filas nuevas y 1 ampliada), §20.2 (Cloudflare y RevenueCat; **sin prometer Europa**), §20.3, §20.4 (LGPD), §20.5 (Rusia), §20.6 |
| **Eliminación de datos** | Sección nueva 4 «Borrar lo que compartes en Amigos» (tabla: dejar de compartir, borrar todo, salir de un reto, no hacer nada, bloquear y denunciar; qué hacer sin la app; lo que no se puede borrar). Secciones siguientes renumeradas 5-7 |
| **Términos de uso** | Sección nueva 11 «Amigos y retos compartidos» (solo adultos, reglas de uso, premio, **canal de aviso por correo y por la app**, **por qué se quita una tarjeta**, sin garantías). Siguientes renumeradas 12-14 |
| Índice y soporte | Frases que habrían quedado falsas («todo está en tu teléfono», «no queda nada en ningún servidor»); en soporte, una pregunta nueva sobre Amigos |

La numeración de la política **no cambia**: la sección nueva es «12 bis» en los 8 idiomas para no romper las referencias entre secciones.

## 2. Revisión independiente
Un revisor sin conocimiento de la app leyó las tres páginas en español y dio 38 observaciones. Se aplicaron las que no obligaban a inventar reglas (frases absolutas como «exclusivamente», aviso de «Borrar todo lo mío» antes de desinstalar, glosario, menores, 112, plazo de 15 días en derechos, verificación de identidad por correo) y después se ajustó todo al contrato publicado (denuncias en lista cerrada, 180 días, premio con 24 de 30 días, solo PRO, límites). Se propagó a los 7 idiomas restantes.

## 3. Afirmaciones del texto que **tienen que cumplir** la app y el servidor
Si el código se aparta, hay que cambiar el texto o el código:
1. Registros de Cloudflare apagados (API.md §0 lo dice).
2. Borrado a los 90 días sin uso, reto a los 30 días tras terminar, código 48 h (API.md §5).
3. «Dejar de compartir», «Borrar todo lo mío» y «Salir» del reto: al momento (API.md).
4. El nombre anterior se guarda 30 días; las denuncias, 180 días tras cerrarlas.
5. **El Coach nunca recibe nada de Amigos**: `s.amigos` en `COACH_FORBIDDEN_LOCAL_KEYS` y `requestLeaks` (API.md §7 lo pide a la app).
6. El identificador y la llave no viajan al exportar y quedan fuera de la partida.
7. «Reiniciar partida» y desinstalar **no** borran lo del servidor: si la app ofrece borrarlo al reiniciar, hay que ajustar la eliminación de datos (§3) y la política (12 bis).
8. Botón «Salir» del reto, «Bloquear», «Denunciar» y «Borrar todo lo mío» con esos nombres (los rótulos de cada idioma son traducción nuestra: contrastarlos con los de la app).

## 4. Decisiones y huecos para el propietario
| Tema | Estado |
|---|---|
| **¿Solo Europa?** | **No confirmado.** El contrato no dice nada de la jurisdicción de Cloudflare. El texto dice «No garantizamos que los datos de Amigos se guarden solo en Europa». Si se activa `eu` y se verifica, se cambia |
| Borrado por correo sin la app | El servidor solo borra por `id` (`POST /admin/borrar { id }`), y el propietario no conoce el `id` de quien escribe. El texto promete borrar «lo que podamos identificar con seguridad» y, si no, el borrado a los 90 días. Falta una ruta de administración por nombre o por la «marca» de 4 símbolos, o aceptar solo el plazo |
| **EXP total y Health Connect** | La EXP total suma también la de pasos y carreras. El texto lo dice con claridad y afirma que no sale ningún dato de Health Connect. Es un matiz que el propietario debe aceptar |
| Base jurídica | Art. 6.1.b (la función que activas) para la tarjeta y los retos; 6.1.f para antiabuso y denuncias. Pendiente de confirmar por quien lleve lo legal |
| Punto de contacto y DSA | El texto da canal de aviso (correo y app), motivos y revisión humana en 15 días, sin afirmar que Amigos sea «plataforma en línea» |
| Plazo para atender una denuncia | No se promete; se dice que no es un servicio de emergencias (112) |
| Premio | Solo suscripción de Google Play, una vez por reto y persona, no si el PRO viene de un código; si no puede aplicarse, no se sustituye por otra cosa (decisión redactada aquí: confirmar) |
| Si se acaba PRO | Lo ya creado sigue; no se añaden amigos ni retos (API.md §0.2) |
| `soporte.html` y su fecha | La cabecera sigue en 2.17.0 (octubre): solo se tocaron las respuestas que se habían quedado falsas. Conviene una pasada completa con la 2.20 |
| Nombres de la función | Amigos · Friends · Znajomi · Amis · Freunde · Amici · Друзья · Amigos: contrastar con la app |

## 5. Pasos para publicar (los hace el propietario desde el PC)
1. Revisar y fusionar la rama; publicar GitHub Pages.
2. Comprobar que las URL de borrado de los 8 idiomas cargan antes de enviarlas a Play Console (ver `docs/play/PLAY-AMIGOS.md` en la rama `claude/amigos-legal-app` de `vida`).
