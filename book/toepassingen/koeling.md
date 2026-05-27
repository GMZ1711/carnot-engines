(toepassingen-koeling)=
# Koeling en Warmtepompen

## De omgekeerde Carnot-cyclus

Wat gebeurt er als je de Carnot-cyclus de andere kant op laat draaien?

In plaats van dat warmte stroomt van warm naar koud en arbeid oplevert, gaan we **arbeid toevoegen** om warmte van koud naar warm te pompen. Dit is de werking van:

- **Koelkasten** — warmte uit de koelkast pompen naar de keuken
- **Airco's** — warmte uit de kamer pompen naar buiten
- **Warmtepompen** — warmte van buiten naar binnen pompen om het huis te verwarmen

```{figure} ../figures/warmtepomp-schema.svg
:name: fig-warmtepomp
:width: 100%
:align: center

Schema van een warmtepomp: met behulp van elektriciteit (W) wordt warmte uit de koude omgeving (Qc) verplaatst naar de warme binnenruimte (Qh). De COP is altijd groter dan 1.
```

Volgens de {ref}`tweede hoofdwet <thermo-tweede-hoofdwet>` stroomt warmte nooit vanzelf van koud naar warm. Daarom moeten we er elektrische energie ($W$) instoppen (de compressor).

---

## Prestatiecoëfficiënt: COP

Bij een motor praten we over *rendement* (wat altijd < 100% is). Bij een koelkast of warmtepomp praten we over de **prestatiecoëfficiënt** of **COP** (Coefficient of Performance). Dit getal kan veel groter zijn dan 1 (of 100%)!

```{prf:definition} COP van een warmtepomp
:label: def-cop-warmtepomp

De COP van een warmtepomp is de verhouding tussen de geleverde warmte ($Q_h$) en de daarvoor benodigde arbeid ($W$):

$$
\text{COP}_{warmtepomp} = \frac{Q_h}{W}
$$
```

Voor een ideale Carnot-warmtepomp hangt de COP alleen af van de temperaturen:

```{math}
:label: eq-cop-carnot

\text{COP}_{Carnot} = \frac{T_h}{T_h - T_c}
```

```{warning}
Ook hier moeten de temperaturen $T_h$ en $T_c$ altijd in **kelvin** (K) staan!
```

---

## Rekenvoorbeeld Warmtepomp

```{admonition} Voorbeeld: Huis verwarmen
:class: note

Een warmtepomp verwarmt een huis tot 20°C (warm reservoir, $T_h$). Buiten is het 5°C (koud reservoir, $T_c$).

**Stap 1:** Reken temperaturen om naar kelvin
- $T_h = 20 + 273 = 293$ K
- $T_c = 5 + 273 = 278$ K

**Stap 2:** Bereken de Carnot-COP
$$
\text{COP}_{Carnot} = \frac{T_h}{T_h - T_c} = \frac{293}{293 - 278} = \frac{293}{15} \approx 19{,}5
$$

Dit betekent dat een ideale warmtepomp voor elke 1 kWh aan elektriciteit maar liefst **19,5 kWh aan warmte** in het huis kan pompen!
```

### De praktijk is anders

In het echt halen warmtepompen deze extreem hoge COP niet door wrijving, pompverliezen en temperatuurverschillen in de warmtewisselaars. Een reële COP voor een warmtepomp onder deze omstandigheden is **4 tot 5**.

Dat is nog steeds fantastisch: voor elke kWh stroom krijg je 4 tot 5 kWh warmte. Dat is veel efficiënter dan een elektrische kachel (die heeft een COP van precies 1).

---

## Waarom daalt de COP als het buiten vriest?

Kijk goed naar de formule:

$$
\text{COP}_{Carnot} = \frac{T_h}{T_h - T_c}
$$

Als het buiten kouder wordt ($T_c$ daalt), wordt de noemer ($T_h - T_c$) groter. Hierdoor wordt de COP **kleiner**.

- Bij $T_c = 10$°C is de ideale COP ca. 29
- Bij $T_c = 0$°C is de ideale COP ca. 15
- Bij $T_c = -10$°C is de ideale COP ca. 10

```{important}
Hoe kouder het buiten is, hoe harder een warmtepomp moet werken en hoe meer stroom hij verbruikt om het binnen warm te krijgen!
```

---

## Samenvatting

| Apparaat | Doel | Formule COP |
|----------|------|-------------|
| **Warmtepomp** | Warmte leveren ($Q_h$) | $\text{COP} = \frac{Q_h}{W}$ |
| **Koelkast / Airco** | Warmte weghalen ($Q_c$) | $\text{COP} = \frac{Q_c}{W}$ |
| **Carnot Warmtepomp** | Ideale prestatie | $\text{COP}_C = \frac{T_h}{T_h - T_c}$ |

```{exercise}
:label: oef-koeling-1

Een warmtepomp heeft een COP van 4,0. De warmtepomp verbruikt 1,5 kW aan elektrisch vermogen. Hoeveel kW aan warmte levert de warmtepomp aan het huis?
```

```{solution} oef-koeling-1
:class: dropdown

Gegeven:
- $\text{COP} = 4{,}0$
- $W = 1{,}5$ kW (elektrisch vermogen)

$$
\text{COP} = \frac{Q_h}{W} \quad \Rightarrow \quad Q_h = \text{COP} \times W = 4{,}0 \times 1{,}5 = \textbf{6,0 kW}
$$

De warmtepomp levert **6,0 kW** aan warmte.
```

```{exercise}
:label: oef-koeling-2

Een koelkast koelt de binnenkant tot 4°C ($T_c$) in een kamer van 21°C ($T_h$).

a) Wat is de maximaal haalbare COP van deze koelkast (Carnot-COP voor koeling)?  
*(Tip: de formule voor Carnot-koeling is $\text{COP}_{koeling} = \frac{T_c}{T_h - T_c}$)*  
b) Leg uit waarom de COP voor koeling lager is dan die voor een warmtepomp.
```

```{solution} oef-koeling-2
:class: dropdown

**a) Carnot-COP voor koeling:**

$T_c = 4 + 273 = 277$ K  
$T_h = 21 + 273 = 294$ K

$$
\text{COP}_{koeling, Carnot} = \frac{T_c}{T_h - T_c} = \frac{277}{294 - 277} = \frac{277}{17} \approx \textbf{16,3}
$$

**b) Verklaring:**

Een warmtepomp levert warmte $Q_h$ aan de warme kamer. Dit is de warmte die uit de koude omgeving is gehaald ($Q_c$) **plus** de toegevoegde arbeid van de compressor ($W$). Er geldt $Q_h = Q_c + W$. 

Omdat een warmtepomp ook de warmte van de arbeid zelf benut voor het verwarmen, is de COP van een warmtepomp altijd precies 1 hoger dan de COP van een koelkast bij dezelfde temperaturen:

$$
\text{COP}_{warmtepomp} = \text{COP}_{koeling} + 1
$$
```
