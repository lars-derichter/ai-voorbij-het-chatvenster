# Werk presentatie uit

[Terug naar het overzicht](README.md)

## Lars

Wat denk je van de [outline.md](sources/outline.md) ? Mis ik nog iets? Past dit bij het onderwerp en het doelpubliek?

## Assistent (voortgang)

Ik lees de outline samen met de workshopbeschrijving en de andere relevante context. Daarna geef ik je gerichte feedback op de inhoud, de haalbaarheid binnen een uur en de aansluiting bij het publiek.

## Assistent

Ja, de [outline](/Users/lars/-work/thomas-more/ai-competence-center/ai-voorbij-het-chatvenster/sources/outline.md) past goed bij het onderwerp en bij de belofte waarmee deelnemers zich hebben ingeschreven. Je vertrekt vanuit een herkenbaar probleem: wie al met chatbots werkt, wil verder dan telkens context en tekst kopiëren. De combinatie van bestanden, projectinstructies, kwaliteitscontrole en herbruikbare workflows geeft daar een overtuigend antwoord op.

Mijn grootste bedenking is de **breedte**. Er zit genoeg in voor meerdere sessies. Voor een uur met vijftig mensen, van wie sommigen onzeker zijn over technische onderwerpen en mogelijk geen laptop bijhebben, zou ik vooral kiezen wat je zichtbaar wilt maken. Een demonstratie kan meerdere principes tegelijk dragen.

Wat ik nog mis, is een **concreet eindbeeld voor de deelnemer**: wat kan ik na afloop als eerste zelf proberen? Bijvoorbeeld: “Ik maak een map voor een terugkerende taak, geef ChatGPT toegang, voeg een paar bronnen en afspraken toe, en laat een eerste resultaat maken dat ik zelf nakijk.” Dat maakt ook de afzonderlijke begrippen betekenisvol.

**Mijn inhoudelijke suggesties:**

- **Maak één herkenbaar voorbeeld de rode draad.** Neem bijvoorbeeld bestaand cursusmateriaal en laat zien hoe je daaruit een oefening of lesvoorbereiding maakt. Toon dezelfde werkwijze daarna kort voor een niet-onderwijstaak, zoals een draaiboek of interne handleiding. Zo zien ook andere medewerkers waar ze ermee aan de slag kunnen.
- **Laat de groei van de werkwijze zien.** Begin met een opdracht en enkele bestanden, voeg daarna een kleine `AGENTS.md` met projectafspraken toe en maak van een terugkerende aanpak eventueel een skill. Zo wordt duidelijk welk probleem elk onderdeel oplost. Een skill is dan een herbruikbare werkwijze, geen extra stap die altijd nodig is.
- **Maak kwaliteitscontrole tastbaar.** “Heb vertrouwen zodra het plan oké is” zou ik nuanceren: een goedgekeurd plan helpt, maar garandeert geen goed resultaat. Laat in de demo zien dat je bronnen, wijzigingen en output nakijkt, en toon liefst ook een fout of een correctieronde.
- **Geef deelnemers een kleine eerste stap mee.** Een kopieerbaar voorbeeldproject en een zelfstandige startgids lijken me belangrijker dan Git leren als eerste opdracht. Git kan een waardevolle vervolgstap zijn voor versiebeheer en samenwerking, maar hoeft geen toegangsdrempel te worden. Ook VS Code en Pandoc zou ik als hulpmiddelen of verdieping voorstellen.
- **Houd agents en subagents klein.** Ze horen bij de inschrijvingsbelofte, dus ik zou ze wel benoemen en eventueel kort tonen. De manager-agent met modellen en *effort* is een interessant gevorderd voorbeeld, maar dreigt de aandacht weg te trekken van wat deelnemers morgen zelf kunnen proberen. Je vertaalworkflow kan hier een inspirerende blik op wat later mogelijk is zijn.
- **Integreer de grenzen in het voorbeeld.** Werk met fictief of publiek materiaal, gebruik geen identificerende studentgegevens, laat AI geen studentenwerk quoteren en blijf zelf verantwoordelijk. Verwijs naar het [AI-beleid van Thomas More](https://thomasmore365.sharepoint.com/sites/ICTS/Gedeelde%20documenten/Forms/AllItems.aspx?id=%2Fsites%2FICTS%2FGedeelde%20documenten%2F260924%2DTM%2DAD%2DFlow%2EAI%2DOD%202%2DAI%20CC%2DAI%20Beleid%2DDefinitief%20%28TM%2Dversie%29%2Epdf&parent=%2Fsites%2FICTS%2FGedeelde%20documenten). Het beleid vraagt onder meer kritische controle, zorgvuldigheid met gegevens en transparantie bij betekenisvol AI-gebruik.

Ik zou enkele formuleringen ook wat voorzichtiger maken. “Zoveel mogelijk in tekst werken” is een sterk persoonlijk uitgangspunt, maar deelnemers hebben vaak goede redenen om met Word, PowerPoint of andere formaten te werken. Laat vooral zien **waarom Markdown hier handig is**, zonder het als voorwaarde voor goed AI-gebruik te presenteren. En de stelling dat een op zichzelf staand essay geen valide evaluatie meer is, kan een interessant gesprek openen, maar is erg absoluut voor een bonuspunt. Een praktische vraag is: “Wat gebeurt er als je je eigen opdracht aan AI geeft, en wat betekent dat voor wat je wilt beoordelen?”

De productuitleg verdient voor de workshop nog een test in de **Thomas More-omgeving**. Volgens OpenAI kan Work in de desktopapp lokale mappen gebruiken, maar de toegang hangt af van abonnement en werkruimte-instellingen; Work en Codex worden apart beheerd. OpenAI vermeldt ook automatische ontdekking van `AGENTS.md` en skills bij lokale projecten. De documentatie over de precieze skilllocaties beschrijft vooral Codex, dus ik zou specifiek in Work demonstreren of een skill in `.agents/skills` wordt gevonden en gebruikt. Ook de uitspraak dat centrale skills en plugins niet beschikbaar zijn, zou ik als een vaststelling over jullie concrete installatie formuleren, zodra die is getest. [ChatGPT Work and Codex](https://help.openai.com/en/articles/20001275-chatgpt-work-and-codex), [lokale projecten](https://learn.chatgpt.com/docs/whats-new), [skills bouwen](https://learn.chatgpt.com/docs/build-skills?kbid=111697).

Een mogelijke verdeling voor het uur:

| Tijd | Onderdeel |
|---|---|
| 5 min | Probleem, belofte en korte grenzen |
| 10 min | Chat, Work en lokale bestanden: wat verandert er? |
| 20 min | Doorlopende demo met bronnen, Markdown en `AGENTS.md`, inclusief controle |
| 10 min | Een terugkerende aanpak als skill; kort agents en subagents |
| 10 min | Toepassingen voor onderwijs en andere taken, plus eerste stappen |
| 5 min | Vragen en verwijzing naar de startgids |

Dat is vooral een voorstel om te zien of de onderdelen passen; de definitieve timing hangt af van het gekozen voorbeeld en hoe uitgebreid je de demonstratie wilt maken. Mijn gevoel is dat de outline inhoudelijk weinig essentiële thema’s mist: **een herkenbare rode draad, een zichtbare controle en een haalbare eerste stap** zouden het verschil maken.

## Lars

- goed idee van het voorbeeld, ik zal een voorbeeldproject (2 cursusmodules ofzo) integreren in de repo, dan kunnen we tonen hoe we daarvan een test maken; als ander voorbeeld zou ik het vertalen van een tekst naar het Engels nemen.
- akkoord met de groei en werkwijze
- goed om nog eens te benoemen dat plannen bijgestuurd kunnen worden en dat kwaliteit nagekeken moet worden
- eerste stap meegeven vind ik heel goed, maak een bestand deliverables.md in sources met een lijst van wat we allemaal meegeven
- die vertaalworkflow was inderdaad bedoeld als blik op hoe ver je daarin kan gaan
- verwijzing naar het kader zit vooraan

Wat "zoveel mogelijk in tekst werken betreft" daar sta ik 100% achter en dat heeft zich ook uitgebreid bewezen. Het is ook gewoon veel efficiënter en laat toe om te exporteren naar verschillende formaten. De stelling rond essays is bewust een beetje provocerend, maar daar sta ik ook helemaal achter.

Wat er nu in staat is getest in de omgeving. Skills binnen een projectmap werken (in .agents/skills) en worden gevonden.

Werk op basis van de outline, jouw en mijn opmerkingen al een eerste versie van de slides uit. Ik kan daar dan op verder bouwen.

## Assistent (voortgang)

Ik werk een eerste presentatie uit met het cursusvoorbeeld als rode draad en de vertaalworkflow als tweede voorbeeld. Ik zet ook de mee te geven materialen in `sources/deliverables.md`, zodat je die lijst verder kunt aanvullen.

## Assistent (voortgang)

De eerste versie volgt nu de opbouw van een concrete toetsopdracht naar projectafspraken en een herbruikbare skill. Ik controleer nog of de presentatie correct wordt opgebouwd en of de slides goed binnen het thema passen.

## Assistent

De eerste versie van de [slides](/Users/lars/-work/thomas-more/ai-competence-center/ai-voorbij-het-chatvenster/slides.md) staat klaar. Ze volgen de groei van cursusmateriaal naar toets, projectafspraken en een herbruikbare skill. Het vertaalvoorbeeld en de uitgebreidere vertaalworkflow komen daarna aan bod. Bij de slides staan ook sprekersnotities met suggesties voor de demonstratie.

In [deliverables.md](/Users/lars/-work/thomas-more/ai-competence-center/ai-voorbij-het-chatvenster/sources/deliverables.md) staat een werklijst van het materiaal voor deelnemers. Het voorbeeldproject zelf is nog niet opgenomen; de demo en voorbeeldopdracht kunnen we daarop afstemmen zodra je de cursusmodules toevoegt.

De presentatie is met succes opgebouwd met `npm run build`.

## Lars

In het algemeen vind ik dat je wel wat uitgebreider mag zijn. Ik verwacht iets meer detail in de presentatie. Kijk nog eens goed naar de outline die ik opstelde. Ik mis volgens mij nog een aantal elementen daaruit.

Ik zou bijv. zeker de principes expliciet maken en laten terugkeren op het einde.

## Assistent (voortgang)

Ik leg de presentatie opnieuw naast je outline en kijk welke principes en voorbeelden onderbelicht zijn. Daarna stel ik een concreet plan voor de uitbreiding voor, met aandacht voor de beschikbare tijd.

## Assistent

Je hebt gelijk: ik heb de outline te sterk teruggebracht tot een demonstratieverhaal. Daardoor staan verschillende ideeën alleen in de sprekersnotities, terwijl ze belangrijk genoeg zijn om expliciet op de slides te komen. Ook jouw stelling over essays heb ik afgezwakt tot een vraag.

Ik stel deze herwerking voor:

1. **De principes vooraan zichtbaar maken en achteraan herhalen.** Ik zou zes principes uit je outline gebruiken: werk zo veel mogelijk in tekst; geef context; weet wat kwaliteit is; geef heldere instructies en stuur bij; denk in workflows; blijf experimenteren. Elk principe krijgt onderweg een herkenbare plaats in het verhaal en komt op het einde terug als overzicht.

2. **Meer ruimte voor tekst en context.** Naast het Markdown-voorbeeld toon ik duidelijker hoe je met een teksteditor werkt, hoe je vanuit een tekstbron naar andere formaten exporteert en hoe AI daarbij kan helpen. Bij context maak ik het onderscheid zichtbaar tussen persoonlijke instructies, bronnen in een project en projectafspraken in `AGENTS.md`. Ook het interview als manier om verwachtingen boven tafel te krijgen, krijgt een eigen voorbeeld.

3. **Kwaliteit en instructies afzonderlijk uitwerken.** Niet alleen de toets controleren, maar ook uitleggen waarom je eerst moet weten wat een goed resultaat voor jou betekent. Bij instructies neem ik mee dat ze helder moeten zijn zonder dat een prompt perfect hoeft te zijn: laat een plan maken, stuur het bij en werk iteratief.

4. **Workflows en skills concreter maken.** Ik laat zien hoe een herhaalde taak uitgroeit tot een skill en hoe die in de geteste omgeving via `.agents/skills` wordt gevonden. Ik benoem ook de beperking die je in de outline vermeldt over centrale skills en plugins in jullie installatie.

5. **Agents en de vertaalworkflow meer inhoud geven.** Ik leg eerst uit wat een agent en een subagent doen. Daarna toon ik jouw werkwijze met een manager die overzicht en eindkwaliteit bewaakt en aparte agents voor deeltaken en controles. De boekvertaling blijft een blik op wat mogelijk is, met de kanttekening dat de auteurs de vertaling nog nalezen.

6. **Experiment en vervolgstappen uitbreiden.** De grillige grens tussen wat AI wel en niet kan, de vraag wat je zelf wilt uitbesteden, en de mogelijkheid om AI om hulp te vragen bij het ontdekken van toepassingen komen expliciet terug. Je stelling over het essay zet ik zichtbaar op een slide als jouw bewust provocerende stelling. Markdown, de repository en Git krijgen elk een duidelijke plaats bij de vervolgstappen.

Ik behoud de toetsdemo als rode draad en het vertalen als tweede voorbeeld. De slides blijven afzonderlijk leesbaar en sober, maar de presentatie krijgt meer inhoud en waar nodig extra slides; de sprekersnotities dragen de verdere toelichting.

Mag ik de presentatie volgens dit plan herwerken? Ik wacht op je akkoord omdat je projectafspraken vragen om inhoudelijke keuzes eerst voor te leggen.

## Lars

go

## Assistent (voortgang)

Ik werk de slides nu uit volgens die opbouw: de principes worden de rode draad, met meer zichtbare uitleg en een herhaling op het einde. Ik behoud ruimte voor de demonstratie en de voorbeelden die je nog aan de repository toevoegt.

## Assistent

De [presentatie](/Users/lars/-work/thomas-more/ai-competence-center/ai-voorbij-het-chatvenster/slides.md) is uitgebreid. De zes principes staan nu vooraan, krijgen elk een plaats in het verhaal en keren aan het einde terug.

Ik heb onder meer context en projectinstructies, kwaliteitsbesef, workflows en skills, agents en subagents, en experimenteren verder uitgewerkt. Ook je stelling over essays staat nu zichtbaar op een slide. De toetsdemo blijft de rode draad; het voorbeeldproject moet nog worden toegevoegd.

De presentatie bouwt zonder fouten met `npm run build`. De uitgebreidere versie zal nog wel op timing moeten worden bekeken zodra de demo met de echte cursusmodules klaarstaat.

## Lars

Ik bedenk net: als rode draad zouden we het maken van deze presentatie kunnen gebruiken. Als extra project kunnen we dan het ontwikkelen van een startgids markdown-gebruik doen. Die wordt dan live tijdens de workshop gemaakt en op het einde gedeeld.

## Assistent

Dat vind ik een sterke rode draad. De presentatie is een herkenbaar voorbeeld van iets wat met AI en lokale bestanden tot stand komt. Bovendien kunnen we de deelnemers het project laten zien terwijl we erover vertellen.

Ik zou de workshop zo herwerken:

1. **Start met het resultaat:** toon de presentatie en vertel dat ze samen met AI is gemaakt. Open daarna de projectmap: de slides staan in `slides.md`, de achtergrondinformatie in `sources/` en de projectafspraken in `AGENTS.md`.

2. **Gebruik de presentatie om de principes zichtbaar te maken:** toon hoe Markdown de inhoud bewaart, hoe de bronnen context geven, hoe de projectinstructies de samenwerking sturen en hoe jij voorstellen en wijzigingen beoordeelt. Je kunt ook een bestaande slide aanpassen om de feedbacklus te laten zien.

3. **Maak live een Markdown-startgids:** vraag AI om op basis van een duidelijke opdracht en eventuele projectafspraken eerst een plan voor te stellen. Stuur dat bij, laat de gids maken en kijk samen een stuk na. De gids kan uitleggen hoe deelnemers Markdown lezen, schrijven en met AI gebruiken.

4. **Deel de gids op het einde:** voeg hem toe aan de repository, zodat deelnemers hem na de workshop kunnen terugvinden. Daarvoor moeten we vooraf bepalen hoe je de wijzigingen tijdens de sessie publiceert en controleren of dat lukt.

5. **Gebruik vertalen als tweede voorbeeld:** toon hoe dezelfde principes op een andere taak toepasbaar zijn. De boekvertaling blijft een korte blik op uitgebreidere workflows met agents en kwaliteitscontroles.

De cursusmodules en toets hoeven dan niet langer de rode draad te zijn. Ze kunnen later nog als aanvullend voorbeeld dienen. Ik zou voor de live demo wel een voorbereide beginstaat én een reserveversie van de gids klaarzetten, zodat je het resultaat ook kunt tonen en delen als een stap langer duurt of mislukt.

Mag ik de slides en de lijst met mee te geven materiaal volgens deze nieuwe opbouw aanpassen? Ik leg deze inhoudelijke koerswijziging eerst voor, zoals afgesproken in de projectinstructies.

## Lars

Go

## Assistent (voortgang)

Ik pas de presentatie aan zodat dit project zelf de principes laat zien en de live gemaakte Markdown-startgids het centrale demonstratiemoment wordt. Ik werk ook de lijst met mee te geven materiaal bij en houd rekening met een reserveversie voor de demo.

## Assistent

De [slides](/Users/lars/-work/thomas-more/ai-competence-center/ai-voorbij-het-chatvenster/slides.md) gebruiken nu dit presentatieproject als rode draad. De live demo laat zien hoe je samen met AI een Markdown-startgids plant, maakt en nakijkt. De zes principes blijven vooraan en achteraan zichtbaar; het vertaalvoorbeeld blijft behouden.

Ook [deliverables.md](/Users/lars/-work/thomas-more/ai-competence-center/ai-voorbij-het-chatvenster/sources/deliverables.md) is aangepast. Daarin staan de reserveversie van de gids en het vooraf testen van de publicatie als voorbereidingspunten. Die zijn nog niet uitgevoerd; de gids zelf is bedoeld om live te maken.

De presentatie bouwt met succes met `npm run build`.

## Lars

Ik zou willen aanpassen dat we eerste de toepassing van de principes tonen in het project van deze presentatie en dat we daarna de live demo doen met de markdown guide.

## Assistent (voortgang)

Ik herschik de presentatie zodat we eerst de zes principes herkennen in het bestaande presentatieproject. Daarna passen we ze opnieuw toe tijdens de live demo van de Markdown-gids.

## Assistent

De [presentatie](/Users/lars/-work/thomas-more/ai-competence-center/ai-voorbij-het-chatvenster/slides.md) volgt nu de gewenste volgorde: eerst de principes aan de hand van het presentatieproject, daarna de live demo waarin we ze toepassen om de Markdown-startgids te maken.

Ik heb de voorbeelden en sprekersnotities daarop afgestemd. De presentatie bouwt zonder fouten.

## Lars

Ik heb intussen nog wat aanpassingen gedaan en ook een voorbeeldskill: presentatie-ontwerpen gemaakt.

Pas deze zin: Bijvoorbeeld: eerst een plan, dan feedback, daarna schrijven en controleren. aan de bestaande skill aan.

## Assistent (voortgang)

Ik kijk even naar de voorbeeldskill en pas de zin op de slide aan zodat ze de echte werkwijze beschrijft.

## Assistent

De zin in [slides.md](/Users/lars/-work/thomas-more/ai-competence-center/ai-voorbij-het-chatvenster/slides.md) beschrijft nu de werkwijze van `presentatie-ontwerpen`: context verzamelen, interviewen, een outline afspreken en daarna de presentatie schrijven en controleren.

Ik heb ook de sprekersnotities bijgewerkt: daarin stond nog dat er geen voorbeeldskill in het project was.

## Lars

agents komt nu heel abrupt. Maak hier een aparte sectie van. Voeg een diagram in om de workflow met een manager en multipele workers visueel te maken. Voeg een diagram toe van de boekvertaal workflow (manager - editors - elke editor een vertaler en een typesetter + SOP's die procedures vastleggen met stappenplannen en checklists.)

## Assistent (voortgang)

Ik maak van agents een duidelijk afgebakend onderdeel en werk twee schema’s uit: eerst het algemene patroon met een manager en workers, daarna de boekvertaalworkflow met editors, vertalers, typesetters en SOP’s.

## Assistent

Ik heb in [slides.md](/Users/lars/-work/thomas-more/ai-competence-center/ai-voorbij-het-chatvenster/slides.md) een aparte sectie over agents toegevoegd, met twee diagrammen:

- een manager die werk verdeelt over meerdere workers;
- de boekvertaalworkflow met per hoofdstuk een editor, een vertaler en een typesetter, ondersteund door SOP’s.

Bij het tweede diagram staat dat de hoofdstukken één voor één worden verwerkt. De sprekersnotities geven extra uitleg over de controles en de review. De presentatie bouwt zonder fouten.

## Lars

vertaler en typesetter verdienen hun eigen vakjes. SOP's kan je er laten uitzien als een stapeltje documenten langs de zijkant.

## Assistent (voortgang)

Ik pas het schema aan: vertaler en typesetter krijgen elk een eigen vak, en de SOP’s komen als een stapeltje documenten naast de workflow.

## Assistent

Het diagram in [slides.md](/Users/lars/-work/thomas-more/ai-competence-center/ai-voorbij-het-chatvenster/slides.md) toont nu voor elke editor aparte vakjes voor de vertaler en de typesetter. De SOP’s staan als een stapeltje documenten naast de workflow.

De presentatie bouwt zonder fouten.

## Lars

voorzie iets meer marge onder de diagrammen

## Assistent (voortgang)

Ik voeg wat ruimte toe onder beide diagrammen, zodat de tekst eronder beter loskomt.

## Assistent

Er staat nu meer ruimte onder beide diagrammen in [slides.md](/Users/lars/-work/thomas-more/ai-competence-center/ai-voorbij-het-chatvenster/slides.md).

## Lars

Tekst vertalen ga ik niet meer doen. Dan wordt het te lang, verwijder dat onderdeel uit de presentatie.

## Assistent (voortgang)

Ik verwijder het afzonderlijke voorbeeld over een tekst vertalen. De boekvertaling blijft staan als illustratie van de workflow met agents.

## Assistent

Het afzonderlijke voorbeeld over een tekst vertalen is uit de [presentatie](/Users/lars/-work/thomas-more/ai-competence-center/ai-voorbij-het-chatvenster/slides.md) verwijderd. De boekvertaling blijft staan als voorbeeld van een workflow met agents.
