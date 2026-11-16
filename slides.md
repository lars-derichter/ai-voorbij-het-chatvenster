---
theme: tm
title: AI voorbij het chatvenster
info: |
  Workshop voor medewerkers van Thomas More.
mdc: true
layout: cover
eyebrow: Workshop
presenter: Lars De Richter
affiliation: Thomas More
hideInToc: true
---

# AI voorbij het chatvenster

Van losse gesprekken naar samenwerken aan bestanden

<!--
Stel jezelf voor. De deelnemers kennen chatbots al. Vandaag kijken we hoe AI
kan helpen bij werk dat uit meerdere bestanden en stappen bestaat.
-->

---

# Vandaag

- Zes principes om met AI samen te werken
- Hoe deze presentatie gemaakt is
- Live: een startgids voor Markdown maken
- Van een taak naar een herbruikbare workflow
- Een eerste stap voor je eigen werk

<!--
De demo staat centraal. Deelnemers hoeven niet mee te werken op een laptop.
Dit project is de rode draad. We maken live een Markdown-startgids in de
projectmap. De vertaling naar het Engels is een tweede toepassing; de
boekvertaling toont hoe ver je een workflow kunt uitbouwen.
-->

---

# Zes principes

1. Werk zo veel en zo lang mogelijk in tekst.
2. Geef context.
3. Weet wat kwaliteit voor jou betekent.
4. Geef heldere instructies en stuur bij.
5. Denk in workflows.
6. Blijf experimenteren.

<!--
Deze principes keren terug in de voorbeelden en op het einde van de workshop.
Ze zijn een manier van werken, geen checklist die je telkens volledig moet
doorlopen. We herkennen ze in dit project en in het maken van de startgids.
-->

---

# Eerst: het kader van Thomas More

- Deel geen identificerende gegevens van studenten.
- Laat AI geen studentenwerk quoteren.
- Controleer het resultaat. Jij blijft verantwoordelijk.
- Wees transparant over betekenisvol AI-gebruik.

[AI-beleid van Thomas More](https://thomasmore365.sharepoint.com/sites/ICTS/Gedeelde%20documenten/Forms/AllItems.aspx?id=%2Fsites%2FICTS%2FGedeelde%20documenten%2F260924%2DTM%2DAD%2DFlow%2EAI%2DOD%202%2DAI%20CC%2DAI%20Beleid%2DDefinitief%20%28TM%2Dversie%29%2Epdf&parent=%2Fsites%2FICTS%2FGedeelde%20documenten)

<!--
Focus vandaag op de technische mogelijkheden, binnen het geldende kader.
Gebruik voor de demo fictief of publiek materiaal. Het beleid vraagt ook
zorgvuldigheid met vertrouwelijke gegevens, auteursrechten en brongebruik.
-->

---
layout: section
color: navy
number: "01"
eyebrow: Van gesprek naar project
---

# Geef AI een werkplek

Bestanden en afspraken blijven bij elkaar.

---
layout: two-cols-tm
---

# Chat, Work en Codex

::left::

**Chat**

Vragen stellen, ideeën verkennen, samen denken.

**Work**

Taken uitvoeren met bestanden en hulpmiddelen.

::right::

**Codex**

Werken aan code en projecten, ook met documenten.

Vandaag gebruiken we **Work** in de ChatGPT-desktopapp.

<!--
Toon de app en hoe je een lokaal project opent en toegang tot een map geeft.
Beschikbaarheid hangt af van het abonnement en de instellingen van de
werkruimte. Codex is voor deze workshop geen vereiste.
-->

---

# Aan de slag met Work

1. Installeer en open de ChatGPT-desktopapp.
2. Kies **Work** en open een lokaal project.
3. Geef toegang tot de map waarin je wilt werken.
4. Beschrijf de taak en bekijk de wijzigingen.

<!--
Toon de stappen in de Thomas More-omgeving. Work en toegang tot lokale
bestanden hangen af van abonnement en instellingen. Een project brengt werk
samen; toegang tot de lokale map laat de agent met bestanden daarin werken.
Codex is afzonderlijk beheerd en is hier niet nodig.
-->

---

# Deze presentatie is een project

```text
ai-voorbij-het-chatvenster/
├── slides.md          ← deze presentatie
├── sources/           ← ideeën en bronnen
├── writing-style.md   ← afspraken over stijl
└── AGENTS.md          ← afspraken voor het project
```

<!--
Open de echte map in Work en eventueel in VS Code. Deze presentatie is samen
met AI gemaakt en door Lars bijgestuurd. Laat zien dat de bestanden die het
verhaal ondersteunen samen in de projectmap staan. Maak duidelijk welke
bestanden de agent mag gebruiken en waar hij mag schrijven.
-->

---

# 1. Werk zo veel mogelijk in tekst

- Je kunt tekst makkelijk lezen, aanpassen en vergelijken.
- AI kan rechtstreeks met je bestanden werken.
- Vanuit één bron kun je naar andere formaten exporteren.

<!--
Deel je eigen ervaring: zo veel en zo lang mogelijk in tekst werken maakt je
workflow efficiënter. Tekst kan ook de bron zijn voor Word of PDF. Een tool
zoals Pandoc helpt bij omzetting; vraag AI om daarbij te helpen.
-->

---

# Van tekst naar een document

**Schrijf en bewaar** je inhoud in Markdown.

**Bewerk en vergelijk** bestanden in een teksteditor, zoals VS Code.

**Exporteer** bijvoorbeeld naar Word of PDF, met hulp van AI en Pandoc.

<!--
Toon eventueel de tekst en de weergave naast elkaar in VS Code. Pandoc is een
hulpmiddel om documenten om te zetten; de exacte mogelijkheden en opmaak hangen
af van het formaat en de gekozen instellingen. Vraag AI om te helpen bij de
omzetting en controleer het geëxporteerde resultaat. Deze presentatie gebruikt
Slidev om slides.md als presentatie te tonen.
-->

---

# Markdown: tekst met eenvoudige opmaak

```markdown
# Een titel

Een alinea met **nadruk**.

- Een eerste punt
- Een tweede punt
```

Leesbaar als tekst én om te zetten naar andere formaten.

<!--
Toon het bestand en de weergave naast elkaar. Je hoeft Markdown niet volledig
uit het hoofd te kennen: laat AI helpen met de opmaak.
-->

---
layout: section
color: navy
number: "02"
eyebrow: Demonstratie
---

# Live: een Markdown-startgids

Samen plannen, maken, nakijken en delen.

<!--
De gids bestaat nog niet: we maken hem tijdens de workshop. Bereid een
reserveversie voor en test vooraf hoe het delen via de repository werkt. Als
de live uitvoering vastloopt, toon je de reserveversie en benoem je wat er
gebeurd is. Publiceer pas na nazicht; ga niet uit van automatische publicatie.
-->

---

# Begin met een duidelijke opdracht

> Maak een startgids waarmee collega's zelfstandig Markdown kunnen gebruiken.
> Stel eerst een plan voor en wacht op mijn feedback.

Geef ook mee: voorkennis, doel, voorbeelden en waar de gids moet komen.

<!--
Open dit project in Work. De prompt is een startpunt: vraag om een beknopte,
zelfstandig bruikbare gids in Markdown met voorbeelden om uit te proberen.
Vraag de agent om de projectafspraken en schrijfstijl te lezen en relevante
bronnen te gebruiken. Spreek af waar het bestand komt. Toon het plan, geef
feedback en keur het goed vóór de agent de gids uitwerkt.
-->

---

# 2. Geef context

- **Bronnen:** wat moet de AI weten?
- **Afspraken:** wat geldt voor dit project?
- **Opdracht:** wat wil je nu bereiken?

<!--
Toon sources/, writing-style.md en AGENTS.md in de projectmap. Maak onderscheid
tussen bronmateriaal, blijvende projectafspraken en de huidige opdracht.
Vraag AI om je te interviewen als je je eigen verwachtingen nog wilt uitklaren.
-->

---

# Welke context hoort waar?

- **Persoonlijke instructies:** voorkeuren voor je gesprekken.
- **Bronnen in je map:** materiaal dat relevant is voor deze taak.
- **`AGENTS.md`:** afspraken die bij het project horen.
- **Je opdracht:** wat je nu wilt laten doen.

<!--
Bijvoorbeeld: een persoonlijke voorkeur voor helder Nederlands, de outline als
bron, writing-style.md en AGENTS.md als projectafspraken, en de huidige
opdracht om een Markdown-startgids te maken. De beschikbaarheid en werking van
instructies verschilt per toepassing en instelling.
-->

---

# Laat AI je interviewen

> Help me om mijn verwachtingen voor deze startgids helder te krijgen.
> Stel me één vraag per keer.

Bewaar de afspraken die later opnieuw van pas komen.

<!--
Een interview kan helpen om doelgroep, voorkennis, toon of kwaliteitscriteria
concreet te maken. Beslis zelf welke antwoorden en afspraken je bewaart en waar.
-->

---

# `AGENTS.md`: afspraken voor dit project

```markdown
# Afspraken

- Leg inhoudelijke keuzes eerst voor in een plan.
- Lees writing-style.md voor publiek zichtbare tekst.
- Verifieer feiten en actuele functies.
- Lever documentatie als Markdown aan.
```

<!--
Dit zijn beknopte parafrases van afspraken uit het echte projectbestand. Open
AGENTS.md om de volledige afspraken te tonen. Toon hoe je samen met AI
afspraken opstelt en aanpast. Afspraken blijven mensenwerk en zijn geen garantie
dat de agent ze perfect volgt.
-->

---

# 3. Weet wat kwaliteit betekent

Wat maakt een resultaat voor jou goed?

- Welke voorbeelden vind je sterk?
- Welke fouten zijn onaanvaardbaar?
- Wat moet je zelf beoordelen?

<!--
Kwaliteitsbesef en smaak zijn belangrijk wanneer produceren makkelijker wordt.
Maak verwachtingen concreet met voorbeelden en criteria; toets die ook aan het
resultaat. Een agent kan helpen controleren, maar neemt je oordeel niet over.
-->

---

# 4. Geef heldere instructies en stuur bij

Zeg wat je wilt bereiken, voor wie en met welke randvoorwaarden.

Je prompt hoeft niet perfect te zijn: stel vragen en verfijn samen.

---

# Eerst plannen, dan bijsturen

1. Laat een plan voorstellen.
2. Kijk na en stuur bij.
3. Laat de AI uitvoeren.
4. Controleer en verbeter het resultaat.

<!--
Laat zien wat je in het plan zou veranderen. Een goed plan helpt, maar ook
tijdens de uitvoering kun je bijsturen en achteraf blijft controle nodig.
-->

---

# Wat maakt deze startgids goed?

- Kan een beginner er zelfstandig mee aan de slag?
- Zijn de uitleg en voorbeelden juist en duidelijk?
- Kan de lezer iets uitproberen en het resultaat herkennen?

<!--
Bekijk samen minstens één uitleg en probeer een voorbeeld uit. Controleer
juistheid, duidelijkheid en links. Toon een verbetering of vraag een aanpassing.
Laat zien hoe je wijzigingen bekijkt. Lars beoordeelt de gids vóór die gedeeld
wordt; reserveer tijd voor een laatste controle en de publicatiestap.
-->

---
layout: section
color: navy
number: "03"
eyebrow: Van taak naar workflow
---

# Doe je dit vaker?

Maak je werkwijze herbruikbaar.

---

# 5. Denk in workflows

Welke stappen herhaal je, en waar wil je zelf beslissen?

**Startgids:** context lezen → plan → feedback → schrijven → controleren.

Maak van een aanpak die werkt een herbruikbare skill.

---

# Een skill is een herbruikbare werkwijze

Een map met instructies en eventueel voorbeelden of hulpmiddelen.

```text
.agents/skills/gids-maken/
└── SKILL.md
```

Bijvoorbeeld: eerst een plan, dan feedback, daarna schrijven en controleren.

<!--
Vertrek van de werkwijze die je net hebt doorlopen. Laat AI helpen om de stappen
als skill op te schrijven wanneer je vaker gidsen maakt. De map op de slide is
een illustratief voorbeeld, geen bestaande skill. In de geteste omgeving worden
skills in de projectmap gevonden; instellingen kunnen per omgeving verschillen.
-->

---

# Skills in ons project

- Bewaar een skill in `.agents/skills` in je projectmap.
- In onze geteste omgeving wordt die daar gevonden.
- Centrale skills en plugins zijn in onze installatie niet beschikbaar.

<!--
Toon waar SKILL.md staat en hoe je de skill laat gebruiken. Dit beschrijft de
geteste installatie; functies en toegang kunnen in een andere omgeving anders
zijn. Een skill kan ook voorbeelden en aanvullende bestanden bevatten.
-->

---

# Nog een voorbeeld: vertalen

**Opdracht:** vertaal een tekst naar het Engels.

**Context:** doelgroep, gewenste toon en woordenlijst.

**Controle:** betekenis, termen, cijfers en leesbaarheid.

<!--
Verbind dit met werk buiten het onderwijs: een handleiding of projecttekst voor
internationale collega's. Een eenvoudige vertaling kan uitgroeien tot een
herbruikbare skill. Controleer de vertaling ook zelf.
-->

---

# Wat is een agent?

Een **agent** voert een taak uit en kan hulpmiddelen gebruiken.

Een **subagent** krijgt een afgebakende deeltaak en rapporteert terug.

Jij bepaalt de opdracht en beoordeelt het resultaat.

---

# Een team van agents

- Een **manager** bewaakt het geheel en de eindkwaliteit.
- Subagents krijgen elk een duidelijke deeltaak.
- Ze controleren hun werk en rapporteren aan de manager.

<!--
In mijn favoriete opzet gebruikt de manager een sterk model met een hogere
redeneerinspanning; een eenvoudiger model kan volstaan voor een afgebakende
deeltaak. De mogelijkheden en modelkeuze hangen af van de toepassing en de
omgeving. Een manager neemt onze verantwoordelijkheid voor de eindkwaliteit
niet weg.
-->

---

# Hoe ver kun je gaan?

Een boekvertaling met AI-agents:

- een manager verdeelt en bewaakt het werk;
- andere agents vertalen en controleren onderdelen;
- vaste controles en menselijke feedback verbeteren het resultaat.

<!--
Een agent voert een taak uit en kan daarbij hulpmiddelen gebruiken. Een
subagent krijgt een afgebakende deeltaak. Dit is een blik op een complexere
workflow, niet iets wat deelnemers eerst moeten bouwen. In dit praktijkvoorbeeld
gaat het om een eerste vertaling die de auteurs nog nalezen.
-->

---

# 6. Blijf experimenteren

- Welke taak doe je vaker?
- Welke bronnen en afspraken heeft AI nodig?
- Hoe herken jij een goed resultaat?
- Welk werk besteed je graag uit?

<!--
Vraag AI om mee te denken of om je te interviewen. Besteed vooral taken uit
waar je zelf minder voldoening uit haalt. AI kan verrassend sterk zijn in de ene
taak en tekortschieten in een schijnbaar vergelijkbare taak: blijf testen.
-->

---

# Vraag AI om mee te denken

> Ik doe regelmatig deze taak. Hoe zou AI me daarbij kunnen helpen?
> Stel vragen om mijn werkwijze te begrijpen.

Probeer een kleine stap uit en kijk wat voor jou werkt.

---

# De mogelijkheden zijn grillig

AI kan verrassend goed zijn in een moeilijke taak en struikelen over iets dat
eenvoudig lijkt.

**Test, controleer en leer waar de grenzen voor jouw werk liggen.**

<!--
Dit wordt ook de jagged frontier genoemd: de grens van AI-capaciteiten is niet
rechtlijnig. Wat werkt hangt onder meer af van de taak, het model en de context.
Koppel dit aan een concreet voorbeeld uit de demonstratie.
-->

---

# Probeer ook je eigen opdracht

Geef je studentenopdracht aan het beste model dat je kunt gebruiken.

**Mijn stelling:** een op zichzelf staand essay is geen valide evaluatie meer.

Wat betekent het resultaat voor wat je wilt beoordelen?

<!--
Een bewust prikkelende stelling: een op zichzelf staand essay is geen valide
evaluatie meer, zeker wanneer een student AI goed kan aansturen en het resultaat
bijstuurt. Gebruik dit als uitnodiging om samen na te denken over wat je wilt
beoordelen. Geef geen identificerende studentgegevens mee.
-->

---

# De zes principes, nog eens

1. Werk zo veel en zo lang mogelijk in tekst.
2. Geef context.
3. Weet wat kwaliteit voor jou betekent.
4. Geef heldere instructies en stuur bij.
5. Denk in workflows.
6. Blijf experimenteren.

<!--
Verbind elk principe kort met de presentatie, de startgids en het vertaalvoorbeeld.
Deelnemers kunnen één principe kiezen om zelf mee te beginnen.
-->

---

# Je eerste stap

1. Kies een kleine, terugkerende taak.
2. Maak een map met geschikte bronnen.
3. Open de map in Work en beschrijf je opdracht.
4. Vraag een plan, stuur bij en kijk het resultaat na.

<!--
Verwijs na afloop naar de repository en de startgids zodra die gedeeld is.
Daarna kun je projectafspraken toevoegen en een workflow
in een skill bewaren. Markdown en Git kun je verder verkennen op je eigen tempo.
-->

---

# Verder aan de slag

- Verken de repository en de bestanden van deze presentatie.
- Gebruik de Markdown-startgids die we vandaag maken.
- Leer werken met Markdown en pas een tekstbestand aan.
- Probeer projectinstructies en een skill uit.
- Leer Git gebruiken om wijzigingen te volgen en te bewaren.

<!--
De repository is de verzameling bestanden bij deze workshop. Deel de link naar
de gids zodra die is gepubliceerd. Git is een hulpmiddel voor versiebeheer;
je hoeft het niet te beheersen om met de eerste stappen te beginnen.
-->

---

# Bronnen en verder lezen

- [AI-beleid van Thomas More](https://thomasmore365.sharepoint.com/sites/ICTS/Gedeelde%20documenten/Forms/AllItems.aspx?id=%2Fsites%2FICTS%2FGedeelde%20documenten%2F260924%2DTM%2DAD%2DFlow%2EAI%2DOD%202%2DAI%20CC%2DAI%20Beleid%2DDefinitief%20%28TM%2Dversie%29%2Epdf&parent=%2Fsites%2FICTS%2FGedeelde%20documenten)
- [ChatGPT Work en Codex](https://help.openai.com/en/articles/20001275-chatgpt-work-and-codex)
- [Skills bouwen](https://learn.chatgpt.com/docs/build-skills)
- [Instructies met AGENTS.md](https://learn.chatgpt.com/docs/agent-configuration/agents-md)
- [Markdown Guide](https://www.markdownguide.org/basic-syntax/)
- [Pandoc](https://pandoc.org/)
- [Git: aan de slag](https://git-scm.com/book/en/v2/Getting-Started-About-Version-Control)

---
layout: end
color: navy
contact: |
  Lars De Richter
  lars.derichter@thomasmore.be
hideInToc: true
---

# Bedankt!

Wat wil jij eens proberen?
