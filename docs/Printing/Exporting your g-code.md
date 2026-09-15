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

??? question "How do I export my sliced model as G-code?"

    Once slicing is complete, click the **Save to Disk** button (or **File → Export**) in the bottom-right corner, choose your destination, and save the file with a `.gcode` extension.

??? question "Can I save G-code directly to an SD card or USB drive?"

    Yes. Insert your SD card or USB drive, then use **Save to Disk** and select the removable drive as the destination folder.

??? question "My printer is connected via USB — can I print without exporting G-code first?"

    If your printer supports USB printing, you can click **Print via USB** instead of exporting. This streams the G-code directly to the printer without saving a file.

??? question "How do I check the estimated print time and material usage before exporting?"

    This information is displayed in the bottom-right panel after slicing, right above the **Save to Disk** button. It shows estimated print time and filament usage in both length and weight.

??? question "Can I export G-code for a printer that isn't connected to my computer?"

    Yes. As long as the correct printer profile is selected in Cura, you can export the G-code file and transfer it manually via SD card or USB drive to the printer.

??? question "Why can't I find the Save to Disk button?"

    Make sure your model has been sliced first (click **Slice**). The **Save to Disk** button only appears after slicing is complete.

??? question "Can I rename the exported G-code file?"

    Yes. When the save dialog opens after clicking **Save to Disk**, you can edit the file name before confirming the export location.
