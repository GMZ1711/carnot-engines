(thermo-tweede-hoofdwet)=
# De Tweede Hoofdwet van de Thermodynamica

## Warmte stroomt maar één kant op

De eerste hoofdwet zegt dat energie behouden blijft. Maar ze zegt niets over de **richting**. Dat doet de tweede hoofdwet:

```{prf:theorem} Tweede Hoofdwet van de Thermodynamica
:label: thm-tweede-hoofdwet

Warmte stroomt **altijd** van een warm object naar een koud object, nooit andersom — tenzij er arbeid wordt verricht.
```

## Waarom is dit belangrijk?

Denk aan je dagelijks leven:

| Gebeurt vanzelf ✅ | Gebeurt NIET vanzelf ❌ |
|-------------------|------------------------|
| Hete koffie koelt af | Koude koffie wordt vanzelf warm |
| IJsklontje smelt in warm water | Water bevriest in een warm glas |
| Motor verbrandt brandstof → warmte | Warmte wordt vanzelf brandstof |

```{note}
De tweede hoofdwet verklaart waarom een koelkast **stroom** nodig heeft: je moet arbeid verrichten om warmte van koud naar warm te verplaatsen. Dat gaat niet vanzelf!
```

## De consequentie voor machines

De tweede hoofdwet heeft een belangrijke consequentie voor warmtemotoren:

```{admonition} Geen 100% rendement
:class: warning

Het is **onmogelijk** om een machine te bouwen die alle toegevoerde warmte volledig omzet in arbeid. Er moet altijd een deel warmte worden afgevoerd aan een koudere omgeving.
```

Dit is precies waarom de Carnot-machine zo belangrijk is: Nicolas Carnot bewees dat er een **maximaal rendement** bestaat, en dat dit afhangt van de temperaturen waartussen de machine werkt.

## Warm en koud reservoir

Een warmtemotor werkt altijd tussen twee **reservoirs**:

```{figure} ../figures/warmtemotor-schema.svg
:name: fig-warmtemotor-schema
:width: 100%
:align: center

Schematische weergave van een warmtemotor: warmte stroomt van het warme reservoir naar het koude reservoir. Een deel wordt omgezet in nuttige arbeid (W).
```

De energiebalans is:

$$
Q_h = W + Q_c
$$

Waarbij:
- $Q_h$ = warmte uit het warme reservoir
- $W$ = nuttige arbeid
- $Q_c$ = warmte afgevoerd aan het koude reservoir

```{important}
$Q_c$ is **niet** nul! De tweede hoofdwet zegt dat je altijd warmte moet afvoeren. Dit is de reden dat auto's een radiator en een uitlaat hebben.
```

## Entropie: de wanorde neemt altijd toe

De tweede hoofdwet wordt soms ook uitgedrukt met het begrip **entropie**:

```{prf:definition} Entropie
:label: def-entropie

**Entropie** ($S$) is een maat voor de **wanorde** in een systeem. Bij elk natuurlijk proces neemt de totale entropie toe of blijft gelijk — ze neemt nooit af.
```

```{dropdown} Meer over entropie (verdieping)
Entropie kun je zien als de "verspreiding" van energie. Een kopje hete thee in een koude kamer verliest warmte aan de omgeving — de energie **verspreidt** zich. Dit is een toename van entropie.

Wiskundig:

$$
\Delta S = \frac{Q}{T}
$$

Hoe **lager** de temperatuur waarop warmte wordt toegevoerd, hoe **groter** de toename in entropie.

Bij een Carnot-machine is de totale entropieverandering precies nul — het is een **reversibel** (omkeerbaar) proces. Dat maakt het de meest efficiënte machine die theoretisch mogelijk is.
```

## Samenvatting

| Concept | Betekenis |
|---------|-----------|
| Tweede hoofdwet | Warmte stroomt spontaan van warm → koud |
| Warm reservoir | Energiebron (hoge temperatuur $T_h$) |
| Koud reservoir | Energieafvoer (lage temperatuur $T_c$) |
| Restwarmte $Q_c$ | Moet altijd afgevoerd worden |
| Entropie | Wanorde neemt altijd toe |
| Gevolg | Geen enkele motor kan 100% rendement halen |

```{exercise}
:label: oef-tweede-hoofdwet-1

Een motor ontvangt 1000 J warmte uit een verbrandingsproces en voert 650 J warmte af aan de buitenlucht. Hoeveel nuttige arbeid levert de motor?
```

```{solution} oef-tweede-hoofdwet-1
:class: dropdown

Gegeven: $Q_h = 1000$ J, $Q_c = 650$ J

$$
W = Q_h - Q_c = 1000 - 650 = 350 \text{ J}
$$

De motor levert **350 J** nuttige arbeid.
```

```{exercise}
:label: oef-tweede-hoofdwet-2

Leg in je eigen woorden uit waarom een koelkast stroom nodig heeft. Gebruik de tweede hoofdwet in je verklaring.
```

```{solution} oef-tweede-hoofdwet-2
:class: dropdown

Een koelkast verplaatst warmte van de **koude** binnenkant naar de **warme** buitenkant (de keuken). Volgens de tweede hoofdwet stroomt warmte alleen spontaan van warm naar koud. Om warmte de andere kant op te laten gaan (van koud naar warm), moet er **arbeid** worden verricht. Die arbeid levert de compressor, aangedreven door elektrische stroom.
```
