---
Title: Kmom10
Description: Report for Kmom10
Template: kmom
---

Kmom10 redovisning
==========================

Länk till projekt-hemsidan:
http://www.student.bth.se/~emeu17/dbwebb-kurser/design/me/kmom10/projekt/

<h2>1.1 För varje krav du implementerat, dvs 1-6, skriver du ett textstycke</h2>
Jag har valt att implementera krav 1-5.

<h3>Krav 1: Webbplats</h3>
Jag valde att skapa upp en ny installation från example/portfolio som jag la under me/kmom10/projekt/ i kursrepot. Jag installerade npm, sass, laddade in Fontawesome och gjorde alla inställningar på nytt som vi har gått igenom under kursmomenten i kursen. Jag valde det sättet dels för att få göra sidan ”från grunden”, för att få repetera alla steg vi har gjort och för att skapa upp mina sass-filer från scratch.
Jag valde att göra en webbplats åt kund 1: Styrelseordförande Ludviga Af Solstråle med kompanjoner som jag har tolkat jobbar med en konsultfirma med lite exklusiva företag.
Alla bilder som jag använt mig av kommer från Pexels, Unsplash eller Pixabay (tre av de sidor som rekommenderades i kursen, dvs där man kan fritt använda bilder från). Cimage har använts på alla bilder (förutom loggan som redan har en väldigt liten storlek) för att minska mängden data som behöver laddas in. Sedan har jag såklart implementerat de krav som fanns under denna rubrik; tre sidor dvs en första-sida, en about-sida och en customer-sida (motsvarar det som kallas highlight-sida), en flash-bild, en logga, en favicon samt navigering som fungerar både på desktop och mobil. Både about-sidan och första-sidan innehåller information om den potentiella kunden och hur jag har tolkat deras verksamhet. Hur kunden vill att webbplatsen ska se ut och användas går såklart igen på alla tre sidor (se även tema och alternativt tema, krav 2 samt krav 4 nedan).

<h3>Krav 2: Tema</h3>
Jag har skapat upp ett tema för bolaget Ex Consulting. Dom säljer dyra konsult-tjänster åt högklassiga företag och jag har beskrivit tanken bakom tema, sass-filer och typografi, designprinciper m.m under dokumentationen som går att komma åt längst ner på about-sidan eller via länken;
http://www.student.bth.se/~emeu17/dbwebb-kurser/design/me/kmom10/projekt/documentation

<h3>Krav 3: Responsivitet och tillgänglighet</h3>
Tillgänglighet har jag kollat av med hjälp av Google Lighthouse och alla sidor har 100% (på både ljust och mörkt tema). Jag har även kollat av att kontrasten är okej på alla sidor med hjälp av https://color.a11y.com/Contrast/, som var med i kursmoment 4. Dessutom har jag haft färgblindhet i åtanke och testat mina teman mot Toptal color blind filter och även där såg kontrasten/läsbarheten bra ut.
Designen i main-delen av webbplatsen är uppbyggd i en 12-kolumnig grid (för att kunna visa upp innehållet i 1, 2 och 3-block/kolumner per rad. Var även inne på att göra 4-kolumner per rad vilket också skulle fungerat med ett 12-grid system). Jag valde att lägga in flexbox där jag presenterar ”what we do” på första sidan för att även få med flexbox och inte bara grid. All grid-design och även flexbox-designen är responsiv. När sidan minskar i storlek minskas antalet ”block” i griden per rad. Vid mobilskärm visas bara ett ”block” i taget. Även navbaren minskar från att skriva ut alla länkar till en ikon som man kan klicka på för att fälla ut länkarna. Alla images är max 100% av sidans bredd för att undvika horisontella scrollbars.
Vid en storlek på 1200px eller mindre visas 3-block/kolumnerna som två, med den tredje i mitten nedanför, och övriga kolumner har inte längre så stor marginal på åt höger och vänster utan tar upp större delen av sidan (1200 px utgick jag ifrån då det utseendemässigt passade bäst med designen).
Cimage har använts på bilderna som presenteras på webbplatsen. Det i kombination med srcset har använts för att anpassa bilder efter enhet.

<h3>Krav 4: Alternativt tema</h3>
Jag har implementerat ett andra, mörkt, tema. Jag har beskrivit tanken bakom det och dess uppbyggnad tillsammans med det ”vanliga” temat i dokumentationen som man hittar via länk längst ner på About-sidan, eller via länken nedan;
http://www.student.bth.se/~emeu17/dbwebb-kurser/design/me/kmom10/projekt/documentation

<h3>Krav 5: Analys aktuell webbplatsdesign</h3>
Jag valde att göra en analys av fyra advokatbyråer som fanns representerade i min hemstad Sundsvall. . I projektet i kmom10 valde jag att göra en hemsida på temat *executive consulting high-end business company*. Då kändes advokatbyråer som en bra inspirationskälla.

Jag valde att fokusera på färgscheman, typsnitt och designprinciper för att få en överblick över skillnader och likheter bland denna nisch av webbplatser. Aktuella trender som jag noterade var att det klassiska och stilrena var populärt; det var inga typsnitt som stack ut utan var alla moderna, enkla och av typsnitt sans-serif. Färgsättning var monokromatisk på alla undersökta webbplatser och designprinciperna var sparsamma och höll sig till grid-baserade designer. Här kan den fullständiga analysen läsas:
http://www.student.bth.se/~emeu17/dbwebb-kurser/design/me/portfolio/analysis/10_webbplatsdesign

<h2>1.2 Skriv ett allmänt stycke om hur projektet gick att genomföra </h2>
Det som tog längst tid för mig med projektet var att komma igång med en design. Jag använde mig av Figma för att rita upp en initial design och jag tror att det besparade mig en del tid då jag lätt kunde testa färgsättningar/logga/flash image/typsnitt och se hur det passade ihop. Jag hade redan bestämt mig för att använda grid-baserad design för main delen och den designade jag inte i förväg utan testade mig fram för att få en bra variation mellan hur många ”block” per rad som skulle visas. Parallellt med att jag skapade upp hemsidan gjorde jag krav 5, analysen av aktuella trender på webbplatser. Det hjälpte mig också att komma vidare med designen på min hemsida. Allt som har med design-delen av göra var svårt; allt från att komma fram till en bra design till att välja bilder och logga. Sedan tar det såklart tid att implementera saker som att sätta upp ett nytt projekt, skapa upp sass/css koden och implementera responsiv design. Men jag tycker att när jag väl hade fått det första temat någorlunda på plats så flöt det på bra. Det var lättare att komma på ett alternativt tema som jag blev nöjd med än jag hade förväntat mig.

Jag tycker att projektet var rimligt för kursen. Jag har lärt mig en hel del om design och tekniker som kan användas, men jag är tacksam över att det här inte är ett design-program utan ser fram emot att dyka ner mer i programmering och scriptning igen framöver 😊

<h2>1.3 Avsluta med ett sista stycke med dina tankar om kursen och vad du anser om materialet och handledningen</h2>
Jag tycker att kursen överlag har varit bra. Det har varit vettigt innehåll och projektet har snyggt summerat ihop vad vi har jobbat med under kursens gång. Niklas genomgångar har varit korta och koncisa med bra innehåll vilket jag har uppskattat. Jag har även tagit mig igenom alla av Emils föreläsningar men jag har inte tyckt att de har gett lika mycket. Det har varit lite för diffust och svävande och tagit längre tid i anspråk än det hade behövt. Hade gärna sett att de också var lite mer ”kort och koncist” då det kändes som mycket tid att lägga ner på något som inte gav (mig i alla fall) så mycket. Kan i och för sig också ha att göra med att jag läste kurslitteraturen och den tyckte jag mer konkret tog upp liknande innehåll som Emils föreläsningar. Kurslitteraturen var för övrigt bra och jag tycker att ni har samlat ihop många bra artiklar som länkades till i kursmomenten!

Som jag skrev längre upp så är design inte riktigt mitt gebit och det har varit lite mer av en utmaning att ta sig igenom den här kursen än andra webbprogrammeringskurser. Men jag har lärt mig en hel del och tycker absolut att det är bra att kursen ligger så pass tidigt i programmet så att vi har med oss tänket genom nästkommande kurser. Något partiskt ger jag kursen 7/10 eftersom jag fortfarande känner mig lite vilsen i designvärlden, hade gärna önskat att mer UX diskuterats under kursens gång (mer användbarhet, även om jag tycker många områden berörts här) och skulle uppskatta om föreläsningarna i den här kursen innehöll mer matnyttigt (eller kortades ner). För att inte avsluta med bara förbättringspotentialer skulle jag vilja tacka för en lärorik kurs som trots allt har gett mig mer förståelse för webbdesign och breddat min förståelse för vilka tekniker som kan användas (mycket uppskattat). Ser nu fram emot kommande kurser!
