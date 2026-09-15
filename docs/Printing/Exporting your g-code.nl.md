# Uw G-code exporteren

Zodra u tevreden bent met hoe het model is gesliced, kunt u de G-code printinstructies exporteren rechtsonder in de applicatie.

!!! note

    Om de exportoptie beschikbaar te hebben, moet u aan twee voorwaarden voldoen

    - uw model moet gesliced zijn
    - u moet zich in de voorbeeldmodus van de applicatie bevinden

Bij het exporteren naar de schijf opent de applicatie een bestandsverkenner die native is aan uw besturingssysteem, waar u een locatie op uw computer kunt selecteren waar de G-code wordt geëxporteerd.

<figure markdown="span">
  ![Welkomstpagina's](../Images/printing/export.gif){ width="900" }
<figcaption>Een map selecteren waar de applicatie de gcode zal exporteren. G-code-bestanden worden opgeslagen met de extensie .gcode<figcaption>
</figure>

??? question "Kan ik G-code direct opslaan op een SD-kaart of USB-stick?"

    Ja. Plaats uw SD-kaart of USB-stick, gebruik vervolgens **Save to Disk** en selecteer de verwisselbare schijf als doelmap.

??? question "Mijn printer is via USB aangesloten — kan ik printen zonder eerst G-code te exporteren?"

    Als uw printer USB-printen ondersteunt, kunt u op **Print via USB** klikken in plaats van te exporteren. Hierdoor wordt de G-code rechtstreeks naar de printer gestreamd zonder een bestand op te slaan.

??? question "Hoe controleer ik de geschatte printtijd en het materiaalverbruik voordat ik exporteer?"

    Deze informatie wordt weergegeven in het paneel rechtsonder na het slicen, direct boven de knop **Save to Disk**. Het toont de geschatte printtijd en het filamentverbruik, zowel in lengte als in gewicht.

??? question "Kan ik G-code exporteren voor een printer die niet op mijn computer is aangesloten?"

    Ja. Zolang het juiste printerprofiel in Cura is geselecteerd, kunt u het G-code-bestand exporteren en handmatig via een SD-kaart of USB-stick naar de printer overzetten.

??? question "Waarom kan ik de knop Save to Disk niet vinden?"

    Zorg ervoor dat uw model eerst is gesliced (klik op **Slice**). De knop **Save to Disk** verschijnt pas nadat het slicen is voltooid.

??? question "Kan ik het geëxporteerde G-code-bestand hernoemen?"

    Ja. Wanneer het opslagvenster verschijnt na het klikken op **Save to Disk**, kunt u de bestandsnaam bewerken voordat u de exportlocatie bevestigt.
