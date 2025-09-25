# TUXEDO Keyboards

*For English steps please check below!*

## 🇩🇪 Individuelle Tastaturen für dein TUXEDO Notebook

[![Watch the video](/video-laser.jpg?raw=true)](https://youtu.be/6wrwNaS5dw4)

Im Sinne von Open Source stellen wir produktionsreife Vorlagen für gelaserte Tastaturen zur Verfügung. Wir möchten damit allen Enthusiasten die Möglichkeit geben, ihr eigenes Tastaturlayout zu erstellen und dieses dann auf ihrem Linux-Notebooks von TUXEDO gelasert zu bekommen. 

Folgende Sprachen existieren bereits:
 * Deutsch (DE-DE)
 * Englisch (US-ISO)
 * Englisch (UK-ISO)
 * Schweiz (DE-CH)
 * Belgisch (BE)
 * Tschechisch (CZ)
 * Dänisch (DK)
 * Estnisch (ET)
 * Französisch (FR)
 * Griechisch (GR)
 * Ungarisch (HU)
 * Italienisch (IT)
 * Norwegisch (NO)
 * Polnisch (PL Programmers)
 * Portugiesisch (PT-PT)
 * Russisch (RU-EN)
 * Slowakisch (SK)
 * Slowenisch / Kroatisch (SL/HR)
 * Spanisch (ES)
 * Schwedisch/Finnisch (SE/FI)
 * Türkisch (TR)

Folgende Layoutvarianten existieren bereits:
 * Dvorak DE-ISO
 * Dvorak US-ISO
   
### Eigenes Layout einreichen
Der Ablauf ist identisch zu den meisten anderen Softwareprojekten auf Github. Zur Sicherheit hier noch einmal alle Schritte im Detail:

 1. Dieses Repository forken, den Fork auf deinen Rechner klonen und danach einen neuen Branch für deine Arbeiten erstellen: <br />
    ```
    git clone https://github.com/<DEIN USERNAME>/keyboard-layouts
    cd keyboard-layouts/
    git checkout -b <NEUER BRANCH>
    ```
 2. Eine Datei kopieren, mit geändertem Sprachkürzel im Dateinamen ablegen und dem Git Index hinzufügen. Zum Beispiel für das InfinityBook S14: <br />
    ```
    cd keyboard-layouts/InfinityBook\ S14/
    cp InfinityBook\ S14\ -\ EN-US.svg InfinityBook\ S14\ -\ <NEUES KUERZEL>.svg
    git add InfinityBook\ S14/InfinityBook\ S14\ -\ <NEUES KUERZEL>.svg
    ```
 3. Bearbeiten der neuen Datei mit einem Vektorgrafikprogramm, vorzugsweise [Inkscape](https://inkscape.org/de/). Bitte hierbei folgende Punkte beachten:
    * Die Ebenen *justify* und *grid* sind gesperrt. Diese auf keinen Fall verändern!
    * Das Gitter ("grid") ist immer für ISO-Layouts angelegt, wird jedoch vom Laser ignoriert. ANSI-Layouts können also problemlos ebenfalls damit erstellt werden!
    * Position der Tastenbeschriftung im Idealfall nicht verändern. Falls doch nötig, bitte nicht zu nahe an den Rand der jeweiligen Taste setzen.
    * Schriftarten nur nach vorheriger Absprache verändern.
      - Die Schriftart für Standardzeichen ist Rajdhani und kann von [Google Fonts](https://fonts.google.com/specimen/Rajdhani) heruntergeladen werden.
      - Die Schriftart für Sonderzeichen heißt Myriad Pro und ist auf [font download](https://font.download/font/myriad-pro) zu finden.
 4. Änderungen speichern und *committen*. Eine aussagekräftige Beschreibung des commits ("commit message") ist immer gerne gesehen: <br />
    `git commit -m "Neues Layout für Sprache XZY"` 
 5. Alle Arbeiten in deinen Fork auf Github.com schieben: <br />
    `git push --set-upstream origin <NEUER BRANCH>`
 6. Mit einem Pull Request reichst du deine Arbeiten bei uns ein.<br />
 **Wichtig:** Bitte vermerke bei deiner Bestellung im Shop, dass du ein Layout auf Github eingereicht hast! Wir prüfen das Layout und geben es frei, sofern alles passt. <br /><br />
 Ab hier gehen deine Daten in die Produktion und schon bald erhältst du dein TUXEDO Notebook mit **deinem** Tastaturlayout! 🎉

#### Präzise Ausrichtung der Beschriftungen

##### Variante 1

* Duplizieren Sie in Inkscape die **PRINT**-Gruppe.
* Sperren Sie die Original-Gruppe und reduzieren Sie deren Deckkraft.
* In der duplizierten Gruppe können Sie dann die Buchstaben nach Bedarf ändern.
* Anschließend können Sie die Original-Gruppe löschen.
  - **Wichtig**: Bitte entfernen oder verändern Sie die **GRID**-Gruppe nicht.

##### Variante 2

* Kopieren Sie das SVG eines bestehendes Layouts
* Erzeugen Sie einen neuen Layer für Ihr eigenes Layout
* Für jede Taste, fügen Sie ein Text-Element mit der ursprünglichen Beschriftung in den neuen Layer ein
  - Setzen Sie die Schriftart auf **Rajdhani**
  - Für die Hauptbeschrichtung ist die Schriftgröße **16 Punkt** und der Stil **fett**
  - Für Zweitbeschriftungen (z.B. Sonderzeichen in der Zahlenreihe, d.h. Shift+Taste) wird Schriftgröße **13 Punkt** und **halbfetter** Stil verwendet
* Richten Sie nun den Text an der ursprünglichen Beschriftung aus:
  - Markieren Sie Ihren Text (zuerst) und (danach) das Pfad-Objekt des ursprünglichen Layouts
  - Im Ausrichtungs-Werkzeug wählen Sie **"ausrichten an letztgewähltem Element"** und richten Sie dann das Text-Element am Pfad horizontal und vertikal aus
  - Nun sollte der Text exakt deckungsgleich mit dem Pfad sein
* Tun Sie dies für alle Tasten
* Ändern Sie nun die Text-Elemente auf die Beschriftung Ihres eigenen Layouts
  - Nach dem Ändern des Textes wird er nicht mehr horizontal mittig auf der Taste ausgerichtet sein
* Richten Sie den Text nochmals an der ursprünglichen Beschriftung aus:
  - Markieren Sie Ihren Text (zuerst) und (danach) das Pfad-Objekt des ursprünglichen Layouts
  - Im Ausrichtungs-Werkzeug wählen Sie **"ausrichten an letztgewähltem Element"** und richten Sie dann das Text-Element am Pfad *horizontal* aus
  - Richten Sie den Text *nicht* vertikal aus!
  - Nun sollte der Text horizontal mittig auf der Taste stehen
* Wandeln Sie die Text-Elemente in Pfade um:
  - Markieren Sie alle Text-Elemente Ihres eigenen Layout-Layers
  - Verwenden Sie den Menupunkt **"Pfad > Objekt zu Pfad konvertieren"** um Texte in Pfade umzuwandeln
* Kopieren Sie die gemeinsamen Pfade (Beschriftungen von Tasten, die Sie nicht angepasst haben) des ursprünglichen Layouts in Ihren eigenen Layout-Layer
* Löschen Sie den Layer mit dem ursprünglichen Layout
  - **Wichtig**: Bitte entfernen oder verändern Sie das **GRID**-Layout nicht

<hr>
 
## 🇺🇸 Custom Keyboards for your TUXEDO laptop

[![Watch the video](/video-laser.jpg?raw=true)](https://youtu.be/6wrwNaS5dw4)

In the spirit of Open Source, we provide production-ready templates for lasered keyboards. We want to give all enthusiasts the possibility to create their own keyboard layout and have it lasered on their Linux notebook by TUXEDO. 

The following languages already exist:
 * German (DE-DE)
 * English (US-ISO)
 * English (UK-ISO)
 * Swiss (DE-CH)
 * Belgian (BE)
 * Czech (CZ)
 * Danish (DK)
 * Estonian (ET)
 * French (FR)
 * Greek (GR)
 * Hungarian (HU)
 * Italian (IT)
 * Norwegian (NO)
 * Polish (PL Programmers)
 * Portugese (PT-PT)
 * Russian (RU-EN)
 * Slovakian (SK)
 * Slovenian / Croatian (SL/HR)
 * Spanish (ES)
 * Swedish/Finnish (SE/FI)
 * Turkish (TR)

The following layout variants already exist:
 * Dvorak DE-ISO
 * Dvorak US-ISO
    
### Submitting your own layout
The process is identical to most other software projects on Github. To be on the safe side here are all steps in detail:

 1. Fork this repository, clone the fork on your machine and then create a new branch for your work: <br />
    ```
    git clone https://github.com/<YOUR USERNAME>/keyboard-layouts
    cd keyboard-layouts/
    git checkout -b <NEW BRANCH>
    ```
 2. Copy a file, save it with a changed language abbreviation in the file name and add it to the Git Index. For example for the InfinityBook S14: <br />
    ```
    cd keyboard-layouts/InfinityBook\ S14/
    cp InfinityBook\ S14\ -\ EN-US.svg InfinityBook\ S14\ -\ <NEW CODE>.svg
    git add InfinityBook\ S14/InfinityBook\ S14\ -\ <NEW CODE>.svg
    ```
 3. Edit the new file with a vector graphics program, preferably [Inkscape](https://inkscape.org/). Please note the following points:
    * The levels *justify* and *grid* are locked. Do not change them under any circumstances!
    * The grid is always created for ISO layouts, but is ignored by the laser. ANSI layouts can therefore also be created with it without any problems!
    * Ideally, do not change the position of the key labeling. If necessary, please do not place it too close to the edge of the respective key.
    * Change fonts only after prior consultation.
      - The font can be downloaded from [Google Fonts](https://fonts.google.com/specimen/Rajdhani).
 4. Save changes and *commit*. A meaningful description of the commit ("commit message") is always welcome: <br />
    `git commit -m "New layout for language XZY"` 
 5. Move all work into your fork on Github.com: <br />
    `git push --set-upstream origin <NEW BRANCH>`
 6. With a Pull Request you submit your work to us. <br />
 **Important:** Please note in your order in the store that you have submitted a layout on Github! We will check the layout and release it if everything fits. <br /><br />
 From here on your data will go into production and soon you will receive your TUXEDO laptop with **your** keyboard layout! 🎉

#### Precise Alignment of Labels

##### Option 1

* Duplicate the **PRINT** group in Inkscape.
* Lock the original group and reduce its opacity.
* In the duplicated group, you can then modify the letters as needed.
* Afterward, you can delete the original group.
  - **Important**: Please do not remove or modify the **GRID** group.

##### Option 2

* Copy the SVG of an existing layout.
* Create a new layer for your own layout.
* For each key, insert a text element with the original label into the new layer:
  - Set the font to **Rajdhani**.
  - For the primary label, use a font size of **16 pt** and a **bold** style.
  - For secondary labels (e.g., special characters in the number row, i.e., Shift+key), use a font size of **13 pt** and a **semi-bold** style.
* Align the text with the original label:
  - Select your text (first) and (afterwards) the path object of the original layout.
  - In the alignment tool, choose **"align to last selected"** and align the text element horizontally and vertically with the path.
  - The text should now be perfectly aligned with the path.
* Repeat this for all keys.
* Change the text elements to the labels of your own layout:
  - After changing the text, it will no longer be horizontally centered on the key.
* Align the text again with the original label:
  - Select your text (first) and (then) the path object of the original layout.
  - In the alignment tool, choose **"align to last selected"** and align the text element *horizontally* with the path.
  - *Do not* align the text vertically!
  - The text should now be horizontally centered on the key.
* Convert the text elements into paths:
  - Select all text elements in your own layout layer.
  - Use the menu option **"Path > Object to Path"** to convert the text into paths.
* Copy the common paths (labels of keys that you have not modified) from the original layout layer into your own layout layer.
* Delete the layer with the original layout.
  - **Important**: Please do not remove or modify the **GRID** layout.
