# Starten met Git

Met Git bewaar je de geschiedenis van een project op je eigen computer. Je kunt
zien wat er veranderde en een eerdere versie terughalen. Dat is handig voor
lesmateriaal, ook als je alleen werkt en niets online zet. Een opgeslagen
moment heet een **commit**; de projectmap met haar geschiedenis heet een
**repository**.

In deze oefening gebruik je [GitHub Desktop](https://desktop.github.com/) om
Git met knoppen te bedienen. GitHub is een aparte website waar je later een
kopie kunt bewaren. Begin met een nieuwe oefenmap en fictieve inhoud.

## Maak een lokale repository

1. Installeer en open GitHub Desktop. Je kunt een account overslaan zolang je
   alleen lokaal werkt. Geef zo nodig een naam en e-mailadres voor je commits.
2. Kies **File → New repository**. Geef de map een naam, bijvoorbeeld
   `git-oefening`, en kies waar je ze op je computer wilt bewaren.
3. Vink **Initialize this repository with a README** aan en kies **Create
   repository**. De map en een eerste commit worden lokaal aangemaakt.
4. Open de map in je teksteditor en bekijk `README.md`. Dit is een gewoon
   Markdown-bestand in je project.

In GitHub Desktop toont **History** je opgeslagen momenten. Een lokale
repository is geen reservekopie op een andere plek: als je computer verloren
gaat, kan die geschiedenis ook verloren gaan.

## Bewaar je wijzigingen

1. Voeg in `README.md` een titel of korte beschrijving toe en bewaar het bestand.
2. Ga terug naar GitHub Desktop en kies **Changes**. Klik op het bestand om te
   zien wat veranderde. Controleer dat alleen de gewenste bestanden aangevinkt
   zijn.
3. Schrijf bij **Summary** een korte omschrijving, bijvoorbeeld `Beschrijf de
   oefening`, en klik op **Commit to …**.
4. Kijk in **History**: je ziet nu het nieuwe opgeslagen moment. Pas het
   bestand opnieuw aan en maak nog een commit om de geschiedenis uit te proberen.

Herhaal dit wanneer je een zinvolle stap hebt afgerond. Een commit beschrijft
een samenhangende wijziging en blijft lokaal tot je ze naar GitHub verstuurt.

## Zet je repository eventueel op GitHub

Een kopie op GitHub kan helpen om je werk op een andere computer terug te
vinden. Hiervoor heb je een [GitHub-account](https://github.com/) nodig.

1. Meld je in GitHub Desktop aan bij GitHub.
2. Kies **Publish repository**. Controleer de naam en vink **Keep this code
   private** aan als je de repository niet openbaar wilt maken.
3. Kies opnieuw **Publish repository**. Bekijk de repository op GitHub via
   **Repository → View on GitHub** en controleer de zichtbaarheid.
4. Maak daarna nog een wijziging en commit. Kies **Push origin** om de nieuwe
   commit naar GitHub te versturen. Een commit staat pas op GitHub na een push.

Met een [gratis persoonlijk GitHub-account](https://docs.github.com/en/get-started/learning-about-github/types-of-github-accounts)
kun je al private repositories maken. Docenten kunnen ook [GitHub Education
voor docenten aanvragen](https://docs.github.com/en/education/about-github-education/github-education-for-teachers/apply-to-github-education-as-a-teacher);
na verificatie zijn er bijkomende voordelen. GitHub vermeldt onder meer gratis
Copilot Pro en de mogelijkheid GitHub Team aan te vragen in de
[actuele voordelen voor docenten](https://docs.github.com/en/education/about-github-education/github-education-for-teachers/about-github-education-for-teachers).
Controleer daar welke voordelen momenteel gelden: een gratis persoonlijk GitHub
Pro-abonnement voor docenten konden we in de actuele documentatie niet bevestigen.

Private betekent dat de repository niet openbaar zichtbaar is, niet dat elk
bestand geschikt is om te uploaden. Controleer welke informatie je deelt en
volg het [AI-beleid van Thomas More](https://thomasmore365.sharepoint.com/sites/ICTS/Gedeelde%20documenten/Forms/AllItems.aspx?id=%2Fsites%2FICTS%2FGedeelde%20documenten%2F260924%2DTM%2DAD%2DFlow%2EAI%2DOD%202%2DAI%20CC%2DAI%20Beleid%2DDefinitief%20%28TM%2Dversie%29%2Epdf&parent=%2Fsites%2FICTS%2FGedeelde%20documenten)
en andere toepasselijke afspraken voor je materiaal.

## Draai een wijziging terug

In **History** kun je een commit en een bestand selecteren om de bijbehorende
wijzigingen te bekijken. Wil je de wijzigingen van één commit ongedaan maken,
bijvoorbeeld de laatste aanpassing aan je oefenbestand?

1. Zorg dat je huidige wijzigingen eerst zijn opgeslagen in een commit.
2. Klik in **History** met de rechtermuisknop op de commit met de wijziging die
   je wilt terugdraaien en kies **Revert Changes in Commit**.
3. GitHub Desktop maakt een nieuwe commit die die wijziging terugdraait. De
   oorspronkelijke commit blijft in de geschiedenis staan. Controleer het
   bestand en gebruik **Push origin** als je de terugdraaiing ook op GitHub wilt.

Deze actie draait alle wijzigingen in die ene commit terug, niet zomaar één
bestand. Bij latere wijzigingen aan dezelfde regels kan een conflict ontstaan;
[vraag dan hulp aan de documentatie](https://docs.github.com/en/desktop/managing-commits/reverting-a-commit-in-github-desktop)
of aan AI en controleer het resultaat zelf.

## Verder leren

De [oefening van GitHub Desktop](https://docs.github.com/en/desktop/overview/creating-your-first-repository-using-github-desktop)
toont dezelfde basisstappen met afbeeldingen. Wil je later samenwerken of
verschillende versies naast elkaar ontwikkelen, lees dan over
[branches](https://docs.github.com/en/get-started/using-github/github-flow) en
[pull requests](https://docs.github.com/en/pull-requests/collaborating-with-pull-requests/proposing-changes-to-your-work-with-pull-requests/about-pull-requests).
