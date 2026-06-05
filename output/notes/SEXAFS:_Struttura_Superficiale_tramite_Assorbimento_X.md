# SEXAFS: Struttura Superficiale tramite Assorbimento X

## Principi Fondamentali

La tecnica SEXAFS (Surface Extended X-Ray Absorption Fine Structure) è basata sull'analisi delle oscillazioni del coefficiente di assorbimento X in funzione dell'energia dei fotoni, al di sopra della soglia di assorbimento. Il coefficiente di assorbimento può essere espresso come:

$$\mu = \mu_0^K(1 + \chi) + \mu_0$$

dove **χ contiene l'informazione strutturale relativa a distanze interatomiche e numeri di coordinazione**.

## Relazione Energia-Vettore d'Onda

Nel processo di fotoeccitazione, l'energia è conservata secondo la relazione:

$$\frac{\hbar^2 k^2}{2m} = \hbar\omega - E_B + V_0$$

dove:
- $E_B$ è l'energia di legame dell'elettrone nello stato iniziale
- $V_0$ è il potenziale interno del solido
- $k$ è il vettore d'onda dell'elettrone fotoeccitato

## Formula EXAFS e Interpretazione Strutturale

La funzione EXAFS χ(k) è descritta dalla formula:

$$\chi(k) = \sum_i A_i(k)\sin\left[2kR_i + \rho_i(k)\right]$$

**Componenti della formula:**
- $R_i$: distanza del guscio di diffusori i-esimo
- $\rho_i(k)$: fase di scattering (dipende dai potenziali dell'atomo assorbitore e diffusore)
- $A_i(k)$: ampiezze EXAFS, proporzionali alle ampiezze di retrodiffusione; incorporano informazioni sulle vibrazioni termiche e sullo smorzamento per scattering anelastico

**Effetti strutturali sulle oscillazioni:**
- Distanze interatomiche minori → massimi di oscillazione a energie più alte (periodo di oscillazione ridotto)
- Numeri di coordinazione maggiori → ampiezze di oscillazione aumentate

## Analisi dei Dati EXAFS

### Metodo Semplice
La distanza $R_i$ può essere stimata dalla separazione energetica $\Delta E$ tra il primo massimo e il primo minimo:

$$R_i[\text{Å}] \approx \left(\frac{151}{\Delta E}\right)^{1/2}$$

### Trasformata di Fourier (Metodo Accurato)
Per un'analisi più precisa, si applica la trasformata di Fourier:

$$F(r) = \frac{1}{\sqrt{2\pi}}\int_{k_{min}}^{k_{max}} \chi(k)\, W(k)\, k^3\, e^{2ikr}\, d(2k)$$

dove:
- **Massimi di |F(r)|** corrispondono alle distanze $R_i$ dei gusci di vicini
- **Fattore $k^3$**: compensa la diminuzione rapida di χ(k) a grandi k
- **Funzione finestra $W(k)$**: smussa χ(k) ai bordi per eliminare bande laterali artificiali

## Sensibilità Superficiale: da EXAFS a SEXAFS

L'EXAFS standard **non è sensibile alla superficie** poiché gli strati superficiali contribuiscono in modo trascurabile all'assorbimento totale.

La sensibilità superficiale si ottiene misurando i **prodotti di diseccitazione**, in particolare:
- **Emissione di elettroni Auger** (metodo SEXAFS)
- Emissione di fotoni X

Il metodo SEXAFS sfrutta il **libero cammino medio limitato degli elettroni** (da pochi Å a ~100 Å per energie comprese tra 20 eV e qualche keV), che conferisce sensibilità selettiva agli strati superficiali. 

**Strumentazione richiesta:**
- Radiazione di sincrotrone (accordabile e ad alta intensità)
- Analizzatore elettronico (es. CMA) per la rivelazione degli elettroni Auger

## Caso Studio: Zolfo su Ni(100)

### Configurazione Sperimentale
Studio SEXAFS dell'adsorbimento di zolfo su Ni(100) con struttura c(2×2) determinata da LEED:
- Misura dello yield Auger (transizione KLL dello S a ~2100 eV)
- Angoli di incidenza: 10°, 45° e 90°

### Risultati Strutturali
La trasformata di Fourier F(r) rivela:

| Picco | Distanza | Interpretazione |
|-------|----------|-----------------|
| A | 2,23 ± 0,02 Å (S–Ni) | Riduzione di 0,16 ± 0,02 Å rispetto al bulk NiS (2,3944 Å) |
| B | 4,15 ± 0,10 Å | Seconda sfera di coordinazione |

### Conclusione Strutturale
L'integrazione di dati SEXAFS con informazioni da LEED e analisi delle intensità e fasi di scattering determina che **l'atomo di zolfo occupa un sito a coordinazione quadrupla**: forma una piramide con base rettangolare costituita da quattro atomi di Ni dello strato superficiale.