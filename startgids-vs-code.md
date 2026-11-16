# Aan de slag met VS Code

Met Visual Studio Code, meestal **VS Code** genoemd, kun je tekstbestanden in
een map bekijken en bewerken. Dat is handig als je bijvoorbeeld samen met AI
lesmateriaal maakt: je ziet welke bestanden er zijn en kunt ze zelf aanpassen.
Je hoeft niet te kunnen programmeren.

In deze oefening bekijk en bewerk je een bestaand bestand in Markdown. Markdown
is gewone tekst met eenvoudige tekens voor opmaak, zoals `#` voor een titel.

## Installeer VS Code

1. Ga naar de [website van VS Code](https://code.visualstudio.com/) en download
   de versie voor je computer.
2. Open het gedownloade installatiebestand en volg de aanwijzingen. Op een
   beheerde werkcomputer kan de installatie afhangen van de instellingen van je
   organisatie. Vraag hulp aan de ICT-dienst als installeren niet lukt.
3. Start VS Code. De voorbeelden hieronder gebruiken de Engelse menunamen; als
   je een andere taal hebt ingesteld, kunnen de namen verschillen.

## Open een map

1. Maak eerst op je computer een map, bijvoorbeeld `vs-code-oefening`. Kopieer
   [writing-style.md](writing-style.md) uit deze repository naar die map. Heb je
   de repository nog niet op je computer? Open de link, kies op GitHub **Download
   raw file** en bewaar het bestand in je oefenmap.
2. Kies in VS Code **File → Open Folder**, selecteer de map en open ze.
3. Krijg je de vraag of je de auteurs van de bestanden vertrouwt? Bij je eigen
   oefenmap kun je die bevestigen. Kies bij een onbekende map voor de beperkte
   modus totdat je weet wat erin staat. Meer uitleg vind je bij
   [Workspace Trust](https://code.visualstudio.com/docs/editing/workspaces/workspace-trust).

Links zie je de **Explorer**, de verkenner met de bestanden en eventuele
submappen. Zie je die niet, klik dan op het pictogram **Explorer** linksboven.
Klik op een bestand om het rechts in de editor te openen. Boven de editor staan
tabbladen waarmee je tussen geopende bestanden wisselt. De bestanden blijven in
de map op je computer staan; VS Code toont en bewerkt ze daar.

## Bewerk en bewaar een bestand

1. Klik in de Explorer op `writing-style.md`. Dit bestand bevat afspraken over
   de schrijfstijl voor het workshopmateriaal. De uitgang `.md` geeft aan dat
   het een Markdown-bestand is.
2. Voeg onderaan een eigen zin toe, bijvoorbeeld:

   ```text
   Deze zin heb ik zelf toegevoegd.
   ```

3. Kies **File → Save** of druk op **Ctrl+S** (Windows) / **Cmd+S** (Mac). Een
   bolletje op het tabblad geeft aan dat er nog niet-bewaarde wijzigingen zijn.
   Pas de tekst aan en bewaar opnieuw.

Sluit het tabblad met het kruisje en open `writing-style.md` opnieuw via de
Explorer. Je ziet de bewaarde tekst terug. Je bewerkt alleen de kopie in je
oefenmap.

Wil je zelf een bestand maken? Beweeg in de Explorer over de naam van je map,
klik op **New File**, het pictogram van een bestand met een plusteken, en geef
het bestand een naam, bijvoorbeeld `notities.md`.

## Bekijk de opmaak

VS Code kan Markdown meteen als opgemaakte tekst tonen:

1. Open `writing-style.md` en kies rechtsboven in de editor **Open Preview to the
   Side**. Je kunt ook **Ctrl+K**, gevolgd door **V** gebruiken op Windows, of
   **Cmd+K**, gevolgd door **V** op Mac.
2. Je ziet de Markdown-tekst en de voorvertoning naast elkaar. Verander een
   titel of voeg een lijstpunt toe en kijk wat er gebeurt.
3. Bewaar je wijziging. Sluit de voorvertoning met het kruisje op het tabblad.

De voorvertoning is ingebouwd in VS Code; daarvoor heb je geen extensie nodig.
Meer voorbeelden vind je in de
[Markdown-documentatie van VS Code](https://code.visualstudio.com/docs/languages/markdown).

## Installeer Markdown All in One

Een **extensie** voegt functies toe aan VS Code. Markdown All in One helpt onder
meer bij het bewerken van lijsten en het maken van een inhoudsopgave.

1. Klik links op **Extensions**, het pictogram met vier blokjes.
2. Zoek naar `Markdown All in One`.
3. Kies **Markdown All in One** van **Yu Zhang**. Controleer eventueel de
   [pagina van de extensie](https://marketplace.visualstudio.com/items?itemName=yzhang.markdown-all-in-one)
   om zeker te zijn dat je de juiste kiest.
4. Klik op **Install**. Als de installatie voltooid is, verschijnt de extensie
   bij je geïnstalleerde extensies. Op een beheerde computer kunnen instellingen
   van je organisatie de installatie beperken.
5. Open `writing-style.md`, zet de cursor aan het einde van een lijstpunt en druk op
   Enter. De extensie helpt je om het volgende lijstpunt te maken. Bewaar het
   bestand als je de wijziging wilt houden.

Via **Extensions** kun je de extensie later ook uitschakelen of verwijderen. De
pagina van de extensie beschrijft de andere functies en sneltoetsen.

## Zoek en volg je bestanden

Zoek je een woord in het open bestand? Gebruik **Ctrl+F** (Windows) of **Cmd+F**
(Mac). Wil je in de map zoeken, klik dan links op **Search**, het vergrootglas,
en typ je zoekterm. Klik op een resultaat om het bestand op die plaats te
openen.

Laat je Work met dezelfde map werken? Open de map ook in VS Code en bekijk de
bestanden die Work maakt of aanpast via de Explorer. Open ze en lees de inhoud;
de voorvertoning helpt om Markdown te bekijken. Bewaar je eigen wijzigingen
voordat AI aan hetzelfde bestand werkt, zodat je niet met twee versies tegelijk
bezig bent. Controleer het volledige resultaat zelf.

## Verder leren

In de
[introductie van VS Code](https://code.visualstudio.com/docs/getstarted/overview)
vind je meer uitleg over de installatie en de onderdelen van het programma.

Wil je afspraken en werkwijzen hergebruiken? Ga verder met de
[gids over herbruikbare instructies, skills en agents](herbruikbare-instructies-skills-en-agents.md).
