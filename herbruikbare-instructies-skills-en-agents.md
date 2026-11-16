# Herbruikbare instructies, skills en agents

Bij een terugkerende taak kun je afspraken bewaren in je projectmap. Zo geef je
een AI-assistent context mee die ook bij een volgende opdracht nuttig is. Begin
met een kleine taak uit de [startgids voor Work](startgids-work.md).

## Persoonlijke instructies

Met persoonlijke instructies, of _custom instructions_, geef je ChatGPT algemene
voorkeuren mee voor je gesprekken. In de desktopapp vind je ze via **Settings →
Personalization → Custom Instructions**. Schakel daar ook de personalisatie in.
Lees meer in de
[uitleg van OpenAI](https://help.openai.com/en/articles/8096356-chatgpt-custom-instructions).

Dit voorbeeld is gebaseerd op de instructies van Lars. Pas het aan je eigen werk
en voorkeuren aan:

```text
Ik werk als docent in het hoger onderwijs.

- Stel bij een grotere opdracht eerst een plan voor en wacht op mijn akkoord.
- Vraag om verduidelijking als belangrijke informatie ontbreekt.
- Wees kritisch en zeg het als mijn redenering niet klopt.
- Controleer je werk en vermeld wat je hebt nagekeken.
- Schrijf helder en beknopt. Geef onzekerheid duidelijk aan.
- Gebruik Markdown voor documenten, tenzij ik een ander formaat vraag.
```

Bekijk ook de
[volledige persoonlijke instructies van Lars](persoonlijke-instructies-lars.md).

## Projectinstructies: afspraken voor je map

Een bestand `AGENTS.md` kan afspraken voor een project bevatten, bijvoorbeeld
voor wie je schrijft en wanneer je eerst een plan wilt zien. Maak in je
projectmap een tekstbestand met die naam en pas dit voorbeeld aan:

```markdown
# Afspraken voor dit project

- Schrijf in helder Nederlands voor docenten.
- Stel bij inhoudelijke keuzes eerst een plan voor en wacht op mijn feedback.
- Gebruik alleen de bronnen die relevant zijn voor de opdracht.
- Bewaar de checklist als Markdown in deze map.
```

Vraag Work bij je volgende opdracht om `AGENTS.md` te lezen en de afspraken toe
te passen. Controleer in het antwoord en het resultaat of dat gebeurt. Hoe een
toepassing instructiebestanden automatisch inleest, verschilt per toepassing en
omgeving. De
[documentatie over AGENTS.md](https://learn.chatgpt.com/docs/agent-configuration/agents-md)
beschrijft de werking voor Codex; ga niet zonder controle uit van dezelfde
werking in Work.

Het [projectbestand van deze workshop](AGENTS.md) is een uitgebreider voorbeeld.
Neem alleen afspraken over die voor jouw project nuttig zijn.

## Skills: een aanpak opnieuw gebruiken

Een skill bundelt een werkwijze voor een bepaalde taak. De voorbeeldskill
[presentatie-ontwerpen](.agents/skills/presentatie-ontwerpen/SKILL.md)
beschrijft bijvoorbeeld hoe je context verzamelt, een voorstel bespreekt en een
presentatie controleert. Het bestand heet `SKILL.md` en staat in een eigen map
onder `.agents/skills`.

Wil je de aanpak uitproberen? Kopieer de volledige map `presentatie-ontwerpen`
naar `.agents/skills` in je eigen project. Open daarna een nieuw Work-gesprek in
dat project en vraag expliciet om de skill te gebruiken. Vindt Work de skill
niet, verwijs dan naar het bestand en vraag om het te lezen. Controleer de
stappen en pas de instructies aan je eigen werkwijze aan. De automatische
herkenning en beschikbare functies hangen af van je toepassing en omgeving.

Lees meer over het maken en gebruiken van skills in de
[officiële documentatie](https://learn.chatgpt.com/docs/build-skills). Die
beschrijft ook functies en locaties voor Codex; controleer wat voor jouw
Work-omgeving geldt. In de [collectie voor onderwijsontwerp](skills/README.md)
vind je meer skills die je kunt bekijken en aanpassen.

## Agents: een taak laten uitvoeren

Een agent is een AI-assistent die een opdracht uitvoert en daarbij beschikbare
hulpmiddelen kan gebruiken, bijvoorbeeld om bestanden te lezen en te wijzigen.
Sommige toepassingen kunnen een deel van het werk aan andere agents uitbesteden;
of dat kan, hangt af van de omgeving. Begin eenvoudig met één duidelijke
opdracht, bijvoorbeeld:

```text
Lees AGENTS.md en gebruik de skill presentatie-ontwerpen uit mijn project.
Help me een korte presentatie voor nieuwe collega's te plannen. Stel eerst
vragen over doel en publiek en wacht op mijn akkoord voor je slides schrijft.
```

Bekijk het voorgestelde plan, geef feedback en controleer het resultaat. Een
projectinstructie of skill helpt richting geven, maar jij blijft
verantwoordelijk voor de inhoud en beslist wat wordt gedeeld.

Wil je wijzigingen volgen en eerdere versies bewaren? Ga verder met de
[startgids Git](startgids-git.md).
