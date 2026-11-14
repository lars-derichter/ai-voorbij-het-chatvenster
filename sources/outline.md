- Intro:
  - voorstellen
  - niet ethiek, milieu etc. ; focus ligt vandaag op het technische
  - kader van Thomas More wel kort overlopen
- Chat vs work vs codex
  - chat voor vragen, voor brainstorm ...
  - work:
    - installeer de app
    - voor werken met documenten
    - gebruik projecten
    - geef een project toegang tot een folder op je computer
  - codex:
    - voorlopig geen toegang
    - voor code, maar werkt ook heel goed met documenten, kan je integreren in
      je editor
- Principes:
  - Zoveel (en zo lang) mogelijk in tekst werken
    - Text editor gebruiken (VS Code)
    - Techniek: markdown als formaat
    - Markdown omzetten (pandoc, laat de llm je helpen)
  - Context is king:
    - Custom instructions in ChatGPT
    - Verzamel relevante documenten (sources folder)
    - AGENTS.md in project folder
    - Tip: laat jezelf interviewen
  - Kwaliteit:
    - wat betekent goed
    - kwaliteitsbesef en smaak worden de belangrijkste vaardigheden in het
      AI-tijdperk
  - Heldere instructies:
    - geef heldere duidelijke instructies (maar maak het niet moeilijker dan
      nodig, je hoeft niet perfect te zijn)
    - laat de AI eerst een plan maken, kijk het plan goed na, eens het plan oke
      is, mag je vertrouwen hebben
    - kijk resultaat na, werk iteratief
  - Workflows:
    - Denk in workflows
    - Als je iets vaker doet: maak een skill (spijtig genoeg hebben we met onze
      installatie geen toegang tot centrale skills en plugins, maar je kan wel
      skills in je project folder kopiëren in de .agents folder)
    - Complexe workflows: agent met subagents
      - wat is een agent?
      - mijn favoriete workflow:
        - Eén manager-agent die het hele proces overziet, die subagents
          aanstuurt en die verantwoordelijk is voor de eindkwaliteit (sterk
          model, met hoge effort)
        - Voor elke subtaak een nieuwe agent, kan vaak een eenvoudiger model
          zijn (krijgt een specifieke taak, controleert de eigen kwaliteit voor
          doorsturen naar de manager)
        - kan heel complex en diep: voorbeeld boekvertaling
  - Probeer dingen uit:
    - test wat voor jou werkt, laat de ai je helpen om je te helpen
    - vraag hoe de ai je kan helpen bij een bepaalde taak
    - laat de ai je interviewen
    - weeg af: besteed vooral uit wat je zelf niet zoveel voldoening uit haalt
    - the jagged frontier
    - bonus: geef de opdrachten die je aan je studenten geeft aan de ai (best
      mogelijke model waartoe je toegang hebt) (en schrik niet; een op zichzelf
      staand essay is geen valide evaluatie meer, zeker niet als de student in
      kwestie goed kan prompten en de moeite neemt om het resultaat nog wat bij
      te sturen)
  - Volgende stappen:
    - exploreer de repository die bij deze workshop hoort
    - leer met markdown werken
    - leer git gebruiken
