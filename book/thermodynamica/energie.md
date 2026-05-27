(thermo-energie)=
# Energie, Warmte en Arbeid

## Wat is energie?

Energie is het **vermogen om iets te veranderen**. In de techniek werken we vooral met twee vormen van energieoverdracht:

- **Warmte** ($Q$) — energie die stroomt door een temperatuurverschil
- **Arbeid** ($W$) — energie die wordt overgedragen door een kracht over een afstand

```{prf:definition} Warmte
:label: def-warmte

**Warmte** ($Q$) is de overdracht van energie van een warm object naar een kouder object, veroorzaakt door een temperatuurverschil. Eenheid: joule (J).
```

```{prf:definition} Arbeid
:label: def-arbeid

**Arbeid** ($W$) is de energie die wordt overgedragen wanneer een kracht een object verplaatst. Eenheid: joule (J).
```

## Een praktisch voorbeeld

Denk aan een fietspomp:

| Wat je doet | Wat er gebeurt |
|-------------|---------------|
| Je duwt de pomp in | Je verricht **arbeid** op de lucht |
| De lucht wordt warmer | De temperatuur stijgt |
| De pomp voelt warm aan | **Warmte** stroomt naar je hand |

```{tip}
Arbeid en warmte zijn allebei vormen van energieoverdracht, maar ze werken op een andere manier. Arbeid gaat via een kracht, warmte gaat via een temperatuurverschil.
```

## Interne energie

Elk systeem (een gas, een vloeistof, een machine) heeft **interne energie** ($U$). Dit is de totale energie van alle deeltjes in het systeem:

- Hoe **warmer** het systeem → hoe **meer** interne energie
- Hoe **meer** deeltjes → hoe **meer** interne energie

```{prf:definition} Interne energie
:label: def-interne-energie

**Interne energie** ($U$) is de totale energie van alle moleculen in een systeem, bestaande uit hun kinetische energie (beweging) en potentiële energie (onderlinge krachten). Eenheid: joule (J).
```

```{figure} ../figures/energie-balans.svg
:name: fig-energie-balans
:width: 100%
:align: center

De energiebalans van een systeem: toegevoerde warmte (Q) verhoogt de interne energie (U), verrichte arbeid (W) verlaagt die.
```

## De energiebalans

De verandering van interne energie hangt af van twee dingen:

$$
\Delta U = Q - W
$$

In woorden: de verandering in interne energie is gelijk aan de toegevoerde warmte **min** de verrichte arbeid.

```{admonition} Tekenconventie
:class: warning
Let op de afspraak:
- $Q > 0$ → warmte wordt **toegevoerd** aan het systeem
- $Q < 0$ → warmte wordt **afgevoerd** uit het systeem
- $W > 0$ → het systeem verricht arbeid (levert energie)
- $W < 0$ → er wordt arbeid verricht **op** het systeem
```

## Samenvatting

```{list-table} Overzicht energiebegrippen
:header-rows: 1
:name: tbl-energiebegrippen

* - Begrip
  - Symbool
  - Eenheid
  - Betekenis
* - Warmte
  - $Q$
  - J (joule)
  - Energieoverdracht door temperatuurverschil
* - Arbeid
  - $W$
  - J (joule)
  - Energieoverdracht door kracht × afstand
* - Interne energie
  - $U$
  - J (joule)
  - Totale energie van alle deeltjes in het systeem
```

```{exercise}
:label: oef-energie-1

Een gas in een cilinder ontvangt 500 J warmte en verricht 200 J arbeid op een zuiger. Hoeveel verandert de interne energie van het gas?
```

```{solution} oef-energie-1
:class: dropdown

Gegeven: $Q = 500$ J, $W = 200$ J

$$
\Delta U = Q - W = 500 - 200 = 300 \text{ J}
$$

De interne energie neemt toe met **300 J**.
```
