# PatternMaker
simple HTML and JavaScript app for making bead patterns.

## Pärlplattemönster

Öppna `index.html` direkt i webbläsaren (ingen server behövs).

1. Välj en JPEG-bild.
2. Ange rastrets storlek N × M (pärlor) och antal färger.
   Öka vid behov **Kontrastförstärkning** (0–200 %) för bilder som blir för platta.
3. Klicka **Generera mönster** och sedan **Ladda ner PNG**.

Bilden medelvärdesbildas per ruta, kontrasten förstärks (färgerna sträcks ut kring
bildens medelljushet) och färgerna reduceras med k-means i CIELAB-färgrymd.
PNG:en innehåller pärlor med symboler, rad-/kolumnnummer, stödlinjer var 10:e pärla
och en färgförklaring med antal pärlor per färg.
