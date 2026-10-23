# AGENTS.md — matechsolinf.ar

## Qué es este sitio
Sitio de Matech Soluciones Informáticas (matechsolinf.ar).
Servicios de ciberseguridad para PyMEs en Argentina.
Público: dueños y gerentes de PyMEs, NO perfiles técnicos.
Objetivo del sitio: que el visitante entienda el riesgo y pida una consulta.

## Reglas de contenido
- Escribir en español rioplatense, trato de "vos".
- Sin jerga técnica sin explicar. Si aparece un término (EDR, phishing,
  ransomware, MFA), explicarlo en una línea la primera vez que se usa.
- Tono: directo y sobrio. Nada de alarmismo ni de promesas absolutas
  ("protección total", "100% seguro"). Nunca citar estadísticas sin fuente.
- Cada página tiene que cerrar con una llamada a la acción clara.

## Reglas técnicas
- HTML y CSS planos. NO agregar frameworks, librerías externas,
  ni dependencias por CDN. El sitio tiene que funcionar sin JavaScript.
- NO tocar: CNAME, robots.txt, favicons, los archivos android-chrome-*.
- Si se agrega, borra o renombra una página: actualizar sitemap.xml
  en el mismo cambio, y revisar links internos que apunten a ella.
- Toda página nueva necesita <title> y <meta name="description">.
- El sitio se tiene que ver bien en celular. Probar siempre a 375px de ancho.
- Excepción a lo anterior: se permite el script de analítica web
  (Cloudflare Web Analytics). Ninguna otra dependencia externa.
- Formularios: se permite un endpoint externo de formularios
  (Formspree o similar). El sitio tiene que seguir siendo usable
  sin JavaScript en todo lo demás.

## Mensajes de commit
Describir qué cambió de verdad, en español, en una línea.
Bien: "Borra climatizacion.html y la saca del sitemap"
Mal: "Update print statement", "Add files via upload", "Changes"

## Fuera de alcance
El sitio ya NO es de climatización. Todo contenido de ese rubro
se elimina, no se actualiza.
