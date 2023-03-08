# Konfiguration av telemetrisensorer

Följande inställningar kan konfigureras för sensorer:

* **Namn:** Sensorns namn - max fyra tecken.
* **Typ:** Alternativen är **Anpassad** och **Beräknad**. Anpassade sensorer är definierade av hårdvaran. Beräknade sensorer är sensorer vars värden beräknas utifrån andra sensorers värden. Se nedan för mer information om beräknade sensorer.
* **ID:** Detta nummer indikerar vilken typ av sensor det är och består av två delar. Den första delen är sensorns ID, vilket definierar typen av sensor. Den andra delen är ett instansnummer för hårdvaran. Om flera sensorer av samma typ är konfigurerade måste instansnumren vara unika.
* **Enhet:** Sensorns enhet. Enheten används när sensorns värde visas eller läses upp.
* **Precision:** Specificerar antalet decimalsiffror när sensorvärdet visas på skärmen. Värdet trunkeras (klipps) baserat på denna inställning.
* **Skalfaktor:** Specificerar ett värde med vilket sensorns värde multipliceras. Detta kan behöva göras för vissa sensorer.
* **Offset:** Specifiecerar en offset som adderas till sensorns värde.
* **Auto offset:** Om aktiverad, kommer första mottagna värde att användas som offset. Det går att använda [Återställ telemetri](../../reset-telemetry.md) för att återställa offsetvärdet för en redan konfigurerad sensor.
* **Positiv:** When selected, the value of the sensor will be displayed only when it is a positive number. Displays zero when the sensor value becomes a negative number.
* **Filter:** When selected, the sensor value becomes a rolling average of the last 5 received values.
* **Logga:** When selected, the value of this sensor will be saved in the log file. SD Card logging is configured in [Special Functions](../special-functions.md) or Global Functions.

För beräknade sensorer finns därutöver följande möjliga inställningar:

* **Formel:** Typ av beräkning att utföra. Alternativen är:
  * **Addera:** Addera värdena av upp till fyra angivna sensorer.
  * **Medel:** Beräkna medelvärdet av upp till fyra angivna sensorer.
  * **Minimum:** Hitta minsta värdet av upp till fyra angivna sensorer.
  * **Maximum:** Hitta största värdet av upp till fyra angivna sensorer.
  * **Multiplicera:** Multiplicera värdet av två sensorer.
  * **Summera:** Beräkna det kumulativa värdet av en sensor.
  * **Cell:** Detta är formeln för FrSKY Lipo-batterisensor. Den visar spänningen för cellen som angetts i fältet "Cellindex".\
    Om "Lägsta" anges i "Cellindex"-fältet, visas spänningen för cellen med lägst värde.\
    Om "Högsta" anges i "Cellindex"-fältet, visas spänningen för cellen med högst värde.\
    Om "Delta" anges i "Cellindex"-fältet, visas spänningskillnaden mellan högsta och lägsta cell.
  * **Förbrukning:** Beräknar förbrukningen (i mAh) genom att kumulativt summera strömsensorns värde.
  * **Avstånd:** Beräknar avståndet mellan mottagaren och radion genom att använda värden från GPS-sensor och höjdmätare.
* **Källa 1, 2, 3, 4:** De sensorer som tillhandahåller argumenten (värdena) som används i angiven beräkningsformel enligt ovan.
* **Beständig:** När detta valts kommer sensorns värde att bevaras mellan modellbyten och efter avstängning av radion.
