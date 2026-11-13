# AI voorbij het chatvenster

## Project en publiek

Deze repository ondersteunt een Nederlandstalige workshop van één uur voor
ongeveer 50 docenten en andere medewerkers van Thomas More. De deelnemers hebben
ervaring met chatbots en zijn bereid iets met de computer uit te proberen, maar
kunnen onzeker zijn over technische onderwerpen.

De workshop inspireert deelnemers om na afloop zelf met lokale projecten en
bestanden aan de slag te gaan: Markdown gebruiken, samen met AI
projectinstructies in `AGENTS.md` schrijven en skills toevoegen, aanpassen,
maken en gebruiken. Toon hoe dat in de ChatGPT-desktopapp kan werken; VS Code
kan dienen om de bestanden en wijzigingen te volgen. Ga niet uit van toegang tot
Codex. Alle medewerkers hebben recent toegang gekregen tot ChatGPT Edu, maar
controleer welke functies binnen de gebruikte omgeving beschikbaar zijn.

De sessie combineert voorbereide voorbeelden met demonstraties. Ga er niet van
uit dat deelnemers een laptop bijhebben of live kunnen volgen. Lesmateriaal is
het belangrijkste toepassingsgebied; maak ook de relevantie voor andere taken
van hogeschoolmedewerkers zichtbaar. De herwerking van Programming Fundamentals
en Coursewright zijn mogelijke voorbeelden, maar de rode draad en tijdsverdeling
liggen nog niet vast.

## Samenwerken

- Leg bij inhoudelijke keuzes eerst een concreet plan voor. Wacht op de
  goedkeuring van Lars voordat je de bijbehorende aanpassingen uitvoert; verwerk
  zijn feedback in het plan.
- Lees `writing-style.md` in de hoofdmap vóór je teksten schrijft die zichtbaar
  zijn voor het publiek, waaronder slides, README en ondersteunend materiaal.
  Als het bestand ontbreekt, vraag Lars erom voordat je die teksten schrijft.
- Verifieer feiten en actuele functies. Geef aan wanneer beschikbaarheid afhangt
  van abonnement, instellingen of omgeving; presenteer aannames niet als feiten.
  Controleer ook of een toepassing `AGENTS.md` en skills daadwerkelijk
  ondersteunt en hoe ze worden ingelezen.
- Behandel aanvullingen in `sources/` als bronnen, niet automatisch als
  vaststaande feiten of goedgekeurde keuzes. Lees de bronnen die relevant zijn
  voor de opdracht en houd de verwijslijst hieronder beknopt en actueel.

## Materiaal en presentatie

- Schrijf voor het publiek in helder, goed leesbaar Nederlands, volgens
  `writing-style.md`. Vertrek vanuit concrete voorbeelden, leg nodige begrippen
  uit en beperk jargon.
- Houd de slides sober en met weinig tekst. Vermeld bronnen aan het einde.
- De repository wordt publiek op GitHub; de slides worden gepubliceerd via
  GitHub Pages. Ontwikkel ook een goede README als ingang voor bezoekers, een
  zelfstandig bruikbare startgids, links naar documentatie en voorbeeldbestanden
  die deelnemers kunnen overnemen. De exacte invulling volgt uit inhoudelijke
  keuzes die eerst met Lars worden besproken.
- Besteed kort aandacht aan grenzen: geef geen identificerende gegevens van
  studenten mee, laat AI nooit studentenwerk quoteren en blijf zelf
  verantwoordelijk. Verwijs naar het
  [AI-beleid van Thomas More](https://thomasmore365.sharepoint.com/sites/ICTS/Gedeelde%20documenten/Forms/AllItems.aspx?id=%2Fsites%2FICTS%2FGedeelde%20documenten%2F260924%2DTM%2DAD%2DFlow%2EAI%2DOD%202%2DAI%20CC%2DAI%20Beleid%2DDefinitief%20%28TM%2Dversie%29%2Epdf&parent=%2Fsites%2FICTS%2FGedeelde%20documenten);
  Raadpleeg `sources/tm-ai-beleid.md` voor de inhoud en vul die niet op basis
  van aannames in. De pdf-versie is bedoeld voor menselijke lezers.
- Lever documentatie als Markdown aan, tenzij een opdracht om een ander formaat
  vraagt.

## Relevante bestanden

- `writing-style.md` — verplicht lezen vóór publiek zichtbare tekst wordt
  geschreven.
- `sources/workflow-ontwikkeling-cursus-pf-coursewright.md` — ruwe chronologie
  en mogelijke voorbeelden uit de ontwikkeling van de cursus en Coursewright.
- `sources/tm-ai-beleid.md` — tekstversie van het AI-beleid van Thomas More;
  gebruik deze versie als agent. `sources/tm-ai-beleid.pdf` is voor mensen.
- `slides.md` — de enige actieve Slidev-presentatie; bevat momenteel nog de
  voorbeelddia’s van het Thomas More-thema.
- `README.md` — huidige projectdocumentatie; bevat nog informatie uit het
  oorspronkelijke sjabloon en moet later een ingang voor bezoekers worden.
- `package.json` en `.github/workflows/deploy.yml` — beschikbare commando’s,
  afhankelijkheden en publicatie-instellingen.

## Technische afspraken

De presentatie gebruikt [Slidev](https://sli.dev) met `theme: tm`. Bewerk
`slides.md`; de ontwikkelserver vernieuwt de presentatie bij opslaan.

```bash
npm install
npm run dev      # ontwikkelserver met browser
npm run build    # statische site in dist/
npm run export   # PDF-export
```

Beide eigen thema’s staan als vastgepinde Git-afhankelijkheden in
`package.json`: `slidev-theme-tm` en `slidev-theme-ldr`. Verwijder het
ongebruikte thema niet zomaar. De thema’s hebben verschillende layouts en
accentklassen; wisselen vergt meer dan alleen de frontmatter aanpassen. Ze
bevatten Vue- en CSS-broncode en hebben geen aparte buildstap nodig. Voor een
thema-update moet eerst een nieuwe tag in de themarepository worden gemaakt,
daarna de pin worden aangepast en `npm install` worden uitgevoerd.

De GitHub Actions-workflow bouwt en publiceert naar GitHub Pages bij een push
naar `main`; de basis-URL gebruikt automatisch de repositorynaam. `dist/` is
gegenereerde uitvoer en wordt niet gecommit. Prettier met
`prettier-plugin-slidev` formatteert `slides.md` en `slides-*.md`.
