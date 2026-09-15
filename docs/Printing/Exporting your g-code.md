# Exporting your G-code

Once your are happy with how the model is being sliced you can export the G-code printer instructions on the bottom right of the application.

!!! note

    In order to have and export option avaialable you have to fullfill two conditions

    - your model must be sliced
    - you must be in the preview mode of the application

When exporting to the disk, application will open file browser native to your operating system where you can select a location on your computer where the g-code will be exported.

<figure markdown="span">
  ![Welcome pages](../Images/printing/export.gif){ width="900" }
<figcaption>Selecting a folder where the applicaiton will export hte gcode. G-code files are saved with .gcode extension <figcaption>
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
