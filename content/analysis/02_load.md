---
Title: 02_load
Description: This is loading analysis.
Template: rapport
---

Loadings
=======================

Uppgiften går ut på att analysera tre hemsidor för att få värden på hur snabba sidorna laddas och få en överblick på saker som finns att förbättra.

Urval
-----------------------

De tre utvalda hemsidorna är IKEA, Amazon och en onlinebutik för sångerskan Sabrina Carpenter.
Tanken bakom valet utgår ifrån veckans kurs moment, bilder. En av de viktigaste delen för en online butik är bilderna på produkter som säljs. Att alla tre hemsidorna har en gemensam
funktion gör det lättare att presentera resultaten rättvist. 
<ul>
<li><a href="https://www.ikea.com/se/sv/">Ikea</a></li>
<li><a href="https://www.amazon.se">Amazon</a></li>
<li><a href="https://store.sabrinacarpenter.com">Sabrina Carpenter Merch</a></li>
</ul>

Metod
-----------------------
För att kunna genomföra och presentera resultaten kommer olika verktyg att användas.
Inbyggda PRNT funktionen för att kunna ta en skärmdumpning på hemsidan.
<a href="https://pagespeed.web.dev/?utm_source=psi&utm_medium=redirect"> PageSped Insights</a> för att få värden på hur snabba hemsidornas innehåll laddar. 
En inbyggd devtool för att mäta sidans laddningstid.
För att presentera resultaten används Google Kalkylark.

Resultat
-----------------------
<h2>IKEA</h2>

<img src="%assets_url%/img/IKEA.jpg" alt="Ikea" width="1000">

<h3>Presentation</h3>

<iframe src="https://docs.google.com/spreadsheets/d/e/2PACX-1vRRVKLfUPorIwjUefmgZlNEN_42nZjxD3DLbJQFl4rpkgqErl7J8vAIddIwHWpYnBlTPg5nKG6_LFUH/pubhtml?gid=0&amp;single=true&amp;widget=true&amp;headers=false" style="width: 900px;"></iframe>

Ikeas dator prestanda är inte särskilt hög, men inte låg heller. Framsidan fick poängen 84 där LCP är segast utav alla. Det tar 1,3 sekunder för LCP att ladda. LCP står för Largest contentful paint, alltså den största content element att synas på skärmen. Lösningen här är att förbättra JavaScripten, tiden det tar att tolka, kompilera och köra JavaScript kod tar enormt mängd av belastning på modertråden. 

<h2>Amazon</h2>

<img src="%assets_url%/img/Amazon.jpg" alt="Amazon" width="1000">

<h3>Presentation</h3>

<iframe src="https://docs.google.com/spreadsheets/d/e/2PACX-1vRRVKLfUPorIwjUefmgZlNEN_42nZjxD3DLbJQFl4rpkgqErl7J8vAIddIwHWpYnBlTPg5nKG6_LFUH/pubhtml?gid=785773594&amp;single=true&amp;widget=true&amp;headers=false" style="width: 900px;"></iframe>

Amazons mobilt prestanda är inte en prioritet trots att många ha börjat onlineshoppa på telefonen. Detta är för att de har en app just för att handla på telefonen. 
Men datorns presentanda ligger på en 87, vilket är en medelmåttig poäng att få. Kategorin som drar ner mest poäng är LCP, där det tar 1,2 sekunder för att laddas. Pagespeed
har diagnotiserat massor med koder som kan förbättras, bland de som nämns är att förbättra JavaScript som tar längst tid att köra. En till lösning är att ändra bildformaten till WebP och AVIF.

<h2>Sabrina Carpenter</h2>

<img src="%assets_url%/img/Sabrina.jpg" alt="Sabrina" width="1000">

<h3>Presentation</h3>

<iframe src="https://docs.google.com/spreadsheets/d/e/2PACX-1vRRVKLfUPorIwjUefmgZlNEN_42nZjxD3DLbJQFl4rpkgqErl7J8vAIddIwHWpYnBlTPg5nKG6_LFUH/pubhtml?gid=995731604&amp;single=true&amp;widget=true&amp;headers=false" style="width: 900px;"></iframe>

Sabrina Carpenters dator presentanda har fått 47 poäng, vilket är ett superlågt poäng att få, där medelsnabb prestanda ligger på 50-89 poäng. LCP ligger på 2,3 sekunder, men den sämsta sidan har fått är på CLS, vilket står för cumulative layout shift. Den ligger på 1,1, vilket är ett högt tal för CLS att få. Den kan ha negativa effekter på användarupplevelse, t.ex att elementen hoppar runt när man scrollar. Lösningar som nämns i Pagespeed diagnotiseringsdelen är att minska arbetsbelastningend på modertråden, förbättra JavaScriptet, och att undvika ett onödigt stort DOM träd.

Analys
-----------------------
De tre hemsidorna har en gemensam användningsområde där slutmålet är att trycka på varukorgen för att slutföra beställningen. Detta innebär att hemsidorna innehåller lockande bilder och användarvänliga funktioner. 

Tack vare resultaten kan vi se att ingen av hemsidorna fick högre än 89 på Pagespeed, skala 90-100 betyder att hemsidan är snabbt. Vad kan det bero på?

Pagespeed nämner olika lösningar som kan förbättra hastigheten av sidladdningen, en gemensam för de valda webbplatserna är laddningstiden på LCP. Alla tre har samma problem att minimisera tiden det tar att
köra JavaScriptet. Det betyder att man kanske ska ta bort onödiga scripter som inte används.

En annan problem är bildupplösningen, en webbutik som har över tusentals produkter har över tusentals bilder. Kvaliteten av bilderna är tyvärr viktiga och därmed inte kan förminskas om kvaliteten påverkas.
Men man kanske kan använda en annan format som ladda snabbare men behåller kvaliteten.

Slutsatsen är att det är viktig hur bra koden måste vara kompilerat för att kunna ladda snabbt, iallafall i en webbutik med mångatals bilder. Utseendet är nog inte det viktigaste, men hur användarvänlig det borde vara!

Misc
-----------------------

<ol>
<li><a href="https://www.amazon.se">Amazon</a></li>
<li><a href="https://www.ikea.com/se/sv/">Ikea</a></li>
<li><a href="https://store.sabrinacarpenter.com">Sabrina Carpenter Merch</a></li>
</ol>

Vinnaren är såklart Amazon och jag tycker väl att det stämmer. Amazon's framsidan innehåller mindre saker jämfört med IKEAs, som inte har någon tom utrymme, hela skärmen är täckt med innehåll.

För mig personligen tyckte jag att Sabrina Carpenters hemsida som fick lägsta Pagespeed poäng utav alla, var ganska snabbt ändå när man går in i den. Det beror nog på att hon inte har lika många produkter
att sälja jämfört med IKEA och Amazon. Min gräns är nog fem sekunder innan jag reloada sidan igen ihopp om att det ska ladda snabbare. Jag tycker att alla mina valda hemsidor agerat fint, de laddar perfekt fram bilderna och videos de har på sidan.

Referenser
-----------------------

<a href="https://pagespeed.web.dev/?utm_source=psi&utm_medium=redirect"> PageSped Insights</a>


Författare
-----------------------

Skriven av: Sumaiyyah Sumaiyyah
