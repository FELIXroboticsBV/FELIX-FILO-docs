# Slicen

Zodra u tevreden bent met hoe uw model is gepositioneerd, kunnen we doorgaan naar de volgende stap: slicen.

Slicen is een procedure die het model omzet in instructies die uw 3D-printer kan begrijpen en uitvoeren. Deze instructies zijn eenvoudige commando's zoals

- verplaats 30 mm langs de x-as
- verplaats 20 mm langs de y-as en breng 0,2 mm filament aan

Om het model te slicen hoeft u alleen maar op slice te drukken, rechtsonder in het venster.

<figure markdown="span">
  ![Welkomstpagina's](../Images/printing/slicing-button.png){ width="600" }
  
<figcaption>Slice-knop rechtsonder</figcaption>
</figure>

Afhankelijk van hoe krachtig uw computer is of hoe groot/gedetailleerd uw model is, kan dit proces enige tijd duren. In extreme gevallen gaat het om uren.

!!! success

    De applicatie zal het slicen niet toestaan als er iets ernstig mis is met uw model. Dit voorkomt dat er schadelijke prints op de printer worden uitgevoerd.

!!! tip

    Als u opnieuw wilt slicen, verplaats het model dan een klein beetje; dit dwingt de applicatie om het model opnieuw te slicen.

## Voorbeeldweergave

Zodra het slicen is voltooid, kunt u een voorbeeld bekijken van de G-code die door de slicer is gegenereerd.

Om dit te doen, moet u schakelen naar een andere modus waarin de applicatie zich momenteel bevindt. Het wisselen van modus doet u door de knoppen in het midden bovenaan uw scherm te selecteren.

<figure markdown="span">
  ![Welkomstpagina's](../Images/printing/preview-mode.png){ width="600" }
  
<figcaption>De voorbeeldmodus bevindt zich in het bovenmenu, in het midden.</figcaption>
</figure>

In de voorbeeldmodus blijft het model aanwezig, maar wordt het weergegeven als een reeks lijnen die overeenkomen met waar de printer naartoe zal gaan.

Het is mogelijk dat u een vreemd object op uw model ziet verschijnen. Hier hoeft u zich geen zorgen over te maken; dit is een ondersteunende structuur die ervoor zorgt dat uw 3D-print niet instort of breekt. Nadat het printen is voltooid, zijn de ondersteunende structuren ontworpen om gemakkelijk te worden verwijderd.

### De voorbeeldweergave gebruiken

3D-printers die worden gebruikt voor het printen van modellen/vormen werken op basis van lagen. De printer begint niet aan een laag totdat de vorige is voltooid. Dit kan worden gevisualiseerd met de schuifregelaar rechts in de voorbeeldmodus. U kunt deze omhoog of omlaag aanpassen, afhankelijk van hoeveel lagen op dat moment zichtbaar moeten zijn.

!!! note

    In tegenstelling tot in de applicatie, begint de printer zijn taak altijd bij laag 0 en werkt hij omhoog in de laagstapel.

<figure markdown="span">
  ![Welkomstpagina's](../Images/printing/layer-preview.gif){ width="600" }
  
<figcaption>Gebruik de schuifregelaar rechts om afzonderlijke lagen te bekijken.</figcaption>
</figure>

U kunt ook een voorbeeld bekijken van hoe de nozzle van de printer zich op deze laag zal bewegen. Dit kan door met de **linkerknop** op het kleine afspeelknopje onderaan het scherm te drukken.

Hierdoor ziet u een virtuele nozzle die materiaal "aanbrengt". Op deze manier kunt u de integriteit van uw prints controleren als u niet zeker weet waarom deze mislukken.

<figure markdown="span">
  ![Welkomstpagina's](../Images/printing/print-preview.gif){ width="600" }
  
<figcaption>De schuifregelaar onderaan geeft aan hoeveel werk de printer nog moet verrichten voordat de geselecteerde laag klaar is</figcaption>
</figure>

??? question "Mijn model valt door het platform heen / zweeft erboven"

    Gebruik de optie **Drop to Buildplate** (rechtsklik op het model → *Drop to Buildplate*) om het automatisch gelijk met het platform te laten aansluiten.

??? question "Mijn print heeft een slechte hechting van de eerste laag"

    Probeer een **Skirt** of **Brim** in te schakelen onder *Build Plate Adhesion*-instellingen. Een Brim voegt extra oppervlak toe rond de basis van uw model, wat helpt om het beter te laten hechten.

??? question "Mijn model is te groot voor het bouwvolume"

    Gebruik het gereedschap **Scale** (`S`) om uw model te verkleinen, of klik met de rechtermuisknop erop en selecteer *Scale to Max* als u wilt dat het automatisch op het platform past.

??? question "Ik wil meerdere kopieën van hetzelfde model printen"

    Klik met de rechtermuisknop op het model en selecteer **Multiply Model**, voer vervolgens het gewenste aantal kopieën in. FELIX-FILO zal deze automatisch op het platform rangschikken.

??? question "Mijn overhangende delen hangen door of zakken in"

    Schakel **Support Structures** in onder de *Support*-instellingen. U kunt ook de *Support Overhang Angle* aanpassen om te bepalen wanneer er supports worden gegenereerd.

??? question "Ik heb per ongeluk een model van het platform verwijderd"

    Gebruik `Ctrl` + `Z` om de verwijdering ongedaan te maken, net als bij elke andere actie in FELIX-FILO.

??? question "Mijn model is niet geroteerd zoals ik wil"

    Gebruik het gereedschap **Rotate** (`R`) om de oriëntatie handmatig aan te passen, of klik met de rechtermuisknop op het model en kies *Reset Rotation* om het terug te zetten naar de standaardoriëntatie.
