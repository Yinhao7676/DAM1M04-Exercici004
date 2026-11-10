# DAM1M04-Exercici004 — Strata

Reproducció acadèmica de la pàgina de Strata amb HTML i CSS.

## Primer dia

- Preparació del repositori i de la branca `dia-1-reinicio`.
- Estructura inicial de la pàgina i navegació interna.
- Primers estils amb Flexbox i contenidor centrat.

És una base de treball: encara no reprodueix el disseny complet.

## Com obrir el projecte

A la branca de treball, obre `index.html` amb Live Server de Visual Studio Code.

## Fonts locals

Les fonts del ZIP de l'exercici es troben a `assets/fonts` i es carreguen abans d'`estils.css`.

- Plus Jakarta Sans per al text principal i els títols.
- JetBrains Mono per a les classes `etiqueta` i `dada`, que es faran servir en les seccions següents.

Es conserven les llicències OFL de les dues famílies dins de la mateixa carpeta. No cal Google Fonts ni connexió a Internet per carregar-les.

## Pendent

- Completar les imatges de producte del ZIP de l'exercici.
- Completar les seccions segons les captures de referència.
- Comprovar l'animació del hero en un navegador amb WebGL.
- Revisar la versió d'escriptori i mòbil.
- Completar els crèdits i les instruccions de publicació.

La maquetació es farà amb Flexbox, sense Grid ni JavaScript propi.

## Capçalera

El logotip i la icona provenen del ZIP de l'exercici i es carreguen des d'`assets/img`. La capçalera es manté visible amb `position: sticky`. En mòbil s'amaga la navegació central i queda visible el botó «Book a Demo». L'avís d'ILTACON reprodueix el text de la captura de referència.

## Hero inicial

El títol, el paràgraf i els dos enllaços segueixen `referencies/textos.txt` del ZIP. El fons i la paraula «done» es construeixen amb degradats CSS. La mida del títol es redueix per sota de 768 px i els enllaços es distribueixen amb Flexbox.

La captura de Nexus es carrega des d'`assets/img/nexus-screenshot.webp`, sense modificar el fitxer del ZIP. La imatge conserva la proporció original. En mòbil, el contenidor mostra només la part superior de la captura, com a la referència, sense deformar-la.

S'han incorporat els scripts facilitats per al fons animat. Aquesta versió encara no és una reproducció completa. S'han comprovat els recursos amb un servidor local; la comparació visual en navegador queda pendent.

## Animació del hero

El ZIP facilita `hero-graph.js`, descarregat de [Strata](https://www.strata.ai/hero-graph.js) el 19/10/2026. Es conserva sense modificacions. Segons `referencies/animacio-origen.txt`, el script original no inclou una declaració de llicència oberta.

També es conserven sense modificacions les dues biblioteques facilitades:

- Three.js r149, procedent de `https://www.strata.ai/assets/vendor/three.min.js`. Projecte: [Three.js](https://github.com/mrdoob/three.js). Llicència MIT completa a `assets/js/vendor/three-LICENSE.txt`.
- 3d-force-graph 1.73.4, procedent de `https://www.strata.ai/assets/vendor/3d-force-graph.min.js`. Projecte: [3d-force-graph](https://github.com/vasturiano/3d-force-graph). Llicència MIT completa a `assets/js/vendor/3d-force-graph-LICENSE.txt`.

Les llicències MIT corresponen a les biblioteques, no al script original de Strata. Tots tres scripts es carreguen localment, en aquest ordre i amb `defer`. No s'ha escrit JavaScript propi.

El script crea el canvas automàticament dins de `.hero`; el contingut de `.hero > .container` queda en una capa superior. El gràfic no intercepta els clics i s'amaga per sota de 768 px o quan es prefereix reduir el moviment, mantenint el degradat CSS. En passar de mòbil a escriptori, cal recarregar per iniciar el gràfic.

S'han comprovat les rutes, l'ordre, la sintaxi dels scripts i la coincidència amb els fitxers del ZIP. El funcionament visual amb WebGL i la prova en les amplades de referència queden pendents.

## Referència

[Enunciat de l'exercici](https://github.com/optimisme/DAM-LlenguatgeMarques/blob/main/02-Web/09-Exercici-Strata.md).

Els logotips, les imatges, els textos i el disseny de referència provenen de [Strata](https://www.strata.ai/). Aquest projecte és una reproducció acadèmica.
