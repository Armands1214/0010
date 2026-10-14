# Rīga kustībā — V2 / pakalpojumu sākumlapa

Saglabāts iepriekšējais tumšais un zaļais stils, tramvaja attēls un lokālie Manrope fonti.

## Kas mainīts
- index.html tagad ir pakalpojumu sākumlapa: biļetes, autostāvvietas, aktualitātes, informācijas bloki un kontakti.
- Maršrutu plānotājs, kustības saraksti un ģeogrāfiskā shēma pieejama tikai marsruti.html, nospiežot “Maršruti un laiki”.
- Sākumlapa neielādē transporta datu failus vai maršrutu lietotni.
- Mobilā izvēlne pieejama abās lapās.
- Ziņu virsraksti un datumi pārņemti no lietotāja pievienotā attēla un ir skaidri marķēti kā paraugi, nevis aktuāla ziņu plūsma.

## Ja iepriekšējā GitHub versija jau darbojas
Nav jāpārvieto jau strādājošās mapes. Repozitorija saknē:
1. Aizstāj index.html un style.css ar šī arhīva versijām.
2. Pievieno marsruti.html un navigation.js.
3. Saglabā izmaiņas ar Commit changes.

app.js, assets/ un data/ ir saglabāti no iepriekšējā komplekta. Ja tie jau augšupielādēti pareizi, nav jāaugšupielādē vēlreiz. README.md var arī aizstāt. Pēc publicēšanas pārlādē lapu; ja redzi veco izskatu, izmanto pārlūka piespiedu atsvaidzināšanu.

## Jauna repozitorija publicēšana
1. Atarhivē ZIP.
2. Augšupielādē tā saturu GitHub, saglabājot assets/ un data/ mapes. Neaugšupielādē pašu ZIP.
3. index.html, marsruti.html, style.css, app.js un navigation.js jāatrodas repozitorija saknē.
4. Settings → Pages → Deploy from a branch → main → / (root) → Save.
5. Sagaidi publicēšanu; vietnes adrese būs redzama Pages sadaļā.

Visi lokālie resursu ceļi ir relatīvi, tāpēc lapa darbojas arī github.io/REPOZITORIJS/ adresē. Nav vajadzīga būvēšana vai Node.js. Saglabā arī .nojekyll, ja tas redzams datorā.

## Apskate datorā
Sākumlapa ar dizainu un izvēlnēm darbojas, atverot index.html. Maršrutu datu ielādei izmanto HTTP serveri, piemēram, ja datorā ir Python:

python -m http.server 8000

Tad atver http://localhost:8000. Publicētajai GitHub Pages lapai lokāls serveris nav vajadzīgs.

## Pārbaudes
Pārbaudīta abu JavaScript failu sintakse, abu lapu iekšējās saites un enkuri, CSS resursu esamība, maršrutu lietotnes vajadzīgo elementu esamība atsevišķajā lapā un to neesamība sākumlapā. Pārlūkā veikta vizuālā pārbaude šajā izstrādes vidē nebija pieejama.

## Piezīmes
Neoficiāls dizaina prototips. Tramvaja attēls ir AI ilustrācija. Biļešu un autostāvvietu oficiālās informācijas saites atver Rīgas satiksmes vietni. Par mums, sadarbības un vakanču saites ved uz oficiālās vietnes sākumlapu, nevis atsevišķām šī prototipa sadaļām. Nav reāllaika GPS datu vai braucienu aprēķina ar pārsēšanos.
