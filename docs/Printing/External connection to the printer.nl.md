# Externe verbinding met de printer

De applicatie ondersteunt verbinding met de printer. Dit betekent dat u deze applicatie kunt gebruiken om gesliced G-code rechtstreeks naar de printer te sturen en het printen te starten. Precies zoals u dat normaal zou doen met klassieke 2D-printers en documenten.

Om het verbindingsproces te starten, moet u het printermenu openen linksboven in het venster.

## Wat is Repetier

Repetier is een programma waarmee u uw 3D-printer vanaf uw computer kunt bedienen. Dit betekent dat u prints kunt starten, de voortgang kunt bekijken en instellingen zoals temperatuur in realtime kunt aanpassen.

Dit is de reden waarom we het gebruiken: het is vooraf geïnstalleerd op al onze 3D-printers, dus zolang de printer verbonden is met het internet, zou u er via deze applicatie verbinding mee moeten kunnen maken.

!!! Warning

    Het is zeer, zeer belangrijk dat zowel de computer waarmee u verbinding maakt als de printer zelf verbonden zijn met hetzelfde netwerk. Met andere woorden, beide moeten verbonden zijn met dezelfde wifi/router.

## Een verbinding tot stand brengen

<figure markdown="span">
  ![Welkomstpagina's](../Images/printing/connections/open-printer-menu.png){ width="900" }
<figcaption>Klik op het printermenu linksboven in de applicatie.<figcaption>
</figure>

Selecteer vervolgens `Manage printers`

<figure markdown="span">
  ![Welkomstpagina's](../Images/printing/connections/manage-printers.png){ width="900" }
<figcaption>Selecteer de optie manage printers<figcaption>
</figure>

U ziet een venster met verschillende instellingen. En nog belangrijker, alle printers die u in de applicatie heeft geïmporteerd.

<figure markdown="span">
  ![Welkomstpagina's](../Images/printing/connections/connect-repetier-with-arrow.png){ width="900" }
<figcaption>Pop-up met alle opties voor de printers<figcaption>
</figure>

!!! warning

    U ziet deze optie alleen bij de printer die momenteel als primair is ingesteld. Dat wil zeggen, u ziet deze linksboven in het viewportmenu, direct rechts van de kleine mapknop.

Klik in deze pop-up op `Connect repetier`. Hierdoor wordt een andere pop-up geopend die u een overzicht toont van alle tot stand gebrachte verbindingen. Klik vervolgens op `Add`.

<figure markdown="span">
  ![Welkomstpagina's](../Images/printing/connections/add-connection.png){ width="900" }
<figcaption>Selecteer de optie manage printers<figcaption>
</figure>

Wat nu volgt is een behoorlijk verwarrende en intimiderende pop-up. Daarom nemen we het rustig stap voor stap door.

<figure markdown="span">
  ![Welkomstpagina's](../Images/printing/connections/making-connection-pop-up.png){ width="900" }
<figcaption>Selecteer de optie manage printers<figcaption>
</figure>

### De gegevens invullen

**Connection name**

Dit is de naam die u aan deze verbinding wilt geven. Het maakt niet uit welke naam u kiest.

---

**IP address or host name**

Onder welk IP-adres is uw printer vindbaar op het huidige netwerk?

Vul het IP-adres in dat wordt weergegeven op het netwerktabblad van uw printer.

---

**Port**

Aangezien er meerdere apparaten met de printer verbonden kunnen zijn, moeten we hier onderscheid tussen maken; dat is het poortnummer.

Dit zou `3344` moeten zijn, maar controleer dit op het netwerktabblad van uw printer-GUI.

---

**Path**

Laat dit op de standaardinstelling staan.

---

**Show security settings**

Dat hebben we niet nodig.

---

### Printers zoeken

Als alles is ingevuld, druk dan op de knop links met de tekst `Get printers`. Als er niets gebeurt, druk er dan na een paar seconden nogmaals op.

Hiermee wordt gecontroleerd of er printers beschikbaar zijn op de server die u heeft opgegeven.

Als alles gelukt is, zou u een naam van de printer moeten zien verschijnen in het kleine keuzevak rechts van de knop `Get printers`. Druk vervolgens op `Ok`.

<figure markdown="span">
  ![Welkomstpagina's](../Images/printing/connections/get-printers.gif){ width="900" }
<figcaption>Printers ophalen<figcaption>
</figure>

### De API-key ophalen

Nu zou uw printer aan de linkerlijst moeten zijn toegevoegd.

<figure markdown="span">
  ![Welkomstpagina's](../Images/printing/connections/printer-in-the-list.png){ width="900" }
<figcaption>Verbinding tot stand brengen met de repetier-server<figcaption>
</figure>

De volgende stap is het ophalen van de API-key van de repetier-server.

Klik hiervoor op de printer die u zojuist heeft toegevoegd in de linkerlijst, en onderaan de pop-up zou een knop moeten staan met de tekst `Open in browser...`. Klik hierop.

<figure markdown="span">
  ![Welkomstpagina's](../Images/printing/connections/open-in-browser.gif){ width="900" }
<figcaption>Repetier openen in de browser<figcaption>
</figure>

!!! NOTE

    De video toont de API-key al ingevuld; dit komt doordat de applicatie deze onthoudt. Bij u zou hier echter niets ingevuld moeten staan. Als dit wel het geval is, volg dan hoe dan ook onderstaande stappen.

U wordt doorgestuurd naar de website van de repetier-server. Het valt helaas buiten het bestek van deze documentatie om hier dieper op in te gaan, dus lees gerust meer op [deze pagina](https://www.repetier-server.com/manuals/1.4/index.html).

Om nu de API-key op te halen, klikt u op het tandwielicoon rechtsboven op de pagina en selecteert u `Global settings`

<figure markdown="span">
  ![Welkomstpagina's](../Images/printing/connections/global-settings.png){ width="900" }
<figcaption>De globale instellingen openen<figcaption>
</figure>

De API-key is te vinden onder de sectie **Connectivity**, in de paragraaf met de naam API Key.

Voor het gemak kunt u de kleine blauwe knop rechts van de API-key gebruiken om deze naar uw klembord te kopiëren. U kunt ook de API-key markeren en op `CTRL+C` drukken.

<figure markdown="span">
  ![Welkomstpagina's](../Images/printing/connections/api-key-location.png){ width="900" }
<figcaption>De API-key vinden onder Connectivity -> API key<figcaption>
</figure>

Nu kunt u terugkeren en de API-key die u zojuist heeft verkregen, plakken in het invoerveld met de naam `API Key`.

Zodra de API-key is ingevuld, zou de knop `Connect to printer` niet langer grijs moeten zijn en kunt u erop klikken. Als alles goed is gegaan, zou onderaan het scherm een pop-up moeten verschijnen die aangeeft dat de verbinding tot stand is gebracht.

<figure markdown="span">
  ![Welkomstpagina's](../Images/printing/connections/connected.gif){ width="900" }
<figcaption>Verbinding tot stand brengen door op connect te drukken<figcaption>
</figure>

Na deze stap kunt u beide pop-ups sluiten en verdergaan met uw werk.

Om op elk moment te controleren of een printer verbonden is, kunt u de printerstatus linksboven controleren. Als de printer verbonden is, ziet u een klein blauw rondje naast het pictogram van de printer.

<figure markdown="span">
  ![Welkomstpagina's](../Images/printing/connections/printer-status.png){ width="700" }
</figure>

---

### Veelgestelde vragen

??? question "Ik zie de optie 'Connect Repetier' niet in de printerinstellingen"

    Deze optie verschijnt alleen bij de printer die momenteel als primair is ingesteld — degene die linksboven in het viewportmenu wordt weergegeven, direct naast de kleine mapknop. Zorg er eerst voor dat de juiste printer als primair is geselecteerd. Als de optie nog steeds niet verschijnt, kan dit een ongebruikelijk probleem zijn — stuur een bugreport via het menu rechtsboven in de applicatie.

??? question "Ik kan geen verbinding maken met mijn printer, ook al heb ik het IP-adres en de poort ingevuld"

    Controleer of zowel uw computer als de printer verbonden zijn met **hetzelfde netwerk** (dezelfde WiFi/router). Controleer ook of het IP-adres en poortnummer exact overeenkomen met wat wordt weergegeven op het netwerktabblad van uw printer. Als alles klopt en het lukt nog steeds niet, is dit mogelijk geen veelvoorkomend probleem — stuur een bugreport via het menu rechtsboven.

??? question "Er gebeurt niets wanneer ik op 'Get printers' klik"

    Wacht een paar seconden en druk er opnieuw op — soms heeft de server even nodig om te reageren. Als herhaalde pogingen geen printers opleveren, is dit waarschijnlijk geen veelvoorkomend probleem, dus stuur een bugreport via het menu rechtsboven in de applicatie.

??? question "Er verschijnt geen printernaam in het keuzevak na het zoeken"

    Dit betekent meestal dat de verbindingsgegevens (IP, poort) onjuist zijn, of dat de printer niet bereikbaar is op het netwerk. Controleer de gegevens opnieuw op het netwerktabblad van uw printer. Als de gegevens correct zijn en de printer nog steeds niet verschijnt, meld dit dan als bug via het menu rechtsboven.

??? question "De knop 'Connect to printer' blijft grijs"

    Dit betekent dat het API-keyveld leeg is. Zorg ervoor dat u de API-key van de Repetier-server heeft gekopieerd vanuit Global Settings onder **Connectivity** en deze heeft geplakt in het API Key-veld. Als de knop grijs blijft, zelfs na het plakken van een geldige sleutel, is dit waarschijnlijk geen veelvoorkomend probleem — stuur een bugreport via het menu rechtsboven.

??? question "Ik zie geen bevestigingspop-up na het klikken op Connect to printer"

    Normaal gesproken verschijnt er een pop-up onderaan het scherm die de verbinding bevestigt. Als er niets verschijnt, wacht dan een paar seconden en controleer het printerstatuspictogram linksboven. Als er geen blauw rondje naast het printerpictogram staat en er ook geen foutmelding is, is dit ongebruikelijk — stuur een bugreport via het menu rechtsboven.

??? question "Het printerstatuspictogram toont geen blauw rondje, ook al heb ik alle stappen voltooid"

    Een blauw rondje naast het printerpictogram betekent dat er verbinding is. Als dit ontbreekt nadat u alle stappen correct heeft gevolgd, probeer dan het verbindingsproces opnieuw vanuit **Manage Printers**. Als het nog steeds niet werkt, is dit waarschijnlijk geen veelvoorkomend probleem — stuur een bugreport via het menu rechtsboven.

??? question "Ik heb al een API-key ingevuld staan, maar ik heb er zelf nooit een ingevoerd"

    Dit is normaal — de applicatie onthoudt eerder gebruikte API-keys. Volg dezelfde stappen als gebruikelijk om de juiste sleutel op te halen en opnieuw in te voeren. Als dit onverwacht gedrag veroorzaakt, meld dit dan als bug via het menu rechtsboven.

??? question "Wat moet ik doen als geen van de probleemoplossingsstappen mijn verbindingsprobleem oplost?"

    Als uw probleem niet wordt opgelost door de gebruikelijke oplossingen, stuur dan een bugreport via het menu rechtsboven in de applicatie, zodat het verder onderzocht kan worden.
