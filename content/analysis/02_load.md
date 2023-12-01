---
Title: Load kmom05
Description: Rapport om ??
Template: analysis
---

Laddningstid och användbarhet
=======================

Den här rapporten kommer att undersöka hur laddningstider för tre olika webbplatser relaterade till golfindustrin ser ut. Det kommer även att noteras potentiella förbättringar när det kommer till laddningstid och användbarhet.

Urval
-----------------------
De tre webbplatser som kommer att undersökas är relaterade till golfindustrin och har valts ut eftersom att de har en personlig anknytning till författaren.
Webbplatserna är:
- https://teeview.se/
- http://tabygk.se/
- https://golf.se/


Metod
-----------------------

För varje webbplats, görs följande:

    1. En snapshot (bild) tas av webbplatsen.
    2. Google Pagespeed används för att mäta både Mobile och Desktop varianter av webbplatsen. Betygen noteras.
    3. Firefox devtools flik networks används för att notera sidans laddningstid tillsammans med antalet resurser som laddas samt sidans totala storlek. Mätningen görs tre gånger och snittet av mätvärdena används.
    4. Resultaten för webbplatsen diskuteras.


Resultat
-----------------------

<iframe class="loadiframe" src="https://docs.google.com/spreadsheets/d/e/2PACX-1vSPWZ7FHMb5LnaD5GHX6h2KHbirN_GC5G1n2VbXO-ie2yR1-xBQIDYf9h99Cka38FfBPpTT0s0gQDYH/pubhtml?gid=0&amp;single=true&amp;widget=true&amp;headers=false"></iframe>

### teeview.se
En av de största bristerna för webbplatsen tycks vara dess prestanda på mobila enheter. En stor anledning till detta verkar vara att storleken på bilderna som laddas in inte minskar på den mindre skärmstorleken. Att ändra filformat på bilderna till WebP eller AVIF är också en stor prestanda möjlighet. Bilders Cache Time To Live tycks också vara icke-existerande i många fall. Utöver detta är också tillgängligheten bristande då många bilder saknar alt texter. 

### tabygk.se
På tabygk.se ser vi stora brister i prestanda på både mobil och desktop. Den största punkten verkar vara en facebook widget som både laddar in mycket data och mycket oanvänd javascript. Utöver detta är också tillgängligheten bristande då många bilder saknar alt texter.

### golf.se
Här finns stora brister i prestanda på både mobil och desktop. Sidan behöver vänta på en hel del både första- och tredjeparts kod som blockerar första rendreringen av sidan. På den här sidan finns det alt text till bilderna villket är bra för tillgängligheten.


Analys
-----------------------
Genomgående för samtliga webbplatser var att prestandan var bristande, framförallt för mobila enheter. De primära punkterna som påverkar prestandan negativt tycks variera en del mellan webbplatserna. För de två webbplatserna som tillhör mindre företag, teeview.se och tabygk.se, så brister tillgängligheten för bilder då de saknar alt textern. Medan för det större företaget, golf.se, finns det alt texter. Möjligen kan detta bero på högre krav på tillgänglighet för webbplatser med mer traffik.

Övrigt
-----------------------
Martin Granstad