---
Title: Kmom03
Description: Report for Kmom03
Template: kmom
---

Kmom03 redovisning
==========================

Jag har inte tidigare jobbat med varken CSS-Grid eller Flexbox. Ända sedan jag läste kapitel 1 i kurslitteraturen *The principles of Beautiful Web Design* i kmom01 har jag sett fram emot att jobba med just grid-layout. Spontant gillar jag CSS-grid bättre än Flexbox även om jag kan se fördelar med båda. Jag gillar tanken på att designa med hjälp av en grid, vilket känns som ett enkelt sätt att få en design att se snygg (eller åtminstone helt okej) ut för någon som inte är så kreativt lagd. Gillar exemplen på design som fanns i både kurslitteraturen och artikeln *History of the design grid II*. Jag använde mig mestadels av CSS-Grid när jag skapade upp Report- och Kmom-layouten. Jag använde lite Flexbox för den övre delen av boxarna i Report-designen men huvud-designen i båda layouterna är CSS-Grid. Kunde lika gärna ha använt Flexbox för Kmom-layouten och till exempel lagt en flex-grow: 1/flex-grow: 2 respektive på länkarna/redovisningstexten.

Jag hade sedan förra kmom:et delat upp min scss-kod i flera delar; base, layout, variables samt style som sätter ihop alla. Nu la jag, precis som Niklas gick igenom den här veckan, även till report.scss som innehåller style specifik för den layouten. La även till kmom.scss som innehåller style specifikt för kmom-layouten. I min Kmom-layout la jag in länkarna  (den vänstra spalten av designen, som döljs i den responsiva layouten mha *display: none;*) i min twig-fil. Satt och klurade lite på hur Pico fungerade så att jag kunde få länkarna till respektive kmom-sida att skrivas ut automatiskt och precis som i navbaren få den ”aktiva” länken att visas i en annan färg. Hittade i dokumentationen över Pico på github att jag kunde göra en liknande for-sats som i navbaren men specificera vilken underkatalogs sidor jag ville skriva ut och sätta en css-klass för den aktiva sidan; *for page in pages("report")* som är på rad 60 i kmom.twig. På så sätt behövde jag inte skriva in alla länkar i alla md-sidor vilket skulle vara jobbigt om jag var tvungen att lägga till/ta bort/ändra sidor.

Jag valde att endast ändra designen på min report- och kmom-sidor. Det som tog mest tid var dels att få till CSS-Grid på ett bra sätt på kmom-sidorna då jag ville att redovisningstexten skulle hamna över två kolumner och länk-delen över en kolumn. Insåg att lite beroende på hur jag la ut dessa div:ar så behövde jag specificera vilken kolumn de skulle hamna i (ex grid-column: 1 / 3;) och hur många kolumner som div:en skulle ta upp (ex grid-column: span 2;). Sedan tog det tid att fundera ut hur länkarna i kmom-layouten skrevs ut ”automatiskt” (i en for-loop i twig-filen) som jag nämnde ovan.

Min TIL för detta kmom är att CSS Grid var smidigt och känns som något jag vill jobba mer med. Känns som att kombinationen av att använda exempelvis Figma (som tipsades om i kmom01) för att skapa upp några grid-wireframes och sedan implementera dessa med hjälp av CSS Grid kan bli aktuellt till projektet om inte dessförinnan.
