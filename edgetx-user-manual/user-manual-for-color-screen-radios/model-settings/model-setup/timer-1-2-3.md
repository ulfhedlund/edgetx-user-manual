# Timer 1/2/3

<figure><img src="../../../../.gitbook/assets/timers.png" alt=""><figcaption><p>Konfiguration av timer</p></figcaption></figure>

EdgeTX har 3 timers som var och en kan konfigureras individuellt. Följande konfigureringsalternativ finns:

**Namn:** Namnet på timern

**Typ**:

* **Av**- Timern används inte
* **På \*\*\*** - Timern är på så länge som konfigurerad brytare är aktiv. Timern stoppas när brytaren inaktiveras.
* **Start** \*\*\* - Timern är på hela tiden oavsett brytarens läge.
* **Gas** - Timern startar när gasen höjs över noll och konfigurerad brytare är aktiv. Timern stoppar antingen när gasen sänks till noll eller brytaren inaktiveras.
* **Gas %** - Timern är på och räknas upp proportionellt i förhållande till gasläget. Vid full gas är förhållandet 1/1 (reell tid) och vid halv gas 1/2 (50%).
* **Gas Start** - Timern startar när gasen höjs över noll och konfigurerad brytare är aktiv. Därefter är timern på så länge brytaren är aktiv, oavsett gasläget.

{% hint style="info" %}
**Gas**, **Gas % och Gas Start** kan aktiveras av en brytare (även en logisk brytare), vred eller värdet av en annan kanal än gaskanalen. Detta specificeras i fältet **Gaskälla** i sektionen [throttle.md](throttle.md "mention") in **Modellinställningar**.
{% endhint %}

**Switch -** Ange den brytare som ska trigga att timern startar. Om ingen brytare är vald triggas timern enbart beroende på dess typ. Utöver en brytare kan du även ange en trimmer, telemetrikälla (som triggas när data tas emot från källan) eller endera slags fysisk aktivitet (en spak som rörs eller en knapptryckning, kallad **Act)**.

{% hint style="info" %}
De poster som har ett "!" före brytarnamnet betyder att villkoret är inverterat. \
Till exempel: "!SA-" betyder "när brytare SA inte är i sin mitten/centerposition", det vill säga den antingen är upp eller ner.
{% endhint %}

**Start -** Tiden som avänds för timerns avancerade funktioner. Förvald tid är 00:00 och om den lämnas oförändrad fungerar timern som ett stoppur, som räknar upp tills den stoppas. Om en annan tid än 00:00 anges i startfältet, visas ett nytt flervalsfält **Riktning**.

**Riktning** - Om satt till **Visa återstående** kommer timern att räkna neråt från angiven tid ner till noll och därefter varna användaren. Om den är satt till **Visa förbrukad** fungerar timern som ett alarm, genom att räkna upp från noll till angiven tid och därefter varna användaren.

**Minutpip** - Om minutpip är aktiverat kommer du bli meddelad när varje minut passerat, som beskrivet under **Nedräkning**.

**Nedräkning:**

* **Tyst** - No notification is given until the timer reaches zero. When it reaches zero, you will hear one beep.
* **Pip** - The radio will beep every second starting at the time designated.
* **Röst** - The radio will count down by second starting at the time designated.
* **Vibrera** -The radio will vibrate every second starting at the time designated.

**Alltid på:**

* **Av** - The timer value is reset when switching models or when the radio is turned off / on.
* **Flygning** - The timer value is NOT reset when switching models or when radio is turned off / on. The timer value is only reset when the **Reset flight** option is selected in the [Reset telemetry ](../../reset-telemetry.md)menu.
* **Nolla själv -** The timer value is reset only when it is individually selected to be reset (example: Reset timer1) in the [Reset telemetry ](../../reset-telemetry.md)menu.

{% hint style="info" %}
The **Flight** persistent setting can be set for multiple timers and then these timers can be reset simultaneously with the **Reset flight** option.
{% endhint %}
