# DAM1M04-Exercici004 — Strata

Reproducció acadèmica de la pàgina de Strata amb HTML i CSS.

## Estat del projecte

La branca `capcalera-hero` inclou la pàgina completa: Hero, Platform, Operational Value, From the Field, Workflows, Atlas, Governance, Get Started i peu. Es conserva el desenvolupament anterior en l’historial. No s’ha fusionat amb `main`.

## Com obrir el projecte

A la branca de treball, obre `index.html` amb Live Server de Visual Studio Code.

## Fonts locals

Les fonts del ZIP de l'exercici es troben a `assets/fonts` i es carreguen abans d'`estils.css`.

- Plus Jakarta Sans per al text principal i els títols.
- JetBrains Mono per a les classes `etiqueta` i `dada`, utilitzades en les seccions.

Es conserven les llicències OFL de les dues famílies dins de la mateixa carpeta. No cal Google Fonts ni connexió a Internet per carregar-les.

## Maquetació i adaptació

HTML semàntic, un sol `h1`, CSS extern i Flexbox, sense Grid ni JavaScript propi. El contenidor té una amplada màxima i marges automàtics. Els enllaços tenen estats hover i focus-visible.

Sota 1000 px, Governance passa a dues columnes, la consulta d’Atlas ocupa una fila pròpia i es redueixen les xifres grans per donar més espai al text. Sota 768 px, les seccions passen a una columna, es redueixen títols i espaiats, s’amaga el gràfic del hero i els enllaços del peu poden saltar de línia. La captura de Nexus es retalla visualment en mòbil, conservant la proporció.

## Capçalera

El logotip i la icona provenen del ZIP de l'exercici i es carreguen des d'`assets/img`. La capçalera es manté visible amb `position: sticky`. En mòbil s'amaga la navegació central i queda visible el botó «Book a Demo». L'avís d'ILTACON reprodueix el text de la captura de referència.

## Hero inicial

El títol, el paràgraf i els dos enllaços segueixen `referencies/textos.txt` del ZIP. El fons i la paraula «done» es construeixen amb degradats CSS. La mida del títol es redueix per sota de 768 px i els enllaços es distribueixen amb Flexbox.

La captura de Nexus es carrega des d'`assets/img/nexus-screenshot.webp`, sense modificar el fitxer del ZIP. La imatge conserva la proporció original. En mòbil, el contenidor mostra només la part superior de la captura, com a la referència, sense deformar-la.

S'han incorporat els scripts facilitats per al fons animat. S'han comprovat els recursos amb un servidor local; la comparació visual en navegador queda pendent.

## Animació del hero

El ZIP facilita `hero-graph.js`, descarregat de [Strata](https://www.strata.ai/hero-graph.js) el 19/10/2026. Es conserva sense modificacions. Segons `referencies/animacio-origen.txt`, el script original no inclou una declaració de llicència oberta.

També es conserven sense modificacions les dues biblioteques facilitades:

- Three.js r149, procedent de `https://www.strata.ai/assets/vendor/three.min.js`. Projecte: [Three.js](https://github.com/mrdoob/three.js). Llicència MIT completa a `assets/js/vendor/three-LICENSE.txt`.
- 3d-force-graph 1.73.4, procedent de `https://www.strata.ai/assets/vendor/3d-force-graph.min.js`. Projecte: [3d-force-graph](https://github.com/vasturiano/3d-force-graph). Llicència MIT completa a `assets/js/vendor/3d-force-graph-LICENSE.txt`.

Les llicències MIT corresponen a les biblioteques, no al script original de Strata. Tots tres scripts es carreguen localment, en aquest ordre i amb `defer`. No s'ha escrit JavaScript propi.

El script crea el canvas automàticament dins de `.hero`; el contingut de `.hero > .container` queda en una capa superior. El gràfic no intercepta els clics i s'amaga per sota de 768 px o quan es prefereix reduir el moviment, mantenint el degradat CSS. En passar de mòbil a escriptori, cal recarregar per iniciar el gràfic.

S'han comprovat les rutes, l'ordre, la sintaxi dels scripts i la coincidència amb els fitxers del ZIP. El funcionament visual amb WebGL i la prova en les amplades de referència queden pendents.

## Platform

Les targetes Atlas, Nexus i Canvas fan servir Flexbox i els textos de `referencies/textos.txt`. En escriptori es reparteixen en tres columnes i, sota 768 px, passen a una sola columna. La franja de Core també passa d'una fila a una disposició vertical. Els colors i les mides parteixen de les captures del ZIP; la comparació visual de la pàgina en un navegador queda pendent.

## Operational Value

La franja de missatge utilitza degradats CSS i els dos textos de la referència. El panell mostra les dades il·lustratives estàtiques de la captura: 428.610 dòlars recuperats (+18% MoM) i 1.284 hores de capacitat (aproximadament 12 setmanes equivalents a jornada completa). No són dades reals del projecte ni comptadors en directe. Les mètriques passen de dues columnes Flexbox a una sota 768 px; en tauleta es redueix la mida de les xifres.

## From the Field

La secció fosca reprodueix el cas i les dades de la referència de Strata: 13.000 factures mensuals, 19 portals, un cicle de 4–6 setmanes, un equip de 5–7 persones i cap recurs enviat automàticament. És contingut estàtic del material acadèmic. El text i la fitxa es distribueixen amb Flexbox i passen a una sola columna sota 768 px. La fitxa fa servir una llista de definicions per relacionar cada etiqueta amb la seva dada.

## Workflows

La llista inclou els sis serveis del material de referència, amb etiquetes, separadors i fletxes. Invoice appeals apareix com a subapartat visual d'Invoice management. Les files i la navegació són accessibles amb el teclat; els serveis apunten al bloc final de la mateixa pàgina, sense crear pàgines addicionals. Les files Flexbox passen a una distribució vertical en mòbil.

## Atlas

La secció incorpora la captura local d'Atlas, els quatre passos i els dos nodes amb els textos del ZIP. La consulta és una representació estàtica de l'exemple de la captura: no envia preguntes ni té un botó interactiu. Els nodes també es representen estàticament, sense editar dades reals. La imatge conserva la proporció i els passos, la consulta i les targetes passen a una columna en mòbil. La icona de cerca i la marca de confirmació també són recursos locals del ZIP.

## Governance

S'han reproduït les quatre targetes, la seqüència numerada d'una execució i la franja de garanties amb els textos del material de referència. Les targetes i els passos es distribueixen amb Flexbox i passen a una columna sota 768 px. Els quatre passos s'estructuren amb una llista ordenada i les garanties amb una llista. Són continguts de la reproducció acadèmica, no funcionalitats de seguretat implementades per aquest projecte.

## Referència

[Enunciat de l'exercici](https://github.com/optimisme/DAM-LlenguatgeMarques/blob/main/02-Web/09-Exercici-Strata.md).

Els logotips, les imatges, els textos i el disseny de referència provenen de [Strata](https://www.strata.ai/). Aquest projecte és una reproducció acadèmica.

## Get Started i peu

Crida final, tres blocs de confiança i peu amb navegació interna, segons els textos i les captures del ZIP. En mòbil els blocs es col·loquen en columna i els enllaços del peu poden saltar de línia. Book a Demo porta al bloc final de la reproducció; no hi ha reserva de demos implementada.

## Comprovacions i límits

Revisió estàtica del HTML: estructura, un únic h1, identificadors únics, destins dels enllaços interns, atributs alt i existència dels recursos locals. Revisió del CSS: claus equilibrades, fonts locals, Flexbox sense Grid i regles de teclat, mòbil i moviment reduït. Scripts comprovats amb `node --check` i comparats byte a byte amb el ZIP, juntament amb les imatges i les fonts. Comprovació HTTP dels recursos locals amb servidor temporal.

La vista prèvia de navegador disponible havia fallat per timeout. No s’ha pogut verificar visualment a 1440, 768, 390 i 360 px ni executar WebGL; aquestes proves continuen pendents. La revisió de les regles responsive no substitueix aquestes proves. Les consultes, nodes i mètriques són estàtics.

No s’ha publicat a Proxmox ni Sites. La publicació a l’institut i l’aportació real del segon alumne continuen pendents; no s’atribueixen contribucions a altres persones.
