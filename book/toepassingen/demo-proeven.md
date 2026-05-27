(toepassingen-demo-proeven)=
# Demo's uit de praktijk

In dit hoofdstuk vind je zes klassikale demonstratieproeven die de theorie van de Carnot-engine tastbaar maken. De proeven komen uit de [Show the Physics](https://github.com/FreekPols/ShowthePhysics) collectie van de TU Delft — gelicenseerd onder CC‑BY‑4.0.

```{admonition} Bronvermelding
:class: note
De demo's in dit hoofdstuk zijn afkomstig uit: Freek Pols e.a., *Show the Physics* (TU Delft). De teksten zijn bewerkt en vertaald voor dit boek. Licentie: [CC BY 4.0](https://creativecommons.org/licenses/by/4.0/).
```

---

(demo-koken-vacuum)=
## 1. Koken zonder warmte — onder vacuüm

*Door Paul Hupkens en Ed van den Berg | Tijdsduur: 15 min | Niveau: vanaf klas 2*

```{figure} ../figures/demo-koken-vacuum.svg
:width: 80%
:align: center
:name: fig-demo-koken-vacuum

Water koken op kamertemperatuur door de luchtdruk te verlagen.
```

### Wat zie je?
Water in een bekerglas begint te **koken bij kamertemperatuur** zodra de luchtdruk onder een vacuümstolp sterk wordt verlaagd. Er ontstaan bubbels en de thermometer laat geen temperatuurstijging zien — integendeel: de temperatuur daalt juist.

### Waarom is dit bijzonder?
Normaal kookt water bij 100°C (op zeeniveau). Pas dan is de dampdruk in de bellen hoog genoeg om de luchtdruk te overwinnen. **Verlaag je de luchtdruk**, dan kunnen bellen al bij een veel lagere temperatuur overleven — het water "kookt" zonder vuur.

### Wat heeft dit met Carnot te maken?

- **Druk × Volume** — De pV-relatie uit de ideale gaswet bepaalt of bellen groeien of imploderen.
- **Faseovergang** — Verdampen kost energie (latente warmte) → het water **koelt af** tijdens het koken.
- **Eerste hoofdwet** — $\Delta U = Q - W$: zonder warmtetoevoer ($Q = 0$) daalt $U$, dus daalt $T$.

---

(demo-radiometer)=
## 2. De radiometer van Crookes

*Door Kirsten Stadermann | Tijdsduur: 15–30 min | Niveau: bovenbouw*

```{figure} ../figures/demo-radiometer.svg
:width: 70%
:align: center
:name: fig-demo-radiometer

Een Crookes-radiometer: gasdeeltjes aan de zwarte (warme) kant bewegen sneller en laten het molentje draaien.
```

### Wat zie je?
Een glazen bol met een molentje van zwart/wit-gekleurde wieken begint te draaien in **zonlicht**. De zwarte kant beweegt *weg* van het licht. Zet je de bol in de schaduw, dan stopt de draaiing. Houd je er ijs tegen, dan draait het molentje zelfs de andere kant op.

### Waarom draait het?
Lang werd gedacht dat lichtdeeltjes (fotonen) de wieken duwen — maar dat klopt niet. De moderne verklaring: gasmoleculen aan de **warme zwarte kant** bewegen sneller en botsen harder tegen de wieken dan de tragere moleculen aan de koele witte kant. De terugstoot ("kick") van die botsingen laat het molentje draaien.

### Wat heeft dit met Carnot te maken?

- **Temperatuur en moleculaire snelheid** — Hoe hoger $T$, hoe sneller de gasdeeltjes. Direct zichtbaar!
- **Tweede hoofdwet** — Warmte stroomt van de hete zwarte kant naar de koele witte kant.
- **Moleculair denken** — De Carnot-cyclus gaat over een "ideaal gas". Met de radiometer zie je letterlijk het gedrag van echte gasmoleculen.

---

(demo-vlamkoeler)=
## 3. De vlamkoeler

*Door Kirsten Stadermann | Tijdsduur: 5–10 min | Niveau: alle klassen*

```{figure} ../figures/demo-vlamkoeler.svg
:width: 80%
:align: center
:name: fig-demo-vlamkoeler

Een koperen spiraal rond de kaarsvlam voert warmte zo snel af dat de vlam dooft.
```

### Wat zie je?
Een brandende kaars. Breng een **koperen spiraal** van bovenaf over de vlam — de zichtbare vlam verdwijnt zodra de spiraal de hete gassen omhult. Haal je de spiraal weg, dan ontvlamt het kaarsvet weer (als het nog heet genoeg is).

### Waarom dooft de vlam?
Voor verbranding zijn drie dingen nodig: brandstof (kaarsvetdamp), zuurstof en een **voldoende hoge temperatuur**. Koper is een uitstekende warmtegeleider. De spiraal neemt zoveel warmte op dat de temperatuur van de kaarsvetdamp **onder de ontbrandingstemperatuur zakt**. De damp is er nog wél — je kunt hem boven de spiraal opnieuw aansteken.

### Wat heeft dit met Carnot te maken?

- **Warmtegeleiding** — Energieverlies via geleiding is een van de redenen dat echte motoren het Carnot-rendement niet halen.
- **Rendementsverlies** — $Q_{verlies}$ in de energiebalans: $Q_h = W + Q_c + Q_{verlies}$.
- **Activeringsenergie** — Verbranding heeft een drempeltemperatuur nodig; bij een echte motor heet dit de "zelfontbrandingstemperatuur".

---

(demo-kaarsenval)=
## 4. De kaarsenval

*Door Norbert van Veen | Tijdsduur: 5–10 min | Niveau: onderbouw*

```{figure} ../figures/demo-kaarsenval.svg
:width: 80%
:align: center
:name: fig-demo-kaarsenval

Twee kaarsen onder een stolp. De bovenste kaars dooft het eerst. Waarom?
```

### Wat zie je?
Onder een glazen stolp staan twee brandende kaarsen: één lange en één korte. Na enkele seconden zie je dat de **bovenste (langste) kaars als eerste dooft**, terwijl de onderste nog even blijft branden. Leerlingen voorspellen vaak het omgekeerde!

### Waarom de bovenste eerst?
Bij verbranding ontstaat **CO₂**, een warm gas dat door zijn lage dichtheid naar boven stijgt. Het hoopt zich op tegen de bovenkant van de stolp. De lange kaars staat in deze CO₂-laag en krijgt te weinig zuurstof. De korte kaars profiteert nog even van de zuurstofrijke lucht onderin.

### Wat heeft dit met Carnot te maken?

- **Convectie** — Warme gassen stijgen op. In een warmtemotor zorgt convectie voor de afvoer van restwarmte.
- **Verbranding & zuurstof** — Een echte motor regelt het brandstof/lucht-mengsel; zonder zuurstof geen verbranding, geen $Q_h$.
- **Temperatuursverschillen** — CO₂ is warm en stijgt → temperatuurgelaagdheid = direct gevolg van $\Delta T$ in Carnot.

---

(demo-condensatiewarmte)=
## 5. Condensatiewarmte zichtbaar in infrarood

*Door Norbert van Veen | Tijdsduur: 10–30 min | Niveau: klas 4 en hoger*

```{figure} ../figures/demo-condensatiewarmte.svg
:width: 80%
:align: center
:name: fig-demo-condensatiewarmte

Een infraroodcamera laat zien dat condensatie van waterdamp het papier opwarmt — een nanoscopisch proces dat wél meetbaar is.
```

### Wat zie je?
Met een **infraroodcamera** (FLIR) meet je de temperatuur van een vel papier dat boven een schaaltje water ligt. Na een minuut is een ronde warmere plek zichtbaar — het papier is daar **1°C warmer** dan de omgeving. Haal je het papier weg, dan koelt de plek snel af.

### Wat gebeurt hier?
Waterdamp uit het schaaltje condenseert aan de onderkant van het papier. Bij condensatie komt **latente warmte** vrij — dezelfde energie die je in water stopt om het te laten verdampen. Het laagje water dat condenseert is slechts **~50 nanometer** dik, maar levert genoeg energie om het papier meetbaar op te warmen.

### Wat heeft dit met Carnot te maken?

- **Faseovergangen en energie** — Bij de Carnot-machine gaat het alleen om gas. Bij echte machines spelen verdamping en condensatie wél een rol (stoomturbines!).  
- **Latente warmte** — $Q = m \cdot L$ — de verborgen energie die vrijkomt of nodig is bij faseovergangen beïnvloedt het totale rendement.
- **Tweede hoofdwet** — Condensatie "levert" warmte aan de omgeving, precies de omgekeerde richting van wat je met een warmtepomp wil bereiken.

---

(demo-koken-koelen)=
## 6. Koken door te koelen

*Door Ed van den Berg | Tijdsduur: 15 min | Niveau: alle klassen*

```{figure} ../figures/demo-koken-koelen.svg
:width: 90%
:align: center
:name: fig-demo-koken-koelen

Links: water koken op 100°C. Rechts: dezelfde fles omgekeerd, koud water erover — het water kookt opnieuw bij 80°C!
```

### Wat zie je?
Water wordt in een erlenmeyer aan de kook gebracht (100°C). Zet je de brander uit, sluit je de fles met een stop, en keer je hem om — en giet je vervolgens **koud water** over de fles — dan begint het water opnieuw te koken! De thermometer wijst nu slechts ~80°C aan. Koken door af te koelen — hoe kan dat?

### Hoe werkt dit?
Tijdens het eerste koken wordt de lucht in de fles verdrongen door **waterdamp**. Sluit je de fles en koel je de wand met koud water, dan condenseert die damp razendsnel. De druk in de fles **stort in** (net als bij de vacuümpomp van Demo 1). Door de extreem lage druk kunnen bellen al bij 80°C overleven — het water "kookt" opnieuw.

### Wat heeft dit met Carnot te maken?

- **Druk daalt → kookpunt daalt** — Exact dezelfde pV-relatie als in het Carnot pV-diagram.  
- **Condensatie verlaagt druk** — Het omgekeerde van verdamping; de cyclus $T$ ↑ ↓ $P$ ↑ ↓ zie je hier live.
- **Tweede hoofdwet** — Warmte stroomt van het hete glas naar het koude gietwater — de natuurlijke richting.
- **Carnot-limiet** — Het maximale rendement $\eta = 1 - T_c/T_h$ voel je hier: hoe kouder het gietwater, hoe lager $T_c$, hoe groter het temperatuurverschil.

---

```{admonition} Zelf proberen?
:class: tip

Alle zes demo's zijn klassikaal uit te voeren met eenvoudige materialen. De volledige beschrijvingen (inclusief benodigdheden, stappenplannen, en video's) vind je op [Show the Physics](https://github.com/FreekPols/ShowthePhysics) (CC‑BY‑4.0). Perfect voor een practicumles over thermodynamica!
```