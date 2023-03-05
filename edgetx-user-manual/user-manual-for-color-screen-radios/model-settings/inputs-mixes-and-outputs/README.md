# Input, Mixar & Output

För att kunna stödja många olika typer av radiosändare använder EdgeTX ett generiskt kontrolldataflöde som kan användas i alla sändare. I detta dataflöde kan endera av radions fysiska kontroller (spakar, brytare, vred, reglage) mappas till en input i radions mjukvara (firmware). Dessa inputs kan direkt kopplas till en mix eller kombineras med andra inputs till en enskild mix. Dessa mixar kan modifieras genom att applicera vikt, offset och kurvor och kopplas sedan till en enskild kanal i output. Slutliga justeringar av kontrolldata kan därefter göras (inklusive subtrim, kurvor, start-, mitt- och ändpunkt) innan kontrolldata slutligen skickas till sändarmodulen. Nedanstående flödesschema beskriver översiktligt dataflödet för kontrollerna. Detaljerad information om flödet finns under sidorna [Input](inputs.md), [Mixar](mixes.md) och [Output](outputs.md).

<figure><img src="../../../../.gitbook/assets/inputflow (1).jpg" alt=""><figcaption><p>Kontrollernas dataflöde</p></figcaption></figure>

EdgeTX använder nedanstående ikoner för att skilja på olika typer av källor.

<figure><img src="../../../../.gitbook/assets/inputicons (1).jpg" alt=""><figcaption><p>Källikoner</p></figcaption></figure>
