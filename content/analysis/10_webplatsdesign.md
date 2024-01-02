---
Title: Design principles kmom10
Description: Rapport om aktuella trender i webbdesign
Template: analysis
---

Trender inom tillgänglighet i webbdesign för golfklubbar i norra Stockholm
=======================

I rapporten kommer tre olika golfklubbars i norra Stockholms webbsidor att väljas ut, analyseras och jämföras när det kommer till att ha tillgänglighet i åtanke vid designen. Frågan "Finns det någon nuvarande trend bland golfklubbar i norra Stockholm när det kommer till att ta tillgänglighet i åtanke när de designar sina webbsidor?" kommer att besvaras.

Urval
-----------------------

Urvalet gjordes genom att tre av de största golfklubbarna i norra Stockholm valdes ut.

Metod
-----------------------

Metoden som användes för att analysera sidorna fortskred enligt följande (per sida): 
1. Webbplatsens accessibility score i verktyget Lighthouse mäts och noteras.
2. Om Lighthouse pekar ut några problem så noteras dem.
3. Ett test hur det fungerar att navigera på webbplatsen med hjälp av TAB görs och resultatet noteras.
4. Författaren gör en subjektiv bedömning om det finns något ytterligare att notera kring tillgängligheten på en skala 0-100.

Slutligen utförs en jämförelse av de olika sidorna med avsikten att besvara frågan "Finns det någon nuvarande trend bland golfklubbar i norra Stockholm när det kommer till att ta tillgänglighet i åtanke när de designar sina webbsidor?".

Resultat
-----------------------

### https://www.ostgk.se/se
Webbplatsens accessibility score i verktyget Lighthouse uppmättes till 87.
Lighthouse anmärkningar var följande.
1. [aria-hidden="true"] elements contain focusable descendents
2. Links do not have a discernible name
3. Heading elements are not in a sequentially-descending order

Det går inte helt att navigera på sidan med enbart TAB. Huvudnavigationen fungerar med TAB men som Lighthouse första notering säger så finns det en kalender där det inte går att byta vecka med enbart TAB. Den djupt nästlade navigationen gör det dock till en påfrestande process. Det går på många ställen inte att se vart på sidan man befinner sig.

Sidan borde också ha en lägre score i Lighthouse. Det finns ett alt attribut på bilderna men de innehåller ingen faktiskt beskriving. Detta resulterar i att Lighthouse inte reagerar på det men det ger ingen hjälp till personen som behöver alt texten.

Lighthouse klagar inte på kontrasten för brödtexten men jag upplever personligen att den är väldigt svårläst och hade gärna sett mer kontrast.

Det finns också en del text som ligger i bilder vilket gör att den inte kan läsas utan att se bilderna.

Webbplatsen får sammantaget 65 i betyg för tillgängligheten. Detta eftersom att den brast på fler sätt än Lighthouse plockade ut.

### http://tabygk.se/se
Webbplatsens accessibility score i verktyget Lighthouse uppmättes till 86.
Lighthouse anmärkningar var följande.
1. Image elements do not have [alt] attributes
2. Links do not have a discernible name

Det går att navigera på sidan med endast TAB. Den djupt nästlade navigationen gör det dock till en påfrestande process. Det går på många ställen inte att se vart på sidan man befinner sig.

Webbplatsen får sammantaget 80 i betyg för tillgängligheten. Detta eftersom att den endast brast på något fler sätt än Lighthouse plockade ut.

### https://arningegk.se/
Webbplatsens accessibility score i verktyget Lighthouse uppmättes till 96.
Lighthouse anmärkningar var följande.
1. Links do not have a discernible name

Det går att navigera på sidan med endast TAB. Den djupt nästlade navigationen gör det dock till en påfrestande process. Det går på många ställen inte att se vart på sidan man befinner sig.

Sidan borde också ha en lägre score i Lighthouse. Det finns ett alt attribut på bilderna men de innehåller ingen faktiskt beskriving. Detta resulterar i att Lighthouse inte reagerar på det men det ger ingen hjälp till personen som behöver alt texten.

Det finns också en del text som ligger i bilder vilket gör att den inte kan läsas utan att se bilderna.

Webbplatsen får sammantaget 80 i betyg för tillgängligheten. Detta eftersom att den endast brast på många fler sätt än Lighthouse plockade ut.


Analys
-----------------------
Ingen av sidorna använde sig av alt-texter på ett tillfredställande vis. Samtliga föll på beskrivande länknamn. Samtliga gjorde det svårt att navigera med TAB. Övergripande går det alltså att göra slutsatsen att för detta urvalet av sidor så tycks inte tillgänglighet varit av högsta fokus.

Dessa tre golfklubbar är endast ett urval av det tiotal golfklubbar som finns i norra Stockholm men frågan "Finns det någon nuvarande trend bland golfklubbar i norra Stockholm när det kommer till att ta tillgänglighet i åtanke när de designar sina webbsidor?" bör i alla fall kunna besvaras som att det finns en trend hos åtminsone somliga av klubbarna att inte prioritera tillgänglighet på sina webbsidor.

Vidare går det att problematisera att Lighthouse missar att bilder har tomma alt attribut. Att tomma alt-attribut har lagts till för att lura sökmotorer att sidan har bättre tillgänglighet än den faktiskt har skulle kunna vara en möjlighet eller så handlar det bara om bristande kompetens eller slarv. Undersökningen visar också att det är viktigt att inte bara se till Lighthouse-score när en sidas tillgänglighet ska bedömas.

En möjlig anledning till varför webbsidorna brister i tillgänglighet skulle kunna vara att andelen av deras kundbas som behöver tillgänglighetsanpassning är lägre än för många andra webbsidor. Det blir svårare att spela golf med en funktionsvariation likt blindhet vilket minskar sannolikheten för att dessa personer är intresserad av innehållet på sidan.


Övrigt
-----------------------

Av Martin Granstad