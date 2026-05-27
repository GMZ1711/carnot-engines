(oefeningen-berekeningen)=
# Oefenopgaven en Vragen

## Deel A: Theorievragen

```{exercise}
:label: opg-theorie-1

Wat is de belangrijkste conclusie die Sadi Carnot trok over het rendement van een warmtemotor?

A) Het rendement hangt af van het soort gas dat je gebruikt.  
B) Het rendement kan nooit hoger zijn dan 50%.  
C) Het rendement hangt alleen af van de temperaturen van het warme en koude reservoir.  
D) Met betere smering kan een motor een rendement van 100% halen.
```

```{solution} opg-theorie-1
:class: dropdown

Het juiste antwoord is **C**. 

Sadi Carnot bewees dat het maximale rendement van een warmtemotor alleen afhangt van de temperaturen van de reservoirs waartussen de motor werkt ($T_h$ en $T_c$). De constructie of het type gas (werkmedium) maakt voor dit theoretische maximum niet uit.
```

```{exercise}
:label: opg-theorie-2

Tijdens welk proces in de Carnot-cyclus verandert de temperatuur van het gas **niet**, maar neemt het volume wel toe?

A) Adiabatische expansie  
B) Isotherme expansie  
C) Isotherme compressie  
D) Adiabatische compressie
```

```{solution} opg-theorie-2
:class: dropdown

Het juiste antwoord is **B**.

- **Isotherm** betekent constante temperatuur (de temperatuur verandert dus niet).
- **Expansie** betekent volumetoename (het volume neemt dus toe).
```

---

## Deel B: Rekenopgaven

```{exercise}
:label: opg-rekenen-1

Een benzinemotor in een auto verbrandt brandstof bij een temperatuur van 1200°C. De uitlaatgassen worden afgevoerd bij een temperatuur van 80°C.

a) Bereken het Carnot-rendement van deze motor.  
b) Het werkelijke rendement van de motor is 28%. Hoeveel procent van het theoretische maximum haalt deze motor in de praktijk?
```

```{solution} opg-rekenen-1
:class: dropdown

**a) Carnot-rendement:**

Eerst Celsius omrekenen naar Kelvin:
- $T_h = 1200 + 273 = 1473$ K
- $T_c = 80 + 273 = 353$ K

Nu de Carnot-formule invullen:

$$
\eta_{Carnot} = 1 - \frac{T_c}{T_h} = 1 - \frac{353}{1473} = 1 - 0{,}240 = 0{,}760 = \textbf{76,0\%}
$$

**b) Percentage van het maximum:**

Het werkelijke rendement is 28%. We berekenen de verhouding:

$$
\text{Verhouding} = \frac{\eta_{werkelijk}}{\eta_{Carnot}} \times 100\% = \frac{28\%}{76{,}0\%} \times 100\% \approx \textbf{36,8\%}
$$

De motor haalt in de praktijk dus **36,8%** van zijn theoretisch maximale rendement.
```

```{exercise}
:label: opg-rekenen-2

Een warmtepomp verwarmt een woning. Het warmteafgiftesysteem in huis werkt op 35°C (vloerverwarming). De warmtepomp haalt zijn warmte uit de bodem, waar de temperatuur 10°C is.

a) Bereken de theoretische maximale COP (Carnot-COP) van deze warmtepomp.  
b) Als de warmtepomp een werkelijke COP heeft van 4,5 en hij verbruikt 2,0 kW aan elektriciteit, hoeveel warmte (in kW) levert hij dan aan de woning?
```

```{solution} opg-rekenen-2
:class: dropdown

**a) Carnot-COP:**

Temperaturen omrekenen naar Kelvin:
- $T_h = 35 + 273 = 308$ K
- $T_c = 10 + 273 = 283$ K

Formule invullen:

$$
\text{COP}_{Carnot} = \frac{T_h}{T_h - T_c} = \frac{308}{308 - 283} = \frac{308}{25} = \textbf{12,32}
$$

**b) Geleverde warmte:**

Gegeven:
- $\text{COP}_{werkelijk} = 4{,}5$
- $W = 2{,}0$ kW

$$
\text{COP} = \frac{Q_h}{W} \quad \Rightarrow \quad Q_h = \text{COP} \times W = 4{,}5 \times 2{,}0 \text{ kW} = \textbf{9,0 kW}
$$

De warmtepomp levert **9,0 kW** aan warmte aan de woning.
```

```{exercise}
:label: opg-rekenen-3

Een ideaal gas bevindt zich in een afgesloten cilinder met een volume van 0,05 m³ en een druk van 2,0 × 10⁵ Pa. De temperatuur van het gas is 20°C. 

a) Reken de temperatuur om naar Kelvin.  
b) Bereken de hoeveelheid stof (in mol) van het gas. (Gebruik $R = 8{,}314$ J/(mol·K))
```

```{solution} opg-rekenen-3
:class: dropdown

**a) Temperatuur in Kelvin:**

$$
T = 20 + 273 = \textbf{293 K}
$$

**b) Aantal mol gas:**

Gebruik de ideale gaswet: $PV = nRT$, dus $n = \frac{PV}{RT}$.

Gegevens invullen:

$$
n = \frac{2{,}0 \times 10^5 \text{ Pa} \times 0{,}05 \text{ m}^3}{8{,}314 \text{ J/(mol}\cdot\text{K)} \times 293 \text{ K}} = \frac{10000}{2436} \approx \textbf{4,11 mol}
$$

Het gas bevat **4,11 mol** stof.
```
