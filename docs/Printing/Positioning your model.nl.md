# Het model voorbereiden

Deze pagina begeleidt u door het printproces en hoe u uw 3D-model kunt omzetten naar instructies die de printer kan begrijpen, zoals hieronder beschreven.

Dit proces wordt slicen genoemd en deze instructies worden `G-Code` genoemd.

## Een model importeren

Als eerste is het vereist dat u het 3D-model heeft dat u wilt printen. Dit 3D-model kan worden gemaakt in 3D-modelleersoftware zoals [Blender](https://www.blender.org/), [Maya](https://www.autodesk.com/products/maya/overview) of [AutoCad](https://www.autodesk.com/eu/products/autocad/overview).

Om uw model te importeren moet u het eerst op uw computer terugvinden. Dit kan door op het mapicoon te drukken in het linkerbovendeel van uw scherm, direct naast de naam van de printer.

<figure markdown="span">
  ![Welkomstpagina's](../Images/printing/open-file.png){ width="600" }
  
<figcaption>Bestandsverkenner openen</figcaption>
</figure>

Hierdoor wordt een bestandsverkenner geopend die native is aan uw besturingssysteem. Gebruik deze om naar de map te navigeren waarin uw model is opgeslagen. Dubbelklik op het bestand of selecteer de optie `Open` in uw bestandsverkenner.

!!! Note

    Het wordt aanbevolen om `.stl`-modellen te gebruiken, aangezien deze het meest geschikt zijn voor het sliceproces en dus voor 3D-printen. U kunt ook alternatieven zoals `.gltf` of `.fbx` gebruiken, maar de kwaliteit kan variëren.

<figure markdown="span">
  ![Welkomstpagina's](../Images/printing/import-file.png){ width="600" }
  
<figcaption>Bestand importeren</figcaption>
</figure>

De applicatie zal vervolgens uw verzoek verwerken en het importeren in de editor.

<figure markdown="span">
  ![Welkomstpagina's](../Images/printing/imported-model.png){ width="600" }
  
<figcaption>Bestand importeren</figcaption>
</figure>

## Model positioneren

Het kan gebeuren dat het model dat u heeft geïmporteerd buiten de printmat verschijnt. U kunt de positie, rotatie en schaal van het model eenvoudig aanpassen via de ingebouwde bedieningselementen in de applicatie.

!!! Danger

    Onthoud dat hoe u uw model op de printmat ziet, is hoe het geprint gaat worden! Het is daarom belangrijk om te zorgen voor de juiste oriëntatie en positie van het model.

Om de positioneermodus te openen, beweegt u de cursor met uw muis over het model en drukt u op de **linker** muisknop. Hierdoor worden de randen van het model gemarkeerd en verschijnen er 3 pijlen.

Deze pijlen kunnen worden gebruikt om het model op de printmat te positioneren.

!!! Tip

    Deze pijlen hebben een naam; vanaf nu noemen we ze de `translatie-gizmo` of gewoon `gizmo`.

U kunt bepalen welke bewerking de gizmo's uitvoeren door er één te kiezen in het linkerpaneel dat op uw scherm is verschenen.

<figure markdown="span">
  ![Welkomstpagina's](../Images/printing/operations.png){ width="600" }
  
<figcaption>Gebruik uw muis om het model op de printmat te positioneren</figcaption>
</figure>

De bewerkingen staan in de volgende volgorde

- positie
- schaal
- rotatie

We gaan bekijken hoe elk van deze gebruikt moet worden.

!!! Note

    Er zijn ook andere bewerkingen, maar hier concentreren we ons op de meest basale. U bent vrij om andere bewerkingen zelf te verkennen.
    TODO: schrijf een pagina over andere bewerkingen en verwijs gebruikers daarnaartoe

### De positie van het model wijzigen

Om de positie van het model te wijzigen, beweegt u met uw muis over de pijl die naar de richting wijst waarin u het model wilt verplaatsen, **houdt** u de **linker** muisknop **ingedrukt** en sleept u uw muis langs de pijl.

<figure markdown="span">
  ![Welkomstpagina's](../Images/printing/positioning.gif){ width="600" }
  
<figcaption>Verschillende bedieningsopties in de applicatie</figcaption>
</figure>

### De rotatie van het model wijzigen

Om de rotatie van het model te wijzigen, selecteert u de rotatiebewerking in de linkerbalk

<figure markdown="span">
  ![Welkomstpagina's](../Images/printing/rotation.png){ width="600" }
  
<figcaption>Met uw muis kunt u de rotatie van het model regelen langs de 3 assen (X, Y, Z)</figcaption>
</figure>

Op vergelijkbare wijze als bij het positioneren kunt u de rotatie uitvoeren. Beweeg hiervoor uw muiscursor over de gizmo die u wilt manipuleren, **houd** uw **linker** muisknop **ingedrukt** en sleep de muis in de richting waarin uw model zich zou moeten bewegen.

<figure markdown="span">
  ![Welkomstpagina's](../Images/printing/rotation.gif){ width="600" }
  
<figcaption>Demonstratie van hoe het model geroteerd kan worden</figcaption>
</figure>

### De schaal van het model wijzigen

Als u uw model groter/kleiner wilt maken, kunt u dit doen met de schaalbewerking.

Gebruik uw linkerbalk om de schaalbewerking te selecteren.

<figure markdown="span">
  ![Welkomstpagina's](../Images/printing/scaling.png){ width="600" }
  
<figcaption>Met uw muis kunt u de rotatie van het model regelen langs de 3 assen (X, Y, Z)</figcaption>
</figure>

Schalen werkt een beetje anders dan de vorige bewerkingen, omdat u meestal wilt dat het model uniform schaalt over de 3 assen. Het model in slechts één as schalen kan het vervormen. U bent echter vrij om dit te doen.

Om het model uniform te schalen, moet u de witte kubus manipuleren waaruit alle andere assen ontstaan.

<figure markdown="span">
  ![Welkomstpagina's](../Images/printing/scaling.gif){ width="600" }
  
<figcaption>Gebruik uw muis om de centrale witte kubus te selecteren en te slepen. Als u langs de negatieve Y-as (omlaag) sleept, wordt het model kleiner; als u langs de positieve Y-as (omhoog) sleept, wordt het model groter<figcaption>
</figure>

---

### FAQ

??? question "Ik kan mijn model niet verplaatsen"

    Waarschijnlijk is uw model tijdens het proces gedeselecteerd. Klik op het model om het opnieuw te selecteren.

??? question "Mijn model heeft een tijgerpatroon"

    Uw model is te groot; gebruik de schaalbewerking om het kleiner te maken.

??? question "Mijn model bevindt zich buiten de printmat"

    Gebruik de pijlen om het binnen de printmat te verplaatsen.

??? question "Ik heb mijn model gepositioneerd waar ik het niet wil hebben"

    Geen probleem, gebruik `Ctrl` + `Z` om de Ongedaan maken-actie uit te voeren, waarmee uw wijzigingen worden teruggedraaid. Als u de terugdraaiing ongedaan wilt maken, gebruik dan `Ctrl` + `Y`.
