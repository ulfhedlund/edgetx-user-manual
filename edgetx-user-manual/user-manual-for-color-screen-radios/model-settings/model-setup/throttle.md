# Gas

<figure><img src="../../../../.gitbook/assets/throttle.png" alt=""><figcaption><p>Inställningar för gas</p></figcaption></figure>

I EdgeTX finns möjligheten att ange en specifik källa och trim för modellens gas (trottel). Följande inställningsmöjligheter finns:

**Inverterad gas:** Om detta alternativ är aktiverat inverteras riktningen för den konfigurerade gaskanalen.

**Gaskälla:** Källan som används till gasen.

**Trimma tomgång**: Om detta alternativ är aktiverat kommer gastrimmen endast att påverka den nedre delen av gasens omfång.

{% hint style="info" %}
Exempelvis, med **Trimma tomgång** aktiverad kan gasspaken i nedre läget ha ett värde -80 medan mittläget har värdet 0 och högsta läget värdet 100. Om **Trimma tomgång** i stället är inaktiverat kan gasspaken i nedre läget ha ett värde av -80 medan mittläget har värdet 20 och högsta läget värdet 100.&#x20;
{% endhint %}

**Gastrimmknapp:** The trim switch that will be used to trim the throttle. It is possible to substitute the throttle trim switch with the aileron, rudder, or elevator trim switches.
