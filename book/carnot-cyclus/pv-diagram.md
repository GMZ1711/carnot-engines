(carnot-pv-diagram)=
# Het pV-diagram

## Wat is een pV-diagram?

Een **pV-diagram** (druk-volume diagram) is een grafiek waarin je de toestand van een gas kunt aflezen. Op de assen staan:

- **Horizontale as**: Volume ($V$) in m³
- **Verticale as**: Druk ($P$) in Pa

Elke punt in het diagram is een **toestand** van het gas: een combinatie van druk en volume. Een lijn in het diagram is een **proces**: het gas gaat van de ene toestand naar de andere.

```{tip}
Het pV-diagram is het belangrijkste hulpmiddel om thermodynamische processen te begrijpen. Als je dit diagram kunt lezen, snap je de Carnot-cyclus!
```

## De Carnot-cyclus in het pV-diagram

De vier stappen van de Carnot-cyclus vormen een **gesloten lus** in het pV-diagram:

```
    P (druk)
    ↑
    │     A ←──────────── D
    │    ╱ ╲    isotherme    ╱  adiabatische
    │   ╱    ╲  expansie    ╱   compressie
    │  ╱      ╲           ╱
    │ ╱  Tₕ    ╲         ╱
    │╱    ╲      ╲       ╱
    │      ╲      B ───── C
    │       adiabatische    isotherme
    │       expansie        compressie
    │                          T꜀
    └────────────────────────────→ V (volume)
```

De vier hoekpunten zijn:

| Punt | Toestand |
|------|----------|
| **A** | Hoge druk, klein volume, hoge temperatuur $T_h$ |
| **B** | Lagere druk, groter volume, hoge temperatuur $T_h$ |
| **C** | Lage druk, groot volume, lage temperatuur $T_c$ |
| **D** | Hogere druk, kleiner volume, lage temperatuur $T_c$ |

## De stappen aflezen

### Stap 1: A → B (isotherme expansie bij $T_h$)

- De curve gaat **naar rechts** (volume neemt toe)
- De druk **daalt** geleidelijk
- De curve volgt een **isotherm** (lijn van constante temperatuur)
- Het **oppervlak onder de curve** = de arbeid verricht door het gas

### Stap 2: B → C (adiabatische expansie)

- De curve gaat **verder naar rechts** (volume neemt nog meer toe)
- De druk **daalt sneller** dan bij de isotherm
- De temperatuur daalt van $T_h$ naar $T_c$
- De adiabaat is **steiler** dan de isotherm

### Stap 3: C → D (isotherme compressie bij $T_c$)

- De curve gaat **naar links** (volume neemt af)
- De druk **stijgt** geleidelijk
- De curve volgt een **isotherm** bij de lagere temperatuur $T_c$

### Stap 4: D → A (adiabatische compressie)

- De curve gaat **verder naar links** terug naar punt A
- De druk **stijgt snel**
- De temperatuur stijgt van $T_c$ terug naar $T_h$

## Het oppervlak = de netto arbeid

```{important}
Het **oppervlak binnen de gesloten lus** (A→B→C→D→A) is gelijk aan de **netto arbeid** die de Carnot-machine levert per cyclus.

Hoe groter het oppervlak, hoe meer arbeid de machine levert.
```

Dit kun je als volgt begrijpen:
- De arbeid verricht **door** het gas (stap 1 + 2) is het oppervlak onder de bovenste curves
- De arbeid verricht **op** het gas (stap 3 + 4) is het oppervlak onder de onderste curves
- Het **verschil** is het ingesloten oppervlak = de netto arbeid

## Isothermen vs. adiabaten

In het pV-diagram kun je de twee typen curves herkennen:

```{list-table} Isothermen en adiabaten vergelijken
:header-rows: 1
:name: tbl-isotherm-vs-adiabaat

* - Eigenschap
  - Isotherm
  - Adiabaat
* - Temperatuur
  - Constant
  - Verandert
* - Warmte-uitwisseling
  - Ja ($Q \neq 0$)
  - Nee ($Q = 0$)
* - Steilheid in pV-diagram
  - Minder steil
  - Steiler
* - Vergelijking (ideaal gas)
  - $PV = \text{constant}$
  - $PV^\gamma = \text{constant}$
```

```{dropdown} Wat is γ (gamma)?
$\gamma$ (gamma) is de **warmtecapaciteitsverhouding** van het gas. Voor lucht (en andere tweeatomige gassen) geldt:

$$\gamma = \frac{c_p}{c_v} \approx 1{,}4$$

Hierdoor is de adiabaat steiler dan de isotherm: bij een adiabatisch proces verandert de druk sneller bij dezelfde volumeverandering.
```

## Het pV-diagram lezen: stappenplan

Als je een pV-diagram van een Carnot-cyclus voor je hebt, kun je deze vragen beantwoorden:

1. **Waar zijn de isotherme stappen?** → De minder steile curves (bovenste en onderste)
2. **Waar zijn de adiabatische stappen?** → De steilere curves (linker en rechter)
3. **Welke isotherm hoort bij $T_h$?** → De bovenste (hogere druk)
4. **Welke isotherm hoort bij $T_c$?** → De onderste (lagere druk)
5. **Hoeveel netto arbeid?** → Het ingesloten oppervlak

```{exercise}
:label: oef-pv-1

Bekijk het pV-diagram van een Carnot-cyclus. Bij welke stap(pen):
a) Neemt het volume toe?
b) Is de druk het hoogst?
c) Vindt er warmte-opname plaats?
```

```{solution} oef-pv-1
:class: dropdown

a) Het volume neemt toe bij **stap 1** (isotherme expansie, A→B) en **stap 2** (adiabatische expansie, B→C).

b) De druk is het hoogst bij **punt A** — dit is het beginpunt met het kleinste volume en de hoogste temperatuur.

c) Warmte-opname vindt plaats bij **stap 1** (isotherme expansie bij $T_h$). In deze stap neemt het gas warmte $Q_h$ op van het warme reservoir.
```

```{exercise}
:label: oef-pv-2

Waarom is het ingesloten oppervlak in het pV-diagram gelijk aan de netto arbeid? Leg dit uit in je eigen woorden.
```

```{solution} oef-pv-2
:class: dropdown

In een pV-diagram geldt: het oppervlak onder een procescurve is gelijk aan de arbeid tijdens dat proces.

- Bij de **expansiestappen** (boven, A→B→C) is het oppervlak eronder de arbeid die het gas verricht (positief, want het gas duwt).
- Bij de **compressiestappen** (onder, C→D→A) is het oppervlak eronder de arbeid die **op** het gas verricht wordt (negatief voor het gas).

Het verschil — dus het **ingesloten oppervlak** — is de netto arbeid: wat er over blijft na aftrek van de compressie-arbeid van de expansie-arbeid.
```
