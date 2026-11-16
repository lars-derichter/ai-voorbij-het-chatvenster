# Veilig samenwerken met AI met Git

Vraag je AI om een lesfiche te herwerken? Dan wil je achteraf kunnen zien wat
veranderd is en, als het nodig is, terugkeren naar een eerdere versie. Git helpt
je daarbij: het houdt de geschiedenis van je project op je eigen computer bij.

Een **commit** is een opgeslagen moment in die geschiedenis. De projectmap met
haar Git-geschiedenis heet een **repository**. Maak een commit voordat je aan
een grote wijziging begint en telkens wanneer je een zinvolle stap hebt
afgerond. Zo heb je herkenbare momenten om op terug te vallen.

Git bewaart alleen wat je in een commit opneemt. Controleer dus regelmatig wat
nog niet is vastgelegd. Een lokale repository is bovendien geen reservekopie op
een andere plek: als je computer verloren gaat, kan ook de geschiedenis verloren
gaan. Git neemt je inhoudelijke verantwoordelijkheid niet over: controleer de
wijzigingen van AI zelf.

## Maak een oefenproject

In deze oefening gebruik je [GitHub Desktop](https://desktop.github.com/) om Git
met knoppen te bedienen. GitHub is een aparte website; een account is niet nodig
om lokaal te beginnen. Werk met fictieve inhoud.

1. Installeer en open GitHub Desktop. Je kunt een account overslaan zolang je
   alleen lokaal werkt. Geef zo nodig een naam en e-mailadres voor je commits.
2. Kies **File → New repository**. Geef de map een naam, bijvoorbeeld
   `git-oefening`, en kies waar je ze wilt bewaren.
3. Vink **Initialize this repository with a README** aan en kies **Create
   repository**. De map en een eerste commit worden lokaal aangemaakt.
4. Kopieer [writing-style.md](writing-style.md) uit deze repository naar de
   oefenmap. Heb je de repository nog niet op je computer? Open de link, kies op
   GitHub **Download raw file** en bewaar het bestand in de oefenmap.
5. Open de oefenmap in je teksteditor en bekijk `writing-style.md`. Dit
   Markdown-bestand bevat afspraken over de schrijfstijl voor het
   workshopmateriaal. Je werkt met een kopie; het oorspronkelijke bestand
   verandert niet.

In GitHub Desktop toont **History** je opgeslagen momenten.

## Bekijk en bewaar wijzigingen

1. Kies in GitHub Desktop **Changes** en klik op `writing-style.md`. Je ziet
   het nieuwe bestand. Schrijf bij **Summary** bijvoorbeeld `Voeg schrijfstijl
   toe` en klik op **Commit to …**. Nu is de kopie opgenomen in de geschiedenis.
2. Voeg in `writing-style.md` een eigen zin toe en bewaar het bestand.
3. Kies in GitHub Desktop **Changes** en klik op het bestand. Je ziet welke
   regels zijn toegevoegd en verwijderd. Controleer of de wijziging klopt en of
   alleen de gewenste bestanden aangevinkt zijn.
4. Schrijf bij **Summary** een korte omschrijving, bijvoorbeeld
   `Voeg een zin toe`, en klik op **Commit to …**.
5. Kijk in **History**: je ziet nu het nieuwe opgeslagen moment. Pas het bestand
   opnieuw aan en maak nog een commit om de geschiedenis uit te proberen.

Doe hetzelfde nadat AI bestanden heeft aangepast: lees de wijzigingen en bekijk
ook het resultaat in zijn geheel. Neem geen wachtwoorden, geheime sleutels of
andere gegevens op die niet in de geschiedenis thuishoren. Ook een latere
verwijdering haalt zulke gegevens niet vanzelf uit eerdere commits.

## Gebruik Git in VS Code

[VS Code](https://code.visualstudio.com/) kan dezelfde repository tonen en
beheren als GitHub Desktop. Git-ondersteuning is ingebouwd in VS Code, maar
[Git moet ook afzonderlijk geïnstalleerd zijn](https://code.visualstudio.com/docs/sourcecontrol/quickstart).
Herstart VS Code na de installatie als het Git niet vindt. Voor lokaal werken
heb je geen GitHub-account nodig.

1. Open in VS Code via **File → Open Folder** de oefenmap die je hierboven hebt
   gemaakt.
2. Pas `writing-style.md` aan en bewaar het bestand. Kies in de zijbalk **Source
   Control** (het pictogram met vertakkingen).
3. Klik onder **Changes** op het bestand om de wijzigingen te bekijken. Met het
   plusteken naast het bestand kies je het voor de volgende commit; dit heet
   **staging**. Controleer welke bestanden onder **Staged Changes** staan.
4. Typ bovenaan een korte omschrijving en kies **Commit**. De commit verschijnt
   ook in de geschiedenis van GitHub Desktop: beide programma’s gebruiken
   dezelfde lokale repository.

In VS Code kun je via de **Source Control Graph** de geschiedenis van het
project bekijken. Open een bestand en kijk bij **Timeline** om eerdere versies
van dat bestand te onderzoeken. Meer uitleg vind je in de
[documentatie over geschiedenis in VS Code](https://code.visualstudio.com/docs/sourcecontrol/history).

## Laat AI helpen met commits

Als je AI-omgeving toegang heeft tot je projectmap én Git-commando’s mag
uitvoeren, kun je de AI vragen om zelf commits te maken. Of dat kan, hangt af
van de toepassing, de instellingen en de verleende toegang. Een gewone chat die
geen toegang heeft tot je bestanden kan dat niet zelf doen.

Je kunt bijvoorbeeld deze afspraak meegeven bij een opdracht:

```text
Maak eerst een commit van mijn huidige wijzigingen als ik daarom vraag.
Maak daarna een afzonderlijke commit na elke afgeronde, samenhangende stap.
Bekijk vóór elke commit welke bestanden en wijzigingen erin komen. Neem geen
wachtwoorden, sleutels of andere vertrouwelijke gegevens op. Beschrijf elke
commit kort en vertel me welke commits je hebt gemaakt. Verstuur niets naar
GitHub zonder mijn opdracht.
```

Zijn er al wijzigingen die je wilt bewaren? Bekijk ze eerst en vraag de AI om
daarvan een commit te maken. Zo vermijd je dat bestaand werk ongemerkt samen met
nieuwe AI-wijzigingen in één commit terechtkomt. Controleer nadien de
wijzigingen én de geschiedenis in GitHub Desktop of VS Code. Een commit is een
herstelpunt, maar bewijst niet dat de inhoud juist is.

## Bekijk een eerdere versie

Kies in GitHub Desktop **History**, selecteer een commit en klik op een bestand.
Je ziet de wijzigingen die bij dat moment horen. In VS Code kun je de
**Timeline** van een bestand gebruiken om eerdere versies te bekijken en te
vergelijken. Zo kun je bijvoorbeeld een vroegere formulering terugvinden en
kopiëren zonder het hele project terug te draaien.

## Draai wijzigingen terug

Wat je terugdraait, hangt af van de vraag of je al een commit hebt gemaakt.
Probeer dit eerst in je oefenproject.

### Een wijziging vóór een commit

Heb je een bestand aangepast maar nog niet gecommit? In VS Code kun je onder
**Source Control** met de rechtermuisknop op het bestand klikken en **Discard
Changes** kiezen. Lees de bevestiging zorgvuldig: hiermee verwijder je
niet-gecommitte wijzigingen. Bewaar of kopieer eerst wat je mogelijk nog nodig
hebt. Bij een nieuw, nog niet door Git gevolgd bestand kan deze actie het
bestand verwijderen. Als je wijzigingen al hebt geselecteerd voor een commit,
werkt terugdraaien anders; zie de
[documentatie van VS Code](https://code.visualstudio.com/docs/sourcecontrol/staging-commits#_discard-changes).

### Een bestaande commit

Wil je een eerder vastgelegde wijziging ongedaan maken? GitHub Desktop kan een
nieuwe commit maken die de wijzigingen van één eerdere commit terugdraait.

1. Bekijk eerst je huidige wijzigingen en bewaar wat je wilt houden in een
   commit.
2. Kies **History**, klik met de rechtermuisknop op de commit die je wilt
   terugdraaien en kies **Revert Changes in Commit**.
3. Controleer het resultaat. De oorspronkelijke commit blijft in de geschiedenis
   staan; een nieuwe commit draait de wijziging terug.

Dit draait alle wijzigingen uit die ene commit terug. Wil je meerdere commits
terugdraaien, begin dan bij de recentste. Latere wijzigingen aan dezelfde regels
kunnen een conflict veroorzaken. Vraag dan hulp aan AI of raadpleeg de
[documentatie van GitHub Desktop](https://docs.github.com/en/desktop/managing-commits/reverting-a-commit-in-github-desktop)
en controleer het resultaat zelf.

## Zet je repository eventueel op GitHub

Een kopie op GitHub kan helpen om je werk op een andere computer terug te
vinden. Hiervoor heb je een [GitHub-account](https://github.com/) nodig.

1. Meld je in GitHub Desktop aan bij GitHub.
2. Kies **Publish repository**. Controleer de naam en vink **Keep this code
   private** aan als je de repository niet openbaar wilt maken.
3. Kies opnieuw **Publish repository**. Bekijk de repository via **Repository →
   View on GitHub** en controleer de zichtbaarheid.
4. Maak daarna nog een wijziging en commit. Kies **Push origin** om de nieuwe
   commit naar GitHub te versturen. Een commit staat pas op GitHub na een push.

Private betekent dat de repository niet openbaar zichtbaar is, niet dat elk
bestand geschikt is om te uploaden. Controleer welke informatie je deelt en volg
het
[AI-beleid van Thomas More](https://thomasmore365.sharepoint.com/sites/ICTS/Gedeelde%20documenten/Forms/AllItems.aspx?id=%2Fsites%2FICTS%2FGedeelde%20documenten%2F260924%2DTM%2DAD%2DFlow%2EAI%2DOD%202%2DAI%20CC%2DAI%20Beleid%2DDefinitief%20%28TM%2Dversie%29%2Epdf&parent=%2Fsites%2FICTS%2FGedeelde%20documenten)
en andere toepasselijke afspraken voor je materiaal. Geef geen identificerende
gegevens van studenten mee aan AI en laat AI geen studentenwerk quoteren.

## Verder leren

De
[oefening van GitHub Desktop](https://docs.github.com/en/desktop/overview/creating-your-first-repository-using-github-desktop)
en de
[Git-oefening voor VS Code](https://code.visualstudio.com/docs/sourcecontrol/quickstart)
tonen de basisstappen met afbeeldingen. Wil je later samenwerken of
verschillende versies naast elkaar ontwikkelen, lees dan over
[branches](https://docs.github.com/en/get-started/using-github/github-flow) en
[pull requests](https://docs.github.com/en/pull-requests/collaborating-with-pull-requests/proposing-changes-to-your-work-with-pull-requests/about-pull-requests).

Bekijk ook het [overzicht van het workshopmateriaal](README.md).
