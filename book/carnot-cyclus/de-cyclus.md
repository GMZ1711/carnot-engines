(carnot-de-cyclus)=
# De Vier Stappen van de Carnot-cyclus

## Het grote plaatje

De Carnot-cyclus bestaat uit **vier stappen** die zich steeds herhalen. Een gas wordt afwisselend verwarmd, uitgezet, afgekoeld en samengeperst. Na de vier stappen is het gas terug bij het beginpunt — vandaar "cyclus".

```{admonition} De vier stappen in het kort
:class: tip

1. **Isotherme expansie** — Gas zet uit bij hoge temperatuur, neemt warmte op
2. **Adiabatische expansie** — Gas zet verder uit zonder warmte-uitwisseling, koelt af
3. **Isotherme compressie** — Gas wordt samengeperst bij lage temperatuur, geeft warmte af
4. **Adiabatische compressie** — Gas wordt verder samengeperst zonder warmte-uitwisseling, warmt op
```

```{figure} ../figures/carnot-pv-diagram.svg
:name: fig-carnot-pv-diagram
:width: 100%
:align: center

De volledige Carnot-cyclus in een pV-diagram. De vier stappen (① t/m ④) vormen een gesloten lus. Het ingesloten oppervlak (gearceerd) is de netto nuttige arbeid W.
```

---

## Stap 1: Isotherme expansie (A → B)

```{prf:definition} Isotherm
:label: def-isotherm-herhaling

**Isotherm** = bij constante temperatuur ($T$ verandert niet).
```

Wat er gebeurt:
- Het gas is in contact met het **warme reservoir** (temperatuur $T_h$)
- Het gas **zet langzaam uit**: het volume neemt toe
- Tijdens het uitzetten neemt het gas warmte ($Q_h$) op van het warme reservoir
- De temperatuur blijft constant op $T_h$
- Het gas verricht **arbeid** op de zuiger (duwt de zuiger naar buiten)

```{admonition} In de praktijk
:class: note
Denk aan een zuiger in een cilinder die langzaam naar buiten beweegt terwijl het gas wordt verwarmd. Het gas duwt de zuiger en dat levert nuttige arbeid.
```

---

## Stap 2: Adiabatische expansie (B → C)

```{prf:definition} Adiabatisch
:label: def-adiabatisch-herhaling

**Adiabatisch** = zonder warmte-uitwisseling met de omgeving ($Q = 0$).
```

Wat er gebeurt:
- Het gas wordt **losgekoppeld** van het warme reservoir (geen warmte meer erbij)
- Het gas **blijft uitzetten** (het volume neemt nog verder toe)
- Omdat er geen warmte bijkomt, **daalt de temperatuur** van $T_h$ naar $T_c$
- Het gas verricht arbeid, maar ten koste van zijn eigen interne energie

```{admonition} In de praktijk
:class: note
Dit is alsof je de verwarming uitzet maar de zuiger nog door laat bewegen. Het gas koelt vanzelf af terwijl het arbeid verricht.
```

---

## Stap 3: Isotherme compressie (C → D)

Wat er gebeurt:
- Het gas is nu in contact met het **koude reservoir** (temperatuur $T_c$)
- Het gas wordt **samengeperst**: het volume neemt af
- Tijdens het samendrukken geeft het gas warmte ($Q_c$) af aan het koude reservoir
- De temperatuur blijft constant op $T_c$
- Er wordt arbeid verricht **op** het gas

```{admonition} In de praktijk
:class: note
Denk aan het samendrukken van lucht terwijl deze kan afkoelen naar de buitenlucht. De warmte die vrijkomt door het comprimeren wordt afgevoerd.
```

---

## Stap 4: Adiabatische compressie (D → A)

Wat er gebeurt:
- Het gas wordt **losgekoppeld** van het koude reservoir
- Het gas wordt **verder samengeperst**
- Omdat er geen warmte kan ontsnappen, **stijgt de temperatuur** van $T_c$ terug naar $T_h$
- Er wordt arbeid verricht op het gas
- Het gas is nu terug bij het **beginpunt** → de cyclus kan opnieuw beginnen

```{admonition} In de praktijk
:class: note
Dit is als het laatste stuk van de compressieslag in een motor: het gas wordt zo sterk samengeperst dat het weer opwarmt tot de begintemperatuur.
```

---

## Overzicht van de vier stappen

```{list-table} De vier stappen van de Carnot-cyclus
:header-rows: 1
:name: tbl-carnot-stappen

* - Stap
  - Naam
  - Temperatuur
  - Warmte
  - Volume
  - Arbeid
* - 1 (A→B)
  - Isotherme expansie
  - Constant ($T_h$)
  - $Q_h$ opgenomen
  - Neemt toe
  - Door gas verricht
* - 2 (B→C)
  - Adiabatische expansie
  - Daalt ($T_h → T_c$)
  - Geen ($Q=0$)
  - Neemt toe
  - Door gas verricht
* - 3 (C→D)
  - Isotherme compressie
  - Constant ($T_c$)
  - $Q_c$ afgegeven
  - Neemt af
  - Op gas verricht
* - 4 (D→A)
  - Adiabatische compressie
  - Stijgt ($T_c → T_h$)
  - Geen ($Q=0$)
  - Neemt af
  - Op gas verricht
```

## De netto arbeid

De **netto arbeid** die de Carnot-machine levert, is het verschil tussen:
- De arbeid die het gas verricht tijdens de expansiestappen (1 + 2)
- De arbeid die nodig is voor de compressiestappen (3 + 4)

$$
W_{netto} = Q_h - Q_c
$$

```{important}
De netto arbeid is altijd **kleiner** dan de toegevoerde warmte $Q_h$. Een deel van de warmte ($Q_c$) moet altijd worden afgevoerd. Dit is een direct gevolg van de {ref}`tweede hoofdwet <thermo-tweede-hoofdwet>`.
```

```{exercise}
:label: oef-cyclus-1

In een Carnot-cyclus neemt het gas 2000 J warmte op van het warme reservoir en geeft 1200 J warmte af aan het koude reservoir. 

a) Hoeveel netto arbeid levert de machine?  
b) In welke stappen wordt er arbeid verricht door het gas?  
c) In welke stappen wordt er arbeid verricht op het gas?
```

```{solution} oef-cyclus-1
:class: dropdown

a) $W_{netto} = Q_h - Q_c = 2000 - 1200 = \textbf{800 J}$

b) Het gas verricht arbeid in **stap 1** (isotherme expansie) en **stap 2** (adiabatische expansie). In deze stappen zet het gas uit en duwt het de zuiger naar buiten.

c) Er wordt arbeid verricht **op** het gas in **stap 3** (isotherme compressie) en **stap 4** (adiabatische compressie). In deze stappen wordt het gas samengeperst.
```

```{exercise}
:label: oef-cyclus-2

Noem bij elke stap van de Carnot-cyclus of er warmte wordt uitgewisseld, en zo ja, in welke richting.
```

```{solution} oef-cyclus-2
:class: dropdown

| Stap | Warmte-uitwisseling |
|------|-------------------|
| 1. Isotherme expansie | Ja — warmte ($Q_h$) stroomt **van** het warme reservoir **naar** het gas |
| 2. Adiabatische expansie | Nee — geen warmte-uitwisseling |
| 3. Isotherme compressie | Ja — warmte ($Q_c$) stroomt **van** het gas **naar** het koude reservoir |
| 4. Adiabatische compressie | Nee — geen warmte-uitwisseling |
```
