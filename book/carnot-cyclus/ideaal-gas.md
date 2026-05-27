(carnot-ideaal-gas)=
# Het Ideale Gas

## Wat is een ideaal gas?

Om de Carnot-cyclus te begrijpen, werken we met een vereenvoudigd model: het **ideale gas**. Dit is een denkbeeldig gas dat zich "perfect" gedraagt.

```{prf:definition} Ideaal gas
:label: def-ideaal-gas

Een **ideaal gas** is een theoretisch gas waarbij:
- De gasdeeltjes geen volume innemen
- Er geen krachten zijn tussen de deeltjes
- Botsingen perfect elastisch zijn (geen energieverlies)
```

```{tip}
Een ideaal gas bestaat niet echt, maar echte gassen (zoals lucht) gedragen zich bij lage drukken en hoge temperaturen bijna als een ideaal gas. Het is dus een goede benadering!
```

## De Ideale Gaswet

Het gedrag van een ideaal gas wordt beschreven door één formule:

```{math}
:label: eq-ideale-gaswet

P \cdot V = n \cdot R \cdot T
```

| Symbool | Betekenis | Eenheid |
|---------|-----------|---------|
| $P$ | Druk | Pa (pascal) |
| $V$ | Volume | m³ |
| $n$ | Hoeveelheid stof | mol |
| $R$ | Gasconstante | 8,314 J/(mol·K) |
| $T$ | Temperatuur | K (kelvin) |

```{warning}
Temperatuur moet altijd in **kelvin** (K) staan, niet in graden Celsius!

Omrekenen: $T(K) = T(°C) + 273{,}15$

Voorbeelden:
- 0°C = 273 K
- 20°C = 293 K
- 100°C = 373 K
```

## Wat zegt de gaswet?

De ideale gaswet legt het verband tussen druk, volume en temperatuur:

````{tab-set}
```{tab-item} Druk verhogen
Als je het volume **kleiner** maakt (bij constante temperatuur), gaat de druk **omhoog**.

*Voorbeeld*: Een fietsband oppompen — je perst lucht in een kleiner volume.
```

```{tab-item} Temperatuur verhogen
Als je de temperatuur **verhoogt** (bij constant volume), gaat de druk **omhoog**.

*Voorbeeld*: Een spuitbus in de zon — de druk stijgt en de bus kan ontploffen.
```

```{tab-item} Volume vergroten
Als je de temperatuur **verhoogt** (bij constante druk), wordt het volume **groter**.

*Voorbeeld*: Een heteluchtballon — warme lucht zet uit en de ballon stijgt op.
```
````

## De gaswet in de Carnot-cyclus

In de Carnot-cyclus wordt een ideaal gas afwisselend samengedrukt en uitgezet. Bij elke stap veranderen $P$, $V$ en $T$ volgens de ideale gaswet.

| Stap in de cyclus | Wat verandert? |
|-------------------|---------------|
| Isotherme expansie | $V$ neemt toe, $P$ neemt af, $T$ constant |
| Adiabatische expansie | $V$ neemt toe, $P$ neemt af, $T$ daalt |
| Isotherme compressie | $V$ neemt af, $P$ neemt toe, $T$ constant |
| Adiabatische compressie | $V$ neemt af, $P$ neemt toe, $T$ stijgt |

```{exercise}
:label: oef-ideaal-gas-1

Een ideaal gas heeft een volume van 2,0 liter bij een temperatuur van 20°C en een druk van 1,0 × 10⁵ Pa. Bereken het aantal mol gas. (Gebruik $R = 8{,}314$ J/(mol·K))
```

```{solution} oef-ideaal-gas-1
:class: dropdown

Gegeven:
- $V = 2{,}0$ L $= 2{,}0 \times 10^{-3}$ m³
- $T = 20°C = 293$ K
- $P = 1{,}0 \times 10^5$ Pa

De ideale gaswet: $PV = nRT$, dus:

$$
n = \frac{PV}{RT} = \frac{1{,}0 \times 10^5 \times 2{,}0 \times 10^{-3}}{8{,}314 \times 293} = \frac{200}{2436} \approx 0{,}082 \text{ mol}
$$
```

```{exercise}
:label: oef-ideaal-gas-2

Reken de volgende temperaturen om van Celsius naar Kelvin:
1. 25°C
2. -10°C
3. 500°C
```

```{solution} oef-ideaal-gas-2
:class: dropdown

$T(K) = T(°C) + 273$

1. 25 + 273 = **298 K**
2. -10 + 273 = **263 K**
3. 500 + 273 = **773 K**
```
