---
Title: Analysis kmom05
Description: This is an analysis of page loading times websites.
---

Webbplatsers laddningstid och användbarhet
=======================

I den här rapporten analyseras tre olika webbplatsers laddningstid och användbarhet. Utifrån insamlade mätvärden
rangordnas sedan webbplatserna för att se vilken som presterar bäst.

Urval
-----------------------

I dessa decembermörka tider spenderar jag en del tid på att hålla mig uppdaterad om vädret då det går snabbt i svängarna
både temperatur och vädermässigt. Jag har därför valt att jämföra tre olika webbplatser som levererar väderprognoser;
SMHI.se [1]. YR.no [2] samt Klart.se [3].


Metod
-----------------------

Google Pagespeed användes för att mäta webbplatsernas *page speed*. Mätning gjordes på både Mobile och Desktop versionen
av webbplatserna och på tre olika sidor för respektive webbplats. Jag valde att analysera respektive webbplats förstasida,
sidan med en väderprognos för Sundsvall (där jag bor) samt deras Om/Info-sida. Sidornas laddningstid, antalet resurser (requests)
samt storleken för webbplatsen noterades också med hjälp av *Devtools* och fliken *Networks*. Sidornas laddningstid är för
Desktop(Dator)-versionen av webbplatsen. Allt dokumenterades i ett Google kalkylark.

Resultat
-----------------------

<a href="https://docs.google.com/spreadsheets/d/1HVdU4DKR05DOai8IMxl0Uc1jI7DtujHNf6IxFYPzM-M/edit#gid=0">Här</a> finns en länk till
sammanställningen av alla mätvärden för de tre webbplatserna.

<h2>SMHI</h2>

<img style="max-width: 100%" src="../assets/img/webpages_loading/smhi.JPG" alt="SMHI hemsida">

Förstasidan för SMHI fick i *Pagespeed* betyg 11 för mobilversionen samt 23 för datorversionen. Laddningstiden var
i genomsnitt 4.7 sekunder, antalet resurser (requests) 187 och sidans totala storlek 5,9MB.

Sidan med väderprognos för Sundsvall hade även den endast 11 i betyg i mobilversionen enligt *Pagespeed* men 54 i datorversionen.
Genomsnittlig laddningstid var 2,4 sekunder, storleken på sidan var 3,9MB och antalet resurser 76 stycken.

För SMHI's Om-sida var betygen enligt *Pagespeed* 32 för mobilversionen samt 94 för datorversionen. Sidan laddades i genomsnitt på 1,6
sekunder, hade 35 resurser och storleken var 0,5MB.

<br>
<h2>YR</h2>

<img style="max-width: 100%" src="../assets/img/webpages_loading/yr.JPG" alt="SMHI hemsida">

Förstasidan för YR fick betyg 66 i mobilversionen samt 95 i datorversionen på *Pagespeed*. Den använde 58 resurser, var 2MB i storlek och
sidan laddades i genomsnitt på 3 sekunder.

Sidan med väderprognos för Sundsvall hade betyg 68 samt 96 för mobil- respektive datorversionen enligt *Pagespeed*. Den använde
33 resurser, hade en genomsnittlig laddningstid på 1.6 sekunder och storleken var 0,3MB.

YR hade ingen om-sida men en sida angående info och support. Den fick betyg 49 respektive 90 för mobil-/datorversionen. Sidan
hade en total storlek på 2.1MB, använde 24 resurser och hade en genomsnittlig laddningstid på 1.4 sekunder.

<br>
<h2>Klart</h2>
<img style="max-width: 100%" src="../assets/img/webpages_loading/klart.JPG" alt="SMHI hemsida">

Förstasidan fick betyg 39 för mobilversionen samt 72 för datorversionen enligt *Pagespeed*. Den genomsnittliga laddningstiden var 3.2 sekunder,
sidans storlek var 7MB och antalet resurser fortsatte öka hela tiden. Antalet initiala resurser var cirka 144 stycken, därefter ökade
resurserna långsammare. Detsamma gäller storleken på sidan som fortsatte växa men långsammare efter den initiala laddningen.

Sidan med väderprognos för Sundsvall fick på *Pagespeed* betyget 45 respektive 97 för mobil-/datorversionen. Storleken på sidan
var 2MB, den genomsnittliga laddningstiden var 2.5 sekunder samt antalet resurser 110 stycken. Precis som med förstasidan så
fortsatte antalet resurser och sidans storlek att öka om än i låg takt efter initiala laddningen.

Klart's Om-sida fick betyget 63 respektive 71 för mobil-/datorversionen. Den laddades i genomsnitt på 1.8 sekunder och hade en
storlek på 1MB. Precis som de övriga sidorna på Klart så fortsatte antalet resurser samt storleken på sidan att öka efter den initiala
laddningen men använda resurser var cirka 101 stycken.


Analys
-----------------------

Diskutera och analysera de resultaten du fann.

Genomgående för alla webbplatser var att laddningstiden var längst för förstasidorna. Det var snabbare att ladda väderleksprognosen för
en specifik stad eller läsa deras Om/Info-sida. Webbplatsernas Om/Info sida var alltid den med lägst laddningstid. Gällande laddningstiden så
var den relativt lika för SMHI och Klart's respektive sidor. YR stack ut med betydligt lägre laddningstider samt lägre antal resurser. Sidans
totala storlek var också lägre för YR än de övriga två. Baserat på laddningstider, antal resurser som användes och sidornas totala storlek
så rangordnas sidorna enligt följande:

1. YR
2. SMHI
3. Klart
<br><br>
Klart hade snarlika värden som SMHI (men något högre laddningstid, storlek på sidan och antal resurser) men hade dessutom ett fortsatt användande
av resurser och inladdning av hemsidans storlek. Det kan ses som positivt att den inte laddade in allt på en gång för då skulle laddningstiden
ha blivit längre, men den var fortfarande något längre än SMHI som var klart långsammare än YR. Troligen beror det på att Klart har två
stora videoklipp med reklam som visas på dess sidor.

En till genomgående trend var att mobilversionen fick lägre betyg på *Pagespeed* än datorversionen för alla webbplatser. Även här stack YR ut med
betydligt högre betyg än de övriga webbplatserna. Här var det dock mer spridning där SMHI i princip genomgående fick låga betyg, YR fick höga
betyg och Klart låg mittemellan. Om sidorna rangordnas utifrån *Pagespeed* betyg ser prioriteringen ut enligt nedan:
1. YR
2. Klart
3. SMHI
<br><br>
Det är tydligt att Yr är vinnare av de tre undersökta webbplatserna. Den hade lägre laddningstid, använde färre resurser och fick högre betyg
på *Pagespeed* än övriga webbplatser. Alla tre sidor på YR hade på datorversionen av sidorna betyg över 90. Deras förbättringspotential
verkar finnas på mobilversionen av sidorna där betyget låg mellan 49 och 68. Där verkar det finnas förbättringsåtgärder både inom att
optimera koden (till exempel laddas det in javascriptkod som inte används) och att vänta med att ladda in bilder som inte syns i första
visningsläget på mobilapplikationer.

För både SMHI och Klart's sidor används överlag betydligt fler resurser än YR's sidor. Att dra ner på dessa borde minska laddningstiden på sidorna.
Klart hade relativt bra betyg enligt *Pagespeed* på datorversionen av sina sidor, 71 - 97. Detta jämfört med SMHI som endast hade 23 i betyg
på sin första sida i datorversionen. Väderprognoser kollas säkerligen ofta via mobila enheter och här finns stor förbättringspotential för
både Klart och SMHI. Återigen dyker det upp i *Pagespeed* att det finns javascript kod som laddas in men som inte används. Även css kod dyker
upp i förslag på förbättringsåtgärder. Alltså verkar optimering av kod kunna ha stor påverkan på alla webbplatser i den här analysen.
Gällande förbättring av mobilversionen av webbplatsernas hemsida kan det dock argumenteras för att många kanske använder deras appar och möjligen har det använts mer resurser på att optimera dessa än mobilversionen av webbplatsen.

Jag uppfattade YR's webbplats som helt okej i laddningstid, även deras första sida som hade en laddningstid på nära 3 sekunder. Däremot
upplevdes både Klart och SMHI's förstasidor som "sega" att ladda. Därför skulle jag säga att en laddningstid under 3 sekunder för
en sida känns rimligt.

Referenser
-----------------------
Webbplatser som har undersökts och datum då anlayserna genomfördes ses nedan.

[1] https://www.smhi.se/, besökt 2020-12-04<br>
[2] https://www.yr.no/, besökt 2020-12-04<br>
[3] https://www.klart.se/, besökt 2020-12-04


Övrigt
-----------------------

Som med förra analysen har även denna veckas genomförts kvälls och helgtid och grupparbete
har känts svårt att få till. Den har därmed genomförts och författats av Emma Edlund.

En kort reflektion om denna kmoms analys är att jag hoppas att det här är något vi kommer att arbeta mer med
under kommande kurser! Optimering av kod för att höja prestandan, vilket kändes som något alla tre webbplatser kunde arbeta mer med,
är något jag skulle vilja lära mig mer om. Tycker denna veckas kmom med att optimera bilder och video knyter ihop
bra med analysen även om det i just dessa webbplatsers fall inte var den stora förbättringspotentialen (även om det dök upp
på några *Pagespeed* analyser).
