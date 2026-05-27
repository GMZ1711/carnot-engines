(rendement-carnot)=
# Het Carnot-rendement

## Wat is rendement?

Het **rendement** ($\eta$, uitgesproken als "eta") van een machine vertelt je welk deel van de ingevoerde energie daadwerkelijk wordt omgezet in nuttige arbeid.

```{prf:definition} Rendement
:label: def-rendement

Het **rendement** is de verhouding tussen de nuttige arbeid en de toegevoerde warmte:

$$
\eta = \frac{W}{Q_h} = \frac{Q_h - Q_c}{Q_h} = 1 - \frac{Q_c}{Q_h}
$$

Het rendement is een getal tussen 0 en 1, of wordt uitgedrukt als percentage (0% – 100%).
```

```{admonition} Voorbeeld
:class: note
Als een motor 1000 J warmte opneemt en 350 J nuttige arbeid levert:

$$
\eta = \frac{350}{1000} = 0{,}35 = 35\%
$$

Dit betekent dat 35% van de warmte is omgezet in arbeid, en 65% als restwarmte is afgevoerd.
```

## De formule van Carnot

Het bijzondere aan de Carnot-machine is dat het rendement **alleen afhangt van de temperaturen**:

```{math}
:label: eq-carnot-rendement

\eta_{Carnot} = 1 - \frac{T_c}{T_h}
```

Waarbij:
- $T_h$ = temperatuur van het warme reservoir (in kelvin!)
- $T_c$ = temperatuur van het koude reservoir (in kelvin!)

```{warning}
Gebruik altijd **kelvin** in deze formule, nooit graden Celsius!

$T(K) = T(°C) + 273$
```

## Wat zegt de formule?

Laten we de formule verkennen met een paar voorbeelden:

```{list-table} Carnot-rendement bij verschillende temperaturen
:header-rows: 1
:name: tbl-rendement-voorbeelden

* - $T_h$ (warm)
  - $T_c$ (koud)
  - $\eta_{Carnot}$
  - Rendement
* - 373 K (100°C)
  - 293 K (20°C)
  - $1 - \frac{293}{373}$
  - **21,4%**
* - 573 K (300°C)
  - 293 K (20°C)
  - $1 - \frac{293}{573}$
  - **48,9%**
* - 773 K (500°C)
  - 293 K (20°C)
  - $1 - \frac{293}{773}$
  - **62,1%**
* - 1273 K (1000°C)
  - 293 K (20°C)
  - $1 - \frac{293}{1273}$
  - **77,0%**
```

### Drie belangrijke inzichten

```{admonition} Inzicht 1: Hoger temperatuurverschil = hoger rendement
:class: tip

Hoe **groter** het verschil tussen $T_h$ en $T_c$, hoe **hoger** het rendement. Daarom werken elektriciteitscentrales met stoom van hoge temperatuur.
```

```{admonition} Inzicht 2: 100% is onmogelijk
:class: warning

Voor $\eta = 100\%$ zou $T_c = 0$ K moeten zijn (het absolute nulpunt, -273°C). Dat is in de praktijk onbereikbaar. Dus **geen enkele warmtemotor kan 100% rendement halen**.
```

```{admonition} Inzicht 3: De Carnot-machine is het maximum
:class: important

Geen enkele machine kan een **hoger** rendement bereiken dan het Carnot-rendement bij dezelfde temperaturen. Dit is een fundamentele natuurwet. Elke echte machine zit eronder.
```

## Rekenvoorbeeld stap voor stap

```{admonition} Voorbeeld: Stoomturbine
:class: note

Een stoomturbine werkt met stoom van 400°C en koelt af met rivierwater van 15°C.

**Stap 1:** Reken temperaturen om naar kelvin
- $T_h = 400 + 273 = 673$ K
- $T_c = 15 + 273 = 288$ K

**Stap 2:** Vul de formule in
$$
\eta_{Carnot} = 1 - \frac{T_c}{T_h} = 1 - \frac{288}{673} = 1 - 0{,}428 = 0{,}572
$$

**Stap 3:** Schrijf het antwoord
$$
\eta_{Carnot} = 57{,}2\%
$$

Dit is het **maximale** rendement. In de praktijk zal deze turbine minder halen door wrijving, warmteverliezen en andere onvolmaaktheden.
```

## Samenvatting

| Begrip | Formule | Eenheid |
|--------|---------|---------|
| Rendement (algemeen) | $\eta = \frac{W}{Q_h}$ | — (of %) |
| Carnot-rendement | $\eta_C = 1 - \frac{T_c}{T_h}$ | — (of %) |
| Netto arbeid | $W = Q_h - Q_c$ | J |

```{exercise}
:label: oef-rendement-1

Een Carnot-machine werkt tussen een warm reservoir van 227°C en een koud reservoir van 27°C.

a) Bereken het Carnot-rendement.
b) Hoeveel nuttige arbeid levert de machine als ze 5000 J warmte opneemt?
c) Hoeveel warmte wordt er afgevoerd aan het koude reservoir?
```

```{solution} oef-rendement-1
:class: dropdown

**a) Carnot-rendement:**

$T_h = 227 + 273 = 500$ K  
$T_c = 27 + 273 = 300$ K

$$
\eta_C = 1 - \frac{T_c}{T_h} = 1 - \frac{300}{500} = 1 - 0{,}6 = 0{,}4 = \textbf{40\%}
$$

**b) Nuttige arbeid:**

$$
W = \eta_C \times Q_h = 0{,}4 \times 5000 = \textbf{2000 J}
$$

**c) Warmte afgevoerd:**

$$
Q_c = Q_h - W = 5000 - 2000 = \textbf{3000 J}
$$
```

```{exercise}
:label: oef-rendement-2

Je wilt een warmtemotor met een Carnot-rendement van minstens 60%. Het koude reservoir is de buitenlucht van 20°C. Wat moet de minimale temperatuur van het warme reservoir zijn?
```

```{solution} oef-rendement-2
:class: dropdown

Gegeven: $\eta_C = 0{,}60$, $T_c = 20 + 273 = 293$ K

De formule omschrijven naar $T_h$:

$$
\eta_C = 1 - \frac{T_c}{T_h} \quad \Rightarrow \quad \frac{T_c}{T_h} = 1 - \eta_C \quad \Rightarrow \quad T_h = \frac{T_c}{1 - \eta_C}
$$

Invullen:

$$
T_h = \frac{293}{1 - 0{,}60} = \frac{293}{0{,}40} = 732{,}5 \text{ K} = \textbf{459{,}5°C}
$$

Het warme reservoir moet minstens **460°C** zijn.
```
