(toepassingen-warmtemotoren)=
# Echte Warmtemotoren vs. Carnot

## Waarom halen echte motoren het Carnot-rendement niet?

Een Carnot-machine is een **ideale** machine. In de praktijk hebben we te maken met verliezen. Laten we eens kijken waarom echte motoren (zoals een benzinemotor of een stoomturbine) een lager rendement halen.

### 1. Wrijving
In echte motoren bewegen metalen onderdelen langs elkaar (zoals zuigers in cilinders). Dit veroorzaakt **wrijving**, waardoor nuttige arbeid verloren gaat als warmte. De Carnot-cyclus gaat uit van nul wrijving.

### 2. Warmteverliezen
In de Carnot-cyclus zijn de adiabatische stappen perfect geïsoleerd ($Q=0$). In het echt lekt er altijd warmte weg via de wanden van de cilinder naar de buitenlucht. Die warmte kan geen arbeid meer leveren.

### 3. Snelheid van processen
De isotherme stappen in een Carnot-machine moeten heel langzaam gaan om de temperatuur constant te houden. Echte motoren moeten snel draaien (bijv. 3000 toeren per minuut) om vermogen te leveren. Hierdoor verlopen de processen niet ideaal.

---

## Vergelijking van rendementen

Laten we eens kijken naar het rendement van echte warmtemotoren in vergelijking met hun theoretische Carnot-limiet:

```{list-table} Praktijkrendementen vs. Carnot-limiet
:header-rows: 1
:name: tbl-rendement-vergelijking

* - Motortype
  - Praktijkrendement
  - Carnot-limiet
  - Waarom het verschil?
* - **Benzinemotor** (auto)
  - 25% – 30%
  - ca. 60%
  - Snelle verbranding, hoge wrijving, koelingsverlies.
* - **Dieselmotor** (vrachtwagen)
  - 35% – 45%
  - ca. 65%
  - Hogere compressieverhouding (dus hogere $T_h$).
* - **Gas- en stoomcentrale**
  - 50% – 60%
  - ca. 80%
  - Zeer geavanceerde systemen met minimale wrijving en extreem hoge temperaturen.
```

```{important}
Zelfs de meest geavanceerde elektriciteitscentrale ter wereld kan de Carnot-limiet niet overschrijden. Het Carnot-rendement is een harde natuurkundige grens!
```

---

## Hoe verhogen we het rendement van echte motoren?

Als technicus of ingenieur wil je het rendement zo hoog mogelijk hebben. De Carnot-formule geeft de oplossing:

$$
\eta_{Carnot} = 1 - \frac{T_c}{T_h}
$$

Om het rendement te verhogen kun je twee dingen doen:

1. **Verhoog $T_h$ (de bron-temperatuur):**
   - Hoe heter het verbrandingsgas, hoe hoger het rendement.
   - *Limiet*: Materialen moeten bestand zijn tegen deze extreme hitte (smeltpunt van metalen).

2. **Verlaag $T_c$ (de afkoel-temperatuur):**
   - Koelen met zo koud mogelijk water of lucht.
   - *Limiet*: We zijn afhankelijk van de temperatuur van de omgeving (rivierwater of buitenlucht).

```{exercise}
:label: oef-motoren-1

Een kolencentrale verbrandt kolen op een temperatuur van 550°C. Het koelwater uit de rivier is 12°C. De centrale levert elektriciteit met een werkelijk rendement van 42%.

a) Bereken het theoretische maximale rendement (Carnot-rendement).  
b) Hoeveel procent van het theoretische maximum wordt in de praktijk gehaald?
```

```{solution} oef-motoren-1
:class: dropdown

**a) Carnot-rendement:**

$T_h = 550 + 273 = 823$ K  
$T_c = 12 + 273 = 285$ K

$$
\eta_C = 1 - \frac{T_c}{T_h} = 1 - \frac{285}{823} = 1 - 0{,}346 = 0{,}654 = \textbf{65,4\%}
$$

Het theoretische maximum is **65,4%**.

**b) Percentage van maximum:**

Het werkelijke rendement is 42%.

$$
\text{Verhouding} = \frac{\eta_{werkelijk}}{\eta_{Carnot}} = \frac{42}{65{,}4} \approx 0{,}642 = \textbf{64,2\%}
```
