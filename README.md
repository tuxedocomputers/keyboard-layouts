# TUXEDO Keyboards

*For English steps please check below!*

## 🇩🇪 Individuelle Tastaturen für dein TUXEDO Notebook

[![Watch the video](/video-laser.jpg?raw=true)](https://youtu.be/6wrwNaS5dw4)

Im Sinne von Open Source stellen wir produktionsreife Vorlagen für gelaserte Tastaturen zur Verfügung. Wir möchten damit allen Enthusiasten die Möglichkeit geben, ihr eigenes Tastaturlayout zu erstellen und dieses dann auf ihrem Linux-Notebooks von TUXEDO gelasert zu bekommen. Sollte Ihr Layout auch für andere Kunden relevant sein, beispielsweise bei neuen Sprachvarianten, ist das Ganze sogar kostenlos. Denn von zusätzlichen Speziallayouts profitiert wiederum die gesamte Community!

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
      - Die Schriftart kann von [Google Fonts](https://fonts.google.com/specimen/Rajdhani) heruntergeladen werden.
 4. Änderungen speichern und *committen*. Eine aussagekräftige Beschreibung des commits ("commit message") ist immer gerne gesehen: <br />
    `git commit -m "Neues Layout für Sprache XZY"` 
 5. Alle Arbeiten in deinen Fork auf Github.com schieben: <br />
    `git push --set-upstream origin <NEUER BRANCH>`
 6. Mit einem Pull Request reichst du deine Arbeiten bei uns ein.<br />
 **Wichtig:** Bitte vermerke bei deiner Bestellung im Shop, dass du ein Layout auf Github eingereicht hast! Wir prüfen das Layout und geben es frei, sofern alles passt. <br /><br />
 Ab hier gehen deine Daten in die Produktion und schon bald erhältst du dein TUXEDO Notebook mit **deinem** Tastaturlayout! 🎉
 
 <hr>
 
## 🇺🇸 Custom Keyboards for your TUXEDO laptop

[![Watch the video](/video-laser.jpg?raw=true)](https://youtu.be/6wrwNaS5dw4)

In the spirit of Open Source, we provide production-ready templates for lasered keyboards. We want to give all enthusiasts the possibility to create their own keyboard layout and have it lasered on their Linux notebook by TUXEDO. If your layout is also relevant for other customers, for example for new language variants, the whole service is even free of charge. Because additional special layouts in turn benefit the entire community!

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
