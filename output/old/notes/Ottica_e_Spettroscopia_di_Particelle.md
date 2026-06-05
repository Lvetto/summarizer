# Ottica e Spettroscopia di Particelle

## Lenti Elettrostatiche

Le lenti elettrostatiche utilizzano campi elettrici non omogenei per focalizzare fasci di particelle cariche, sfruttando configurazioni di elettrodi metallici che curvano le linee equipotenziali senza richiedere materiali fisici.

### Configurazione e Focussing

Le lenti a tre aperture metalliche generano effetti focussing o defocussing in base alla distribuzione potenziale. Una configurazione simmetrica focalizza gli elettroni quando il potenziale dell'elettrodo centrale è inferiore alle estremità, rallentando le particelle nella regione centrale dove predomina l'effetto focussing.

### Lunghezza Focale

La lunghezza focale inversa per lenti con equipotenziali curve è data da:

$$\frac{1}{f} = \frac{1}{2(U_2)^{1/2}} \int_{x_1}^{x_2} \frac{1}{r(x)} \frac{U'(x)}{\sqrt{U(x)}} dx$$

dove l'indice di rifrazione per gli elettroni è:

$$n(x) = \frac{\sqrt{U(x)}}{\sqrt{U_2}}$$

### Proprietà Universale

Una proprietà fondamentale è che il rapporto e/m non entra nelle condizioni di focussing. Questo significa che particelle diverse (elettroni, protoni, ioni He⁺) vengono fuocate nello stesso punto con gli stessi potenziali applicati, a patto che entrino con la medesima energia cinetica primaria.

---

## Lenti Magnetiche

Le lenti magnetiche sfruttano la curvatura delle traiettorie di particelle cariche in campi magnetici, producendo effetti focussing mediante solenoidi e configurazioni di ferro schermato.

### Dinamica delle Particelle

Un elettrone che entra in un solenoide con velocità v ad angolo φ rispetto al campo B segue una traiettoria elicoidale, decomponibile in:
- **Componente parallela**: $v_\parallel = v\cos\phi$ (non accelerata)
- **Componente perpendicolare**: $v_\perp = v\sin\phi$ (moto circolare con frequenza angolare)

La frequenza angolare di rotazione è:

$$\omega = \frac{e}{m}B$$

### Convergenza e Focussing

Gli elettroni provenienti da un punto A che entrano a diversi angoli convergono nel punto C dopo un tempo:

$$\tau = \frac{2\pi m}{eB}$$

La distanza di focussing è:

$$AC = v_\parallel \tau = \frac{2\pi m v \cos\phi}{eB}$$

### Differenze dalle Lenti Elettrostatiche

A differenza delle lenti elettrostatiche, le lenti magnetiche presentano due caratteristiche distintive:
- La condizione di focussing dipende dal rapporto e/m
- L'immagine risulta ruotata rispetto all'oggetto

---

## Analizzatori di Energia per Elettroni

### Analizzatore Cilindrico

L'analizzatore cilindrico utilizza due settori cilindrici come elettrodi per selezionare gli elettroni in base all'energia.

**Geometria e Campo**: Gli elettroni seguono un percorso circolare centrale dove la forza centrifuga è bilanciata dalla forza elettrostatica. Il campo è logaritmico-radiale:

$$E = -\frac{U_p}{r\ln(b/a)}$$

dove a e b sono i raggi interno ed esterno.

**Energia di Passaggio**: Sulla traiettoria centrale, l'equilibrio delle forze fornisce:

$$E_0 = \frac{1}{2}mv_0^2 = \frac{1}{2}\frac{eU_p}{\ln(b/a)}$$

**Focussing**: Per piccole deviazioni dalla traiettoria centrale, la deflessione oscilla con periodo proporzionale a $\omega_0$. Il focussing si verifica con angolo di rotazione:

$$\phi = 127°17'$$

Con aperture di correzione (Herzog apertures), questo valore diventa 118.6°.

### Risoluzione Energetica

La risoluzione energetica relativa è:

$$\frac{\Delta E}{E} = \frac{x_1 + x_2}{r_0} + \frac{4}{3}\alpha^2 + \beta^2$$

dove $x_1, x_2$ sono larghezza e lunghezza delle fenditure, mentre α e β sono deviazioni angolari massime.

### Effetti di Space-Charge

A densità di corrente elevata, la repulsione coulombiana e il campo magnetico indotto distorcono le traiettorie. La densità di corrente varia come:
- **Al passaggio**: $j_i \propto E_0^{3/2} \propto (\Delta E)^{3/2}$
- **All'uscita**: $j_f \propto (\Delta E)^{5/2}$

Questo causa forte riduzione della corrente trasmessa con fenditure più strette, limitando la possibilità di migliore risoluzione.

### Modalità di Funzionamento

- **Costante ΔE/E**: Scansione del voltaggio di passaggio; la risoluzione cambia con l'energia
- **Costante ΔE**: Energia di passaggio fissa; variazione di voltaggio di accelerazione/decelerazione prima dell'analizzatore per misurare diverse energie

### Spettrometro Completo (HREELS)

Un spettrometro per High-Resolution Electron Energy Loss Spectroscopy comprende:
- **Filamento catodico** con sistema di lenti (distribuzione Maxwell 0.3-0.5 eV)
- **Primo monocromatore** (analizzatore cilindrico a pass energy costante) che seleziona finestra 1-10 meV
- **Sistema di lenti** focussante il fascio sul campione
- **Secondo analizzatore** (modo costante ΔE) per gli elettroni retrodiffusi
- **Rivelatore** (tazza di Faraday o channeltron)

### Analizzatore Emisferico

Costituito da due emisferi metallici concentrici, il focussing avviene a 180° di deflessione. La risoluzione è:

$$\frac{\Delta E}{E} = \frac{x_1 + x_2}{2r} + \alpha^2$$

dove $r = \frac{a+b}{2}$.

### Cylindrical Mirror Analyzer (CMA)

Utilizza due elettrodi cilindrici concentrici con focussing per elettroni che entrano in un cono con angolo di apertura:

$$\phi = 42°18.5'$$

L'energia di passaggio è:

$$E_0 = \frac{eU_p}{0.77\ln(b/a)}$$

La risoluzione dipende da deviazione angolare α e spostamenti assiali:

$$\frac{\Delta l}{l_0} = \frac{\Delta E}{E}(1 + 1.84\alpha) - 2.85\alpha^2$$

Varianti a doppio stadio consentono misure con risoluzione angolare mediante rotazione di aperture di selezione.

---

## Surface Extended X-Ray Absorption Fine Structure (SEXAFS)

### Principi dell'EXAFS

Il coefficiente di assorbimento dei raggi X contiene informazioni strutturali attraverso la funzione:

$$\mu = \mu_0^K(1 + \chi) + \mu_0$$

dove χ contiene lunghezze di legame e numeri di coordinazione. L'energia del fotoelettrone eccitato è:

$$\frac{\hbar^2k^2}{2m} = \hbar\omega - E_B + V_0$$

### Meccanismo EXAFS

La struttura fine dell'assorbimento origina dall'interferenza tra l'onda fotoelettronica in uscita e le onde retrodiffuse dai vicini atomici:

$$\chi(k) = \sum_i A_i(k)\sin\left(2kR_i + \rho_i(k)\right)$$

dove:
- $R_i$ è la distanza dei vicini atomici
- $A_i(k)$ sono le ampiezze di retrodiffusione
- $\rho_i(k)$ è la fase di scattering
- Il fattore $2R_i$ riflette il percorso di andata e ritorno del fotoelettrone

Distanze minori producono oscillazioni a frequenze più alte; maggior numero di scatteratori aumenta l'ampiezza.

### Analisi dei Dati

L'analisi prevede:
1. Sottrazione del background monotono $\mu_0^K$
2. Amplificazione e registrazione dell'oscillazione χ
3. Trasformata di Fourier con finestra:

$$F(r) = \frac{1}{\sqrt{2\pi}}\int_{k_{min}}^{k_{max}} \chi(k)W(k)k^3 e^{2ikr}d(2k)$$

I massimi in F(r) corrispondono alle distanze dei gusci atomici vicini.

### Sensibilità Superficiale (SEXAFS)

L'EXAFS convenzionale non è sensibile alla superficie. La tecnica diventa superficiale (SEXAFS) misurando gli **elettroni Auger** emessi dal processo di fotoionizzazione, anziché l'assorbimento diretto. La sensibilità superficiale deriva dal libero cammino medio limitato degli elettroni Auger (pochi Ångström a ~100 Å, dipendente dall'energia).

### Apparato Sperimentale

Richiede:
- Sorgente di raggi X sincrotonici ad alta intensità e accordabile
- Analizzatore CMA (Cylindrical Mirror Analyzer)
- Finestra energetica tipicamente 20-100 eV per massima sensibilità superficiale
- Radiazione sincrotorone polarizzata

### Esempio: Adsorbimento di Zolfo su Ni(100)

La trasformata di Fourier rivela due picchi principali:
- **Picco A** (2.23 ± 0.02 Å): distanza S–Ni, 0.16 Å inferiore al bulk NiS
- **Picco B** (4.15 ± 0.10 Å): distanza del secondo vicino

La struttura superficiale c(2×2) osservata in LEED, combinata con le intensità dei picchi, indica che lo zolfo occupa un sito con coordinazione quattro (piramidale), con base rettangolare formata da quattro atomi di Ni dello strato superficiale.