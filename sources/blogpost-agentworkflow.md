# Een handboek vertalen met een team van AI-agents

Een vakboek van een paar honderd pagina's vertalen naar het Engels, met de
opmaak van het origineel: dat heb ik grotendeels laten doen door AI-agents in
Claude Code. Het interessantste deel was de organisatie van het werk. Drie
dingen maakten het verschil: SOP's, quality gates en een duidelijke rolverdeling
tussen agents.

## SOP's: recepten in plaats van prompts

Elke terugkerende taak staat als checklist in een SOP: een hoofdstuk produceren,
feedback van de klant verwerken, een fout op een pagina melden en oplossen, een
nieuw soort element toevoegen. Over elke SOP ligt een skill, zodat één commando
de hele procedure start.

Dat lijkt bureaucratisch, maar een agent die een bewezen recept volgt, levert
voorspelbaarder werk dan een agent die improviseert. De SOP's groeiden mee: elke
keer dat iets misliep, kwam er een stap of een controle bij.

## Quality gates: meten verslaat kijken

Lang vertrouwden we op visuele controle: render naast origineel leggen en
vergelijken. Dat faalde herhaaldelijk. Kleine afwijkingen in regelafstand of
positie glipten telkens door, ook bij een menselijke controle.

Dus werd elke "kijk of het klopt" omgezet in een meetbare regel. Per hoofdstuk
draait nu een reeks automatische gates in één commando: kloppen de getallen,
komen de termen uit de goedgekeurde woordenlijst, staat er nergens nog brontaal,
komt de opmaak geometrisch overeen met het origineel. Toen we die laatste gate
loslieten op een hoofdstuk dat iedereen als afgewerkt beschouwde, faalde bijna
alles. Terecht.

Een rode gate wordt opgelost, nooit omzeild. Daarnaast bevat de SOP twee
menselijke gates: na de figuren en na de opgemaakte PDF.

## Rollen: manager, editor, workers

Het grootste deel van het boek is geproduceerd terwijl ik op vakantie was. De
opzet:

- Een **manager**-agent neemt mijn rol over. Die werkt de hoofdstukken één voor
  één af, neemt de menselijke gates over en beslist. Zelf produceert de manager
  niets.
- Per hoofdstuk start de manager een **verse editor** die de SOP uitvoert, het
  werk verdeelt, de kwaliteit controleert en commit. Een nieuw team per
  hoofdstuk voorkomt dat context van het ene hoofdstuk het volgende vervuilt.
- **Workers** doen het eigenlijke werk binnen een strak afgebakende opdracht. Ze
  committen niet en beslissen niets.
- Een aparte **review-agent** doet de visuele controle en rapporteert. De
  manager beslist welke opmerkingen terecht zijn.

Waar een echte beslissing nodig was, nam de manager een onderbouwde gok en
schreef die op in een lijst met open vragen voor de klant. Inhoudelijke twijfel
was geen reden om te stoppen.

## Crashbestendig werken

Agents vallen weg door sessielimieten of netwerkstoringen, en dat kondigt zich
niet aan. Daarom volgt na elke afgewerkte stap een commit en een push. Wat niet
gepusht is, geldt als verloren. Een herstart vertrouwt niet op een logboek maar
controleert de git-geschiedenis en de gates, en pikt de draad daar op. Tijdens
de run gebeurde dat meerdere keren, zonder noemenswaardig verlies.

## Wat ik ervan meeneem

Mijn rol verschoof van zelf controleren naar controles ontwerpen. Pas toen die
er stonden, kon ik het werk loslaten. En: schrijf alles op. Elke sessie staat in
een procesnotitie, met mijn prompts, de vragen die terugkwamen en de redenering
achter elke beslissing. Daardoor kan een verse agent, of ikzelf na een vakantie,
op elk moment instappen.

De vertaling is nu een eerste versie. De auteurs lezen ze na, en hun antwoorden
gaan via dezelfde SOP's terug in het boek.
