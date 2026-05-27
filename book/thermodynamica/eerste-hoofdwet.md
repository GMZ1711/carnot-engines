(thermo-eerste-hoofdwet)=
# De Eerste Hoofdwet van de Thermodynamica

## Energie gaat nooit verloren

De eerste hoofdwet is eigenlijk heel simpel:

```{prf:theorem} Eerste Hoofdwet van de Thermodynamica
:label: thm-eerste-hoofdwet

Energie kan niet worden gecreëerd of vernietigd, alleen omgezet van de ene vorm naar de andere.

$$
\Delta U = Q - W
$$

De verandering in interne energie ($\Delta U$) van een systeem is gelijk aan de netto toegevoerde warmte ($Q$) minus de door het systeem verrichte arbeid ($W$).
```

## Wat betekent dit in de praktijk?

Stel je een verbrandingsmotor voor:

```{list-table} Energiebalans verbrandingsmotor
:header-rows: 1
:name: tbl-motor-balans

* - Energie-in
  - Energie-uit
* - Brandstof verbranden → warmte ($Q_{in}$)
  - Zuiger beweegt → arbeid ($W$)
* -
  - Uitlaatgassen → warmte ($Q_{uit}$)
* -
  - Wrijving → warmte (verlies)
```

De eerste hoofdwet zegt: **alle energie die erin gaat, komt er ook weer uit**. Niets verdwijnt.

$$
Q_{in} = W + Q_{uit} + Q_{verlies}
$$

```{note}
De eerste hoofdwet vertelt je **hoeveel** energie er is, maar niet **welke richting** de energie op gaat. Dat is de taak van de tweede hoofdwet.
```

## Soorten processen

In de thermodynamica werken we met verschillende soorten processen. Elk proces heeft een bijzondere eigenschap:

````{tab-set}
```{tab-item} Isotherm
**Constante temperatuur** ($T = \text{constant}$)

- De interne energie verandert niet: $\Delta U = 0$
- Dus: $Q = W$
- Alle toegevoerde warmte wordt omgezet in arbeid

*Voorbeeld*: langzaam gas comprimeren terwijl het kan afkoelen
```

```{tab-item} Isobaar
**Constante druk** ($P = \text{constant}$)

- Het gas zet uit of krimpt bij constante druk
- Arbeid: $W = P \cdot \Delta V$

*Voorbeeld*: water koken in een open pan
```

```{tab-item} Isochoor
**Constant volume** ($V = \text{constant}$)

- Er wordt geen arbeid verricht: $W = 0$
- Dus: $\Delta U = Q$
- Alle warmte gaat naar interne energie

*Voorbeeld*: gas verhitten in een afgesloten container
```

```{tab-item} Adiabatisch
**Geen warmte-uitwisseling** ($Q = 0$)

- Dus: $\Delta U = -W$
- Het systeem koelt af als het arbeid verricht
- Het systeem warmt op als er arbeid op wordt verricht

*Voorbeeld*: snelle compressie in een dieselmotor
```
````

```{important}
Twee van deze processen zijn essentieel voor de Carnot-cyclus: het **isotherme** en het **adiabatische** proces. Onthoud deze goed!
```

## Samenvatting

| Proces | Wat is constant? | Gevolg |
|--------|-----------------|--------|
| Isotherm | Temperatuur $T$ | $Q = W$ |
| Isobaar | Druk $P$ | $W = P \cdot \Delta V$ |
| Isochoor | Volume $V$ | $\Delta U = Q$ |
| Adiabatisch | Geen warmte $Q=0$ | $\Delta U = -W$ |

```{exercise}
:label: oef-eerste-hoofdwet-1

Een gas ondergaat een isotherm proces waarbij het 800 J arbeid verricht. Hoeveel warmte moet er worden toegevoerd?
```

```{solution} oef-eerste-hoofdwet-1
:class: dropdown

Bij een isotherm proces geldt: $\Delta U = 0$, dus $Q = W$.

$$
Q = W = 800 \text{ J}
$$

Er moet **800 J** warmte worden toegevoerd.
```

```{exercise}
:label: oef-eerste-hoofdwet-2

Een gas in een afgesloten container (constant volume) ontvangt 1200 J warmte. Hoeveel arbeid verricht het gas en hoeveel verandert de interne energie?
```

```{solution} oef-eerste-hoofdwet-2
:class: dropdown

Bij constant volume: $W = 0$ (het gas kan niet uitzetten).

$$
\Delta U = Q - W = 1200 - 0 = 1200 \text{ J}
$$

Het gas verricht **0 J** arbeid. De interne energie stijgt met **1200 J**.
```
