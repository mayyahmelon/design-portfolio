---
Title: 01_colors
Description: This is our color page.
Template: rapport
---

Colors
=======================

Uppgiften går ut på att analysera tre hemsidor och deras användning av färger och typografi. 

Urval
-----------------------

För att analysera tre hemsidor har jag valt utifrån tre olika kategorier. Detta för att jag ska kunna
se om det finns en gemensam användning utav färger och typografi oavsett användningsområde. De tre hemsidor jag har valt är följande:

ASOS - En populär hemsida som säljer kläder, accessoarer.

SVT Play - En media platform där man kan streama filmer och TV-program.

The Guardian - En nyhetssida.


Metod
-----------------------

De verktyg jag kommer att använda för att kunna analysera hemsidorna är främst "Inspect Element som finns inbyggd i min webbläsare, Opera GX. Jag kommer att kolla i HTML och CSS, och även använda av mig color-picker. 

Resultat
-----------------------
<h2> Asos </h2>

<img src="%assets_url%/img/Asos.jpg" alt="Asos" width="1000">

<h3>Färgpaletten</h3>
<table style="border-spacing: 4px; border-collapse: separate">
<tr>
<td style="height: 50px; width: 50px; background-color: #2d2d2d">
<td style="height: 50px; width: 50px; background-color: #525050">
<td style="height: 50px; width: 50px; background-color: #d01345">
<td style="height: 50px; width: 50px; background-color: #253a3d">
<td style="height: 50px; width: 50px; background-color: #eeeeee">
<td style="height: 50px; width: 50px; background-color: #ffffff">
</tr>
</table>

ASOS har ett monokromatiskt färgschema för basen med vit bakgrund och mörk/ljusgrå för navbaren. Sedan använder de röd och mörkgrön som är komplementeringsfärger. Den vita bakgrunden passar nog bäst för att bilderna ska kunna synas på det bästa sättet, neutralt. Sedan har vi den röda färgen som sätts där man vill dra mest uppmärksamhet, t.ex Black Friday deals och nedsatta pris. Fokuset är på kläderna som säljs, därför passar hemsidan med mörkgråa navbaren för det är inte något man ska "se".

<h3>Typsnitt</h3>

ASOS "body" tagg har font-style "futura-pt, Tahoma, Geneva, Verdana, Arial, sans-serif;".

All text som finns på hemsidan har font-stylen "futura-pt", vilket är ett san-serif typsnitt. H1 som man ser på bilden har storleken 24px. ASOS verkar inte ha någon andra header element. Texterna i navbaren är en a element med storleken 14px. Brödtexten under varje bild är samma.

<h3> Profil</h3>
ASOS val av färger och design passar hemsidans användningsområde, vilket är att sälja kläder och accessoarer. Fokuset ska vara på varorna och tack vare de färgerna ASOS valde, klaschar inte de med produkterna.

<h2> SVT Play </h2>

<img src="%assets_url%/img/SVT.jpg" alt="SVT" width="1000">

<h3>Färgpaletten</h3>
<table style="border-spacing: 4px; border-collapse: separate">
<tr>
<td style="height: 50px; width: 50px; background-color: #1b1614">
<td style="height: 50px; width: 50px; background-color: #b9232d">
<td style="height: 50px; width: 50px; background-color: #ffffff">
<td style="height: 50px; width: 50px; background-color: #211d1b">
<td style="height: 50px; width: 50px; background-color: #eeeeee">
<td style="height: 50px; width: 50px; background-color: #00c800">
</tr>
</table>

SVT play har en väldigt simpelt tema, mörk bakgrund med vit text. Monokromatisk färgschema. Vi har en röd färg som accent för att framhäva viktiga händelser som användaren inte kan missa! Nämligen "live" knappen. Gröna färgen är såklart SVTs egna logo.

<h3>Typsnitt</h3>

Hemsidan använder typsnittet "publik", i princip allt. Den enda header rubrik som används på framsidan är H2. Brödtexten har storlek 16 px.

<h3> Profil</h3>
Då det är en streaming site har de valt en bra mörkt tema. Användaren ska förmodligen känna sig själv som i bio, där lamporna släckts och filmen spelas. Dessutom har thumbnails massa olika galna färger, som kanske hade klaschat om inte bakgrundsfärgen var mörktgrå.

<h2> The Guardian </h2>

<img src="%assets_url%/img/guardian.jpg" alt="Guardian" width="1000">

<h3>Färgpaletten</h3>
<table style="border-spacing: 4px; border-collapse: separate">
<tr>
<td style="height: 50px; width: 50px; background-color: #052962">
<td style="height: 50px; width: 50px; background-color: #ffe500">
<td style="height: 50px; width: 50px; background-color: #ffffff">
<td style="height: 50px; width: 50px; background-color: #c70000">
<td style="height: 50px; width: 50px; background-color: #121212">
<td style="height: 50px; width: 50px; background-color: #ff5943">
</tr>
</table>

The Guardian är en nyhetssida med komplementfärgschema. Vi har blå header med gula accents, och en orange underline. Bakgrundfärgen är vit med en smal röd border runt aktuella händelser. En live rapportering markeras med en röd bakgrundfärg på rubriken.

<h3>Typsnitt</h3>
Jag kan tyvärr inte hitta typsnittet Guardian använder på framsidan, men det måste nog vara en 'serif' typ. Men ändå är det lättläst. Det beror nog också på koden som ligger i deras body:

    text-rendering: optimizeLegibility;
    font-feature-settings: 'kern';
    font-kerning: normal;
    font-variant-ligatures: common-ligatures;

I brödtexten i en artikel så används fonten "GuardianTextEgyptian". Line-height är satt på 1.4, vilket gör det mer läsbar. Storleken på brödtexten är 17px.

<h3> Profil</h3>

Fokuset för en hemsida som The Guardian borde väl vara läsbarheten. Artiklarna ska ha bra spacing och bra färger så att det inte skär i ögonen när man läser. Sedan är det väl viktig att få så många klicks som möjligt, därför har vi röda färgen som guidar ögonen att se.

Analys
-----------------------

De tre hemsidorna som är valda har olika användningar. Vi har ASOS som är en mode e-handel, SVT Play är en streamingtjänst och The Guardian som är en tidning.

De olika funktionerna till sidan avgör hur designen ska vara. För ASOS är det viktigt att produktbilderna framhävs. Produktbilderna kan innehålla massa olika färger och därför är en neutral bakgrund ett bra val. Men varför vit och inte mörkgrå som SVT-play? 

Det kan nog bero på att SVT play, som tidigare nämnt, är en streamingtjänst. En mörkare bakgrund kan jämföras med att vara på bio. Man vill ha det mysigt och mörkt när man kollar på TV, en stark vit bakgrund hade nog bländat många. ASOS och The Guardian vill man ha det ljust, att läsa och shoppa gör man inte i ett mörkt område. 

Men en gemensam faktor som dessa tre hemsidorna har, trots att de har olika funktioner, är deras användning utav färgen röd. Alla tre hemsidorna använder färgen röd för att markera något viktig. I ASOS är det för alla rabatterade pris och deals, i SVT play är det för live-tv och the guardian är det aktuella händelser.

Referenser
-----------------------

<ul>
<li><a href="https://webdesign.tutsplus.com/an-introduction-to-color-theory-for-web-designers--webdesign-1437a">An Introduction to Color Theory for Web Designers</a></li>
<li><a href="https://www.asos.com/se/kvinna/">ASOS</a></li>
<li><a href="https://www.svtplay.se">SVT Play</a></li>
<li><a href="https://www.theguardian.com/europe">The Guardian</a></li>

</ul>

Författare
-----------------------

Skriven av: Sumaiyyah Sumaiyyah
