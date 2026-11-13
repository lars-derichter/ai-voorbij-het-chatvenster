# Chronologie: AI in de ontwikkeling van Programming Fundamentals en Coursewright

Ruw materiaal voor de workshop voor collega's. Afgeleid uit de git-geschiedenis
van deze cursus (662 commits, mei–november 2026) en van Coursewright (899
commits, maart–november 2026), aangevuld met wat de documenten in `sources/`
prijsgeven. Commit-hashes en data staan erbij, zodat elk punt terug te vinden is
voor een demo.

Ruwe cijfers: ongeveer 515 van de 662 cursuscommits en 786 van de 899
Coursewright-commits dragen een `Co-Authored-By: Claude`-regel. De drukste dag
van de cursus is 11 juli (64 commits, de autonome werkrun), die van Coursewright
23 augustus (110 commits, de herschrijving van de sync-engine).

| Maand     | Cursus | Coursewright |
| --------- | -----: | -----------: |
| maart     |      – |          134 |
| april     |      – |            9 |
| mei       |     87 |           16 |
| juni      |     58 |           12 |
| juli      |     81 |           44 |
| augustus  |     25 |          609 |
| september |    239 |           47 |
| oktober   |    164 |           25 |
| november  |      8 |            3 |

## Fase 1: het gereedschap eerst (maart–april)

- **Het probleem dat alles in gang zet.** Cursusmateriaal schrijven in de
  Canvas-editor is traag, zonder versiebeheer en onbruikbaar voor een AI-agent.
  Het idee: markdown in een git-repo als bron, Canvas als publicatiekanaal.
- **Canvas Local, gebouwd door Claude Code (11–16 maart).** De eerste commit na
  de lege repo heet letterlijk “First version created by Claude Code per my
  instructions” (`907c530`). Binnen een week staan er een CLI, een VS
  Code-extensie, push en pull naar Canvas, retry-logica en een testsuite. Ik ben
  productowner, de agent bouwt.
- **Een stijlgids als systeem (15 april).** De tooling krijgt een vast bestand
  dat beschrijft hoe teksten moeten klinken, met een eigen register voor
  studenten en een voor collega's. Dat bestand leest de agent bij elke sessie.
  Het wordt later een van de belangrijkste hefbomen.

## Fase 2: de didactische fundering (mei)

- **Bronnen verzamelen vóór er iets gegenereerd wordt (17 mei).** Visie van de
  opleiding, de oude doelen en inhouden, de ECTS-fiche, eigen principes,
  projectideeën, redenen voor een nieuwe cursus: alles komt als markdown in
  `sources/didactisch-kader-bronnen/` (`de3154d`, `5db9b96`).
- **Leerdoelen uit een gesprek.** De negen leerdoelen komen uit een gesprek met
  Claude in de chat-app, als bron bewaard in `leerdoelen-gesprek-claude.md`.
  Goed demomoment: chat om te denken, agent in de repo om te bouwen.
- **Het kader laten schrijven, dan nakijken.** De prompt staat bewaard in
  `prompt-pedagogical-framework.md`: secties opgelegd, “ask clarifying
  questions”. Twee opeenvolgende commits vertellen het verhaal: “Have Claude
  create a pedagogical framework” (`1307865`) en “error check Claudes output”
  (`9ced21e`).
- **Het kader als verplichte lectuur.** Meteen daarna een regel in de
  instructies: lees het kader vóór je aan cursusmateriaal werkt (`5039806`). Dat
  principe evolueert later naar `context/course-context.md`.

## Fase 3: de eerste lessen en het ontstaan van de skills (mei)

- **Les 1 met de hand, samen met de agent (17–18 mei).** Lesplan, dan de
  studentenmodule, dan het lesplan bijgestuurd op de module (`d04bbd1`,
  `752abc9`, `6167ef5`). Timing ingekort tot het in drie uur past.
- **Ruw idee, agent werkt uit, ik scherp aan.** Les 2 in drie commits: “Create
  very rough plan for lesson 2”, “Let Claude work out the details for lesson 2”,
  “Tighten lesson 2 plan and fix style violations” (`f106c4c`, `95f5d39`,
  `f376733`). Dat ritme komt de rest van het jaar terug.
- **Wat twee keer gebeurt, wordt een skill.** Op drie dagen ontstaan
  `/proofread` (17 mei), `/summarize-lesson` en `/design-lesson` (19 mei) en
  `/build-lesson-module` (20 mei). Elke skill werkt in twee fasen: eerst een
  voorstel, pas na mijn akkoord schrijven.
- **De stijlgids groeit uit fouten.** Telkens de agent iets fout doet, wordt het
  een regel: telegramstijl, tautologische bezittelijke voornaamwoorden
  (`2dcfe9e`), anglicismen (`8c0076b`, `e4a1bb6`), kastlijnen, scaffolding in
  lesplannen (`dc3e76b`). Een correctie geef je maar één keer.
- **De echte toets als ijkpunt (28 mei).** De toets van 2025–2026 komt in de
  repo, daarna “Adapt lessons to make sure everything in test 1 was seen”
  (`6f1dba4`, `9f16c6f`). Alignment controleren is iets wat een agent snel en
  grondig doet.

## Fase 4: structuur en één bron van waarheid (juni)

- **De woordenlijst wordt data (1 juni).** In plaats van woordenlijsten met de
  hand bij te houden: één `glossary.yml` en een commando dat elke
  woordenlijstpagina cumulatief genereert (`5aaf5fa`, `882cbff`). De skills
  krijgen de opdracht dat bestand bij te werken, niet de pagina's.
- **Een taxonomie voor kaarten (7 juni).** Syntax-, techniek- en patroonkaarten
  krijgen een definitie in een apart contextbestand, en de skills leren ze
  gebruiken (`3613ef9`, `df24903`).
- **Lesplannen 8 tot 20 in een paar weken.** Tussen 30 mei en 24 juni staan alle
  lesplannen er, inclusief een herschikking van de lusinhoud en drie oude
  toetsen als randvoorwaarde.
- **Cursusbehoefte wordt toolfunctie.** `build-glossary` verhuist op 11 juli
  naar Coursewright, net als de vier lesskills. De cursus is het proefkonijn, de
  tool profiteert.

## Fase 5: onderzoek als toetssteen (juli)

- **Een eigen leidraad, opgesteld met AI.** _Hoe leer je beginners effectief
  programmeren?_ is een werkdocument dat ik met AI-assistentie samenstelde, met
  een literatuurstudie en een reader ernaast. Link met de master onderwijskunde.
- **De cursus doorgelicht tegen die leidraad (2 juli).** Een rapport van 500
  regels over sterktes, reële problemen, differentiatie, mastery learning en AI
  voor remediëring (`011fd04`). De toetsen gelden als vaste randvoorwaarde.

## Fase 6: dingen die vroeger niet haalbaar waren (5–11 juli)

- **Checkpoint-games in een dag (5 juli).** Een engine, een reeks widgettypes,
  zeven vragenbanken in YAML met een validator, een hub en een twintigtal
  minigames, allemaal vanilla JavaScript (`810fc9c` tot `1fd9fba`). Op 11 juli
  een “flashy” laag erbovenop: geluid, animatie, een pixel-art-kaart.
- **Showcase-vraag voor collega's.** Welk materiaal zou je maken als de
  productiekost bijna nul is? De beperking verschuift naar review en didactische
  keuzes.

## Fase 7: de autonome werkrun (11 juli)

- **Alles op één lijst.** Doorlichting, verbeteringsideeën en tooling-ideeën
  worden één geprioriteerde checklist: `pre-quarter-plan-2026-07-11.md`.
- **Agents werken de lijst af, met een logboek.** Een `decision-log.md` houdt
  bij welke beslissing de agent zelf nam, met rationale en commit-hash. Een
  `run-log` toont het verloop, inclusief drie keer een sessielimiet en het
  hervatten. Resultaat op één dag: modules voor les 8 tot 19, klasversies voor
  alle twintig lessen, modeloplossingen, AI-beleid, huiswerkconventies,
  remediëringspakketten, een PDF-builder.
- **Wat de agent bewust niet deed.** Geen Canvas-push zonder credentials,
  officiële JetBrains-screenshots enkel als kandidaat wegens auteursrecht. Alles
  wat mijn oordeel nodig heeft, staat onder “Wacht op Lars”.
- **Bouwen wordt nakijken.** De `production-schedule.md` rekent het modulewerk
  daarna als review: één tot twee uur per module, zips openen in IntelliJ,
  screenshots noteren. Dat is de echte kost, en die moet je inplannen.

## Fase 8: Coursewright wordt een product (augustus)

- **609 commits in een maand.** De naam verandert twee keer: Canvas Local wordt
  Canvas Course Builder (9 augustus) en dan Coursewright (27 augustus). Release
  1.0.0 op 30 augustus.
- **Agent-agnostisch.** Instructies verhuizen van `CLAUDE.md` naar een gedeelde
  `AGENTS.md`, skills naar het open Agent Skills-formaat (10 augustus).
  Collega's zijn niet gebonden aan één AI-tool.
- **Een setup voor collega's.** Setup-wizard, `/course-setup`-skill, thema's en
  exportstijlen, een tutorialmodule. De tool moet werken voor iemand die de
  geschiedenis niet kent.
- **Een grote herschrijving onder toezicht (19–23 augustus).** De push- en
  pull-logica wordt vervangen door een pure three-way planner, met tests en
  bijgewerkte documentatie in hetzelfde ritme. Goed voorbeeld van wat een agent
  aankan als de tests er al staan.
- **Skills voor studenten en AI (29 augustus).** `/ai-tutor-build` en
  `/ai-policy-build`: een AI-module met kopieerbare tutorprompts en een
  AI-beleid op basis van onder meer de AI Assessment Scale.
- **Intussen in de cursus.** Scenario's voor 25 kennisclips (9 augustus), en op
  29 augustus de migratie naar Coursewright: het kader en de stijlgids verhuizen
  naar `context/`.

## Fase 9: een tweede mening van een vers model (2 september)

- **Review door een model dat niets gezien heeft.** `fable-5-1-review.md` leest
  de hele cursus in volgorde, door zes brillen: didacticus, docent, student,
  toekomstige professional, toetsspecialist, eindredacteur. 900 regels.
- **Dezelfde dag verwerkt.** Een dertigtal kleine fixcommits: verkeerde uitvoer,
  verouderde verwijzingen, een vals “één-op-één”, een stille val bij `remove` in
  een for-each (`b5abb9a`, `924bfc3`). Wie het werk schreef, ziet zijn eigen
  fouten slecht. Dat geldt ook voor een agent.

## Fase 10: van repo naar klas (september)

- **Eerste push naar Canvas (7 september).** Daarna bijna dagelijks “Sync
  Canvas”: wat ik in Canvas aanpas (deadlines, volgorde) komt terug in de repo.
- **AI-coaches en studiepakketten (8 september).** Studenten krijgen kopieerbare
  prompts en een gecondenseerde export van de cursus om aan een chatbot te
  geven. Later een eigen skill, `/study-pack-build`.
- **Mijn eigen stem terugzetten.** Op 8 september vier commits “Rewrite in more
  natural language and my tone of voice”, later “Manually edit lesson 1”,
  “Review lesson 2”, “Check lesson 3”, “Check lesson 4”. De agent levert een
  goede eerste versie, de laatste hand blijft de mijne.
- **Toegankelijkheid op vraag.** Een toetsenbordalternatief bij elke
  muisinstructie (14 september), en voor een blinde student een handleiding
  IntelliJ met VoiceOver plus docentnotities (21 september). Op korte termijn
  haalbaar dankzij de agent.
- **Lokale skills voor eigen noden.** `/exit-ticket-build` maakt per les een
  printbaar exit ticket in Word (16 september). Een projectbundel bundelt de
  drie projecten voor collega's (17 september).

## Fase 11: lesgeven met een feedbacklus (22 september–oktober)

- **Retro na elke les.** `/lesson-retro` interviewt mij kort na de les, één
  vraag per keer. Timing en tips gaan naar het lesplan, cursusbrede inzichten
  naar de context, fouten naar een issue queue (`sources/retros/2627/`).
- **Een issue queue voor materiaal (22 september).** `/issue-report` noteert een
  fout in tien seconden, `/issue-fix` werkt de lijst later in één keer af.
  Opmerken en verbeteren zijn twee aparte momenten.
- **Bijsturen tijdens het kwartaal.** `boolean`, `char` en modulo verhuizen naar
  les 4, les 13 en 14 wisselen van plaats, de while-lus gaat uit de toetsen.
  Elke verschuiving raakt lesplannen, modules, games, studiepakketten en
  woordenlijst tegelijk, en de agent houdt die consistent.
- **Per klasgroep.** De retro van les 4 bij groep 1 leidt tot een ingekorte
  versie voor groep 2, dezelfde dag nog (`d83f709`, `18c824a`).

## Fase 12: toetsen en vooruitkijken (oktober–november)

- **Toetsen in A- en B-versie met verbetersleutel.** Test 1 (4 oktober), test 2
  (13 oktober), test 3 (21 oktober) plus een inhaaltest C, telkens met
  startcode, oplossingsprojecten en Word-versies om af te drukken.
- **Toetsbundel op maat.** `npm run build-pdf -- --tot-les N` bundelt
  samenvattingen, kaarten en woordenlijst tot de les van de toets.
- **Retro na een toets.** De retro van test 3 noteert tijdens het toezicht wat
  misloopt: grotere gehelen, chaining zoals `route.getRegio().getProvincie()`,
  testcode lezen. Dat wordt input voor volgend jaar.
- **Al bezig met 2027–2028.** Notities voor de volgende editie staan al in de
  repo, zoals de overstap van `KassaTicket` naar `Verkoop` (`00612e1`).

## Terugkerende patronen

Kandidaten voor de rode draad van de workshop.

- **Context vóór generatie.** Kader, course context, stijlgids, kaarttypes,
  `AGENTS.md`. De kwaliteit van de output volgt uit wat de agent vooraf leest.
- **Een correctie wordt een regel.** Elke fout die ik opmerk, landt in de
  stijlgids of de context, zodat ik ze maar één keer moet geven.
- **Eerst met de hand, dan een skill.** Een workflow wordt pas een skill als ik
  hem een paar keer zelf doorlopen heb.
- **Voorstel, akkoord, uitvoering.** Bijna elke skill stopt na fase A. De agent
  stelt voor, ik beslis.
- **Kleine commits als logboek en vangnet.** Elke stap is terug te draaien, en
  achteraf lees je de geschiedenis als een verslag. Deze chronologie is daar het
  bewijs van.
- **Mechanische controles als vangrail.** `validate`, `build-glossary --check`,
  de games-validator, linkcontrole, tests. Wat een machine kan controleren, laat
  ik niet aan mijn oog over.
- **Genereren is goedkoop, nakijken niet.** Review is het eigenlijke werk, en
  vraagt een planning.
- **Een vers paar ogen.** Doorlichting tegen de literatuur, review door een
  ander model, retro's in de klas.
- **De laatste hand blijft menselijk.** Stem, toon, didactische keuzes, wat er
  in de toets komt.
- **Cursus en tool groeien samen.** Een behoefte in de cursus wordt een functie
  in Coursewright, en daarmee bruikbaar voor collega's.
