# Att beställa och förbereda ett penetrationstest
Ett penetrationstest kräver förberedelser hos både beställaren och leverantören. Tydliga mål, fungerande åtkomst och tillgängliga kontaktpersoner ger testarna bättre förutsättningar att undersöka de delar som är viktigast för verksamheten.

Detta dokument beskriver vad beställaren bör förbereda och vad organisationen kan förvänta sig före, under och efter ett penetrationstest. Förberedelserna behöver anpassas till testets mål, omfattning och arbetssätt i dialog med leverantören.

## Mål och omfattning
Beställaren bör ha en grundläggande förståelse för systemet, dess användning och beroenden. Börja med att besvara följande frågor:
- Vad vill vi testa?
- Vad vill vi få ut av testet?
- Varför vill vi testa detta?

Anledningen kan exempelvis vara krav från kunder, lagar och regelverk eller organisationens eget säkerhetsarbete. Syftet hjälper leverantören att föreslå en lämplig omfattning och prioritera inom den tid och budget som finns.

Dokumentera vilka system, funktioner och miljöer som ingår och vilka som undantas. En tydlig avgränsning minskar risken för att viktiga komponenter missas och behöver testas vid ett senare tillfälle. Ändringar under pågående uppdrag kan påverka både kostnad och tidsplan och behöver därför godkännas av båda parter.

Ett penetrationstest ger en bedömning av de undersökta delarna vid testtillfället. Det kan inte garantera att samtliga sårbarheter identifieras.

## Krav och tillstånd
Beställaren behöver klargöra vilka lagar, regelverk, standarder och avtalskrav som är relevanta för uppdraget. Det kan exempelvis vara [DORA](https://eur-lex.europa.eu/eli/reg/2022/2554/oj/swe), [cybersäkerhetslagen](https://www.riksdagen.se/sv/dokument-och-lagar/dokument/svensk-forfattningssamling/cybersakerhetslag-20251506_sfs-2025-1506/) eller branchstandarder som [PCI DSS](https://www.pcisecuritystandards.org/standards/pci-dss/). Tillämpliga krav bör kommuniceras tidigt eftersom de kan påverka omfattning, genomförande och dokumentation.

Leverantören bör kunna beskriva sin erfarenhet av relevanta krav och hur testet kan bidra till att uppfylla dem. Ett penetrationstest innebär dock inte i sig att organisationen uppfyller samtliga krav.

Innan testet börjar ska det finnas ett dokumenterat tillstånd från den som har rätt att godkänna testningen. Beställaren behöver även kontrollera villkor och eventuella tillstånd för berörda driftleverantörer, molntjänster och andra tredjeparter.

## Tidsplan
Planera uppdraget i god tid, särskilt om resultatet behövs före en lansering, revision eller ett årsskifte. Leverantören kan ha andra uppdrag inbokade och begränsad möjlighet att flytta eller förlänga testperioden. Bokning och betalning styrs av avtalet, men förberedelserna behöver vara klara före teststart.

Kom överens om datum för förberedelser, testning, rapportleverans och avrapportering. Rapportskrivningen behöver egen tid, och arbetsinsatsen påverkas bland annat av testets omfattning och antalet fynd. Leveransdatum och hantering av eventuella förseningar bör ändå vara tydliga.

Om åtkomst eller andra förutsättningar saknas kan testtiden behöva omfördelas eller omfattningen begränsas. Parterna bör då komma överens om hur uppdraget ska anpassas. Begränsningar som påverkar resultatet ska framgå av rapporten.

## Ansvar och kontaktpersoner
Vid uppstart och avrapportering bör personer med kunskap om både systemet och verksamhetens behov delta. Det kan exempelvis vara systemägare, utvecklare, driftpersonal och säkerhetsansvariga. Personer som känner till eventuella externa krav kan också behöva medverka.

Under testet ska det finnas kontaktpersoner som kan besvara frågor, ordna åtkomst och hantera driftproblem eller kritiska fynd. Det behöver vara tydligt vem som får godkänna förändringar eller besluta att testet ska pausas.

Dokumentera ordinarie och alternativa kontaktvägar hos båda parter. Säkerställ att kontaktpersonerna har avsatt tid och att det finns ersättare vid ledighet eller annan frånvaro.

## Dokumentation
Relevant och aktuell dokumentation hjälper testarna att förstå systemet och använda testtiden effektivt. Beroende på uppdraget kan följande underlag vara användbara:
- API-specifikationer och beskrivningar av viktiga funktioner
- Arkitekturdiagram och beskrivningar av infrastrukturen
- Nätverksskisser och systemens beroenden
- Inventering av system, komponenter och använda tekniker
- Beskrivningar av verksamhetsprocesser, användarflöden och behörighetsroller
- Källkod och relevanta konfigurationer, när det ingår i testupplägget

Stäm av med leverantören vilket underlag som behövs och ange om dokumentationen är ofullständig eller inaktuell. En genomgång av systemets viktigaste funktioner kan komplettera den skriftliga dokumentationen.

## Åtkomst och introduktion
Vilken åtkomst testarna behöver beror på testets mål och arbetssätt. Beställaren bör i förväg ordna överenskomna testkonton, behörigheter, VPN-anslutningar och eventuell flerfaktorsautentisering. Vid tester av olika användarroller behövs konton som motsvarar dessa roller.

Om beställaren kräver en särskild testdator eller arbete på plats behöver även utrustning, tillträde och en lämplig arbetsplats vara förberedda. Låt testarna kontrollera åtkomsten före teststart så att tekniska problem kan lösas i tid.

Obligatorisk introduktion till exempelvis etiska riktlinjer, säkerhetspolicyer och interna rutiner bör genomföras i förväg. Beställaren behöver informera om sådana krav tidigt så att de kan planeras utan att ta tid från själva testningen.

## Val av testmiljö
Välj testmiljö tillsammans med leverantören utifrån testets syfte och riskerna för verksamheten. En separat miljö, exempelvis för test, kvalitetssäkring eller acceptanstest, kan minska risken för påverkan på kunder, utvecklare och andra anställda. Miljön behöver samtidigt motsvara produktion i de delar som ska undersökas.

Beskriv skillnader i konfiguration, behörigheter, data och integrationer. Om externa tjänster är simulerade eller frånkopplade behöver testarna känna till det och förklara hur det begränsar slutsatserna. I vissa uppdrag kan testning i produktion vara motiverad, exempelvis för att undersöka den faktiska konfigurationen i en Active Directory-miljö.

Undvik oplanerade förändringar under testperioden. Uppdateringar kan göra tidigare resultat inaktuella och kräva ytterligare verifiering. Nödvändiga ändringar ska samordnas med testarna. Om ny funktionalitet tillkommer kan testet behöva flyttas eller kompletteras med ett separat test.

## Risker och återställning
Ett penetrationstest kan belasta system, påverka data eller orsaka driftstörningar. Beställaren och leverantören behöver därför komma överens om tillåtna testmetoder, testtider och vilken påverkan som kan accepteras.

Beställaren bör säkerställa att relevanta säkerhetskopior finns och att rutinerna för återställning fungerar innan testet påbörjas. Berörd driftpersonal behöver känna till hur eventuella problem ska hanteras. Bestäm också när testet ska avbrytas, vem som ska kontaktas och vem som får godkänna att arbetet återupptas.

## Skyddsfunktioner och konfiguration
Brandväggar, intrångsskydd och antivirus kan påverka vilka tester som går att genomföra. Om syftet är att undersöka en applikations eller ett systems underliggande säkerhet kan begränsade undantag behövas för att testtiden ska användas effektivt. Om skyddens funktion ska utvärderas behöver testupplägget ta hänsyn till det.

Eventuella undantag ska beslutas tillsammans med ansvariga hos beställaren, avgränsas till vad som behövs och dokumenteras. Det ska framgå vilka skydd som har ändrats, hur det påverkar resultatet och vem hos beställaren som ansvarar för att återställa konfigurationen efter testet.

## Datahantering och säker överföring
Beställaren behöver tidigt beskriva vilken information som är känslig och vilka regler som gäller för hanteringen. Det omfattar både information som lämnas till leverantören och material som skapas under testet, exempelvis anteckningar, loggar, skärmbilder och rapporter.

Kom överens om var information får lagras, även på testarnas datorer, vilka som får ta del av den och när den ska raderas. Klargör också om externa tjänster eller AI-verktyg får användas för att bearbeta materialet och på vilka villkor. Använd representativ testdata där det är möjligt och undvik onödig exponering av känsliga uppgifter.

Bestäm godkända kommunikationsvägar för rapporter, inloggningsuppgifter och annan känslig information. Om krypterade filer används bör lösenord eller nycklar överföras genom en separat kanal. Metoden behöver följa beställarorganisationens krav på informationshantering.

## Insyn under testet
Beställaren bör kunna förvänta sig tydlig och regelbunden information om hur arbetet fortskrider, vilka hinder som uppstår och om tidsplanen påverkas. Kom överens om hur ofta uppdateringar ska lämnas och vilka som ska få dem. Kritiska fynd och akuta problem ska kommuniceras skyndsamt enligt överenskomna rutiner.

Uppföljningen behöver rymmas inom uppdragets planering. Om beställaren vill följa testarnas arbete i detalj eller använda testet för utbildning bör detta avtalas särskilt, eftersom det kräver tid och kan påverka upplägget.

## Rapportering och sakgranskning
Beställaren bör förvänta sig en rapport som beskriver vad som har testats, vilka begränsningar som funnits, vilka sårbarheter som identifierats och vilka åtgärder som rekommenderas. Resultatet bör gås igenom vid ett avrapporteringsmöte med de personer som ska förstå, prioritera och hantera fynden.

Beställaren ska kunna påpeka sakfel, begära förtydliganden och lämna kompletterande information som kan påverka bedömningen av ett säkerhetsfynd. Sådana ändringar behöver bygga på verifierbara omständigheter. Fynd ska inte döljas eller allvarlighetsgraden sänkas för att tillfredsställa kunder, ägare eller andra intressenter.

Behov av olika rapportversioner bör avtalas i förväg. En intern teknisk rapport kan innehålla detaljer för att återskapa och åtgärda sårbarheter, medan en rapport avsedd för ägare, kunder eller offentligheten kan behöva begränsa dessa uppgifter. Versionerna ska ge en rättvisande bild av resultatet inom den omfattning de beskriver.

## Efter avslutat test
Beställaren behöver avsätta tid och ansvariga personer för att prioritera och åtgärda identifierade brister. Klargör om verifiering av åtgärder, ofta kallad omtest, ingår i uppdraget eller behöver beställas separat.

Avsluta även tillfälliga åtkomster, ta bort testkonton och återställ överenskomna konfigurationsändringar när de inte längre behövs. Hantering och radering av testmaterial ska följa det som parterna har avtalat.
