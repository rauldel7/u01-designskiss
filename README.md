1. Från skiss till kod. Hur gick du tillväga? Var det något i skissen som var svårt att översätta till HTML och CSS, och hur löste du det?

svar: När jag sog skissen i mobil-layout såg jag direkt att det fanns en typ av meny knapp som jag visste skulle bli svår att implementera i HTML och CSS med tanke på att JavaScript borde användas med button. Jag gjorde min research och hittade input type = "checkbox" funkade som en typ av knapp med en inbyggd regel som lät mig ta fram en meny när checkboxen va checkad och ta bort den när jag uncheckade den. I min base.css kunde jag göra så att själva checkbox markeringen försvann med display:none i #menu-togglen och nu hade jag en checkbox som funkade och såg ut som en knapp. Genom #menu-toggle:checked ~ .nav kunde jag använda en o checkad box att .nav skulle ha display:none och sedan en checkad box gav min .nav display:block. Det funkade perfekt tills att jag prövade tangentbords navigeringen. Den ville inte fokusera på min knapp pågrund av att jag lagt display:none på den. Jag testade att lägga till tabindex = "0" i html koden. Nu funkade fokuset på den, fast nu gick det inte att checka boxen längre och min .nav ändras inte från display:none till display:block. Till slut bytte jag display:none på #menu-toggle till opacity:0 så att den helt enkelt var osynlig och då kunde jag fixa mitt problem genom :focus-visible och lite dekoration för outlinen.

2. Semantik. Vilka HTML-element valde du för sidans olika delar, och varför just de? Var landade du i ett div för att inget bättre fanns?

svar: Mina HTML-element var väldigt vanliga. 'header i varje HTML fil med logo typen och input type = "checkbox" med label för att namnge min knapp. nav i alla fler valiga tillfällen som fanns i koden som den horisontella och vertikala navigeringen i menyn eller länkarna i de oliksá projekten. Jag hade section i mina main och article för att dela upp allt i ännu mindre delar. Jag använde figure för profilbilden och img för alla ikoner. i about.HTML hade jag h1, h2, och p i varje article och de log i varsin section.
Använde hr för de grå linjer som separerade de olika article. Jag hade footer i slutet av alla HTML filerna och där jag behöde använda div var där saker behövde läggas i kolumner. Jag hade de i section först men div avr det som funkade för  validator.w3.org.

3. Layout. Var använde du Flexbox, var använde du Grid, och vad avgjorde valet? Hur gjorde du sidan responsiv, och varför lade du brytpunkterna där du gjorde?

svar: Min layout var väldigt mixad. Flexbox användes när det kom till att centrera det mesta och flex-wrap för headern så att den satt rätt på toppen av sidan. 
för project och tech sidan använde jag grid för kolumnerna så att de satt under varandra på samma sätt som skissen.

4. Tillgänglighet. Vad har du gjort för att sidan ska gå att använda för fler? Hur testade du det, och vad visade testet? Vad återstår?

Jag har lagt till det all semantik som låter hemsidan navigeras med bara tangentbordet, alla img har sin alt-text och så har jag media querys så att hemsidan kan gå från mobile till desktop layout och med prefers-color-scheme: dark för att den ska matcha enheter med både ljust eller mörkt-läge.

5. Användbarhet. Vilka UX- eller UI-principer känner du igen i Pawans design? Är det något du hade gjort annorlunda, och varför?


Jag känner igen den vanliga uppbyggnaden av varje sida. Titel i som förklarar det som ligger i sidan, en navigering i toppen som ger någon möjligheten att röra sig mellan sidor. Alla sidorna har samma margins och padding som leder till en finare design. responsiv design som kan röra sig från mobil till desktop layout.

Om jag kunde ändra något hade för det mesta varit färgerna, jag tycker vitt till svart är lite aggresivt när det kommer till kontrast och färgval.

6. Styrkor och brister. Vad blev bra, och vad skulle du bygga om med mer tid?

Jag tycker att min lösning för knappen var bra och en riktig utmaning. ifall jag hade mer tid hade jag försökt att använda en ända typ av layout, till exempel använt flexbox på allt så att det hade hängt ihop och sett bättre ut. Under hela projektet lärde jag mig mer och mer saker som jag ändrade på och till slut blev projektet en blanding av många tekniker. Under hela projektet så städade jag upp min kod och tog bort saker jag sedan märkte var där i onödan. Jag önskar jag hade haft tid att bygga projektet från noll med en bättre struktur.

7. AI-verktyg. Om du använt dem: till vad, och vad ändrade du i det som genererades?

Jag hade svårt med alla ikonerna i tech sidan när det kom till css. Jag använde flexbox i början men tyckte inte om hur det blev för att det inte blev som skissen. Den lärde mig hur grid-columns fungerade som jag sedan använde i projekt sidan också utan hjälp av AI. 

Jag visste heller inte hur jag skulle färga texten med en gradient. AI hjälpte mig få fram css som jag sedan kunde använda igen i alla andra platser som behövde det.