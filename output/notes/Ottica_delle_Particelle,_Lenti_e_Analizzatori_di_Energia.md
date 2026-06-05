# Ottica delle Particelle, Lenti e Analizzatori di Energia

## Lenti Elettrostatiche

### Principio di Funzionamento

Le lenti elettrostatiche sfruttano la curvatura delle superfici equipotenziali create da aperture metalliche a potenziali diversi. Il moto degli elettroni segue le linee equipotenziali in campi elettrici non omogenei.

Una **lente simmetrica a tre aperture** produce sempre un effetto focalizzante, indipendentemente dalla polarità dell'elettrodo centrale:
- Con **potenziale negativo**: l'elettrone rallenta al centro, permanendovi più a lungo (effetto focalizzante)
- Con **potenziale positivo**: l'elettrone rallenta alle estremità, dove prevale la deflessione verso l'asse (effetto comunque focalizzante)

### Lunghezza Focale

La lunghezza focale delle lenti elettrostatiche segue un'analogia con l'ottica geometrica:

$$\frac{1}{f} = \frac{1}{2(U_2)^{1/2}} \int_{x_1}^{x_2} \frac{1}{r(x)} \frac{U'(x)}{[U(x)]^{1/2}} dx$$

dove:
- $r(x)$ è il raggio di curvatura delle equipotenziali
- $U(x)$ è il potenziale elettrico
- L'indice di rifrazione per gli elettroni è $n(x) = v(x)/v_1 \propto [U(x)]^{1/2}$

### Proprietà Fondamentale

Poiché il rapporto $e/m$ non compare nelle condizioni di focalizzazione, le lenti elettrostatiche focalizzano nello stesso punto sia **elettroni che ioni positivi** (protoni, He⁺, ecc.), purché abbiano la stessa energia cinetica iniziale e la stessa geometria di ingresso.

---

## Lenti Magnetiche

### Principio di Funzionamento

Gli elettroni in un solenoide con campo magnetico **B** seguono traiettorie elicoidali. La frequenza angolare ciclotronico è:

$$\omega = \frac{e}{m}B$$

Il periodo di rotazione $\tau = 2\pi m / eB$ è **indipendente dall'angolo di inclinazione** rispetto a **B**.

### Distanza di Focalizzazione

$$AC = v_\parallel \tau = \frac{2\pi m v \cos\varphi}{eB}$$

### Differenze dalle Lenti Elettrostatiche

A differenza delle lenti elettrostatiche:
- La focalizzazione **dipende dal rapporto $e/m$**, quindi varia per particelle di massa o carica diverse
- L'immagine risulta **ruotata** rispetto all'oggetto
- Le lenti magnetiche sono preferite per particelle ad alta energia

---

## Analizzatori di Energia Elettrostatici

### Analizzatore a Settori Cilindrici

#### Configurazione e Energia di Pass

Il cilindrical sector analyzer bilancia la forza centrifuga con il campo elettrico radiale logaritmico tra due settori cilindrici concentrici:

$$E = -\frac{U_p}{r \ln(b/a)}$$

L'energia selezionata (energia di pass) è:

$$E_0 = \frac{1}{2}mv_0^2 = \frac{1}{2} \frac{eU_p}{\ln(b/a)}$$

#### Proprietà di Focalizzazione

La focalizzazione si verifica per settori con angolo di **127°17'** (corretto a **118.6°** con le aperture di Herzog).

#### Risoluzione Energetica

$$\frac{\Delta E}{E} = \frac{x_1 + x_2}{r_0} + \frac{4}{3}\alpha^2 + \beta^2$$

dove:
- $x_1, x_2$ sono le larghezze delle fenditure di ingresso/uscita
- $\alpha$ e $\beta$ sono le deviazioni angolari massime nel piano e perpendicolarmente ad esso

Le migliori strumentazioni raggiungono risoluzioni di $\Delta E / E \sim 10^{-3}$–$10^{-4}$.

#### Effetto della Carica Spaziale

La densità di corrente trasmessa scala come $j_f \propto (\Delta E)^{5/2}$, limitando fortemente la corrente all'aumentare della risoluzione (diminuendo $\Delta E$).

#### Modalità Operative

- **Constant $\Delta E/E$ mode**: scansione della tensione di pass $U_p$; la risoluzione assoluta $\Delta E$ varia con l'energia
- **Constant $\Delta E$ mode**: tensione di pass fissa; lo spettro viene traslato variando una tensione di accelerazione/decelerazione prima dell'analizzatore

---

### Spettrometro HREELS

Lo spettrometro per High-Resolution Electron Energy Loss Spectroscopy (HREELS) è un sistema integrato composto da:

1. **Sorgente elettronica**: catodo + sistema di lenti (larghezza energetica 0.3–0.5 eV)
2. **Monocromatore**: analizzatore cilindrico a energia di pass fissa che seleziona una finestra energetica di 1–10 meV
3. **Sistema di lenti**: focalizzazione sul campione
4. **Analizzatore**: in modalità $\Delta E$ costante per gli elettroni retrodiffusi
5. **Rivelatore**: channeltron o coppa di Faraday

---

### Analizzatore Emisferico

#### Configurazione

Utilizza due elettrodi semisferici concentrici. La focalizzazione avviene per elettroni deflessi di **180°**.

#### Risoluzione

$$\frac{\Delta E}{E} = \frac{x_1 + x_2}{2r} + \alpha^2$$

dove:
- $x_1, x_2$ sono i raggi delle aperture circolari di ingresso/uscita
- $r = (a+b)/2$ è il raggio medio (con $a$ e $b$ raggi delle sfere)
- $\alpha$ è la deviazione angolare massima

---

### Analizzatore a Specchio Cilindrico (CMA)

#### Configurazione e Energia di Pass

Il Cylindrical Mirror Analyzer utilizza due elettrodi cilindrici concentrici. La focalizzazione si verifica per elettroni che entrano in un cono con angolo al vertice $\varphi = 42°18.5'$.

L'energia di pass è:

$$E_0 = \frac{eU_p}{0.77 \ln(b/a)}$$

#### Risoluzione

$$\frac{l}{l_0} = \frac{\Delta E}{E}(1 + 1.84\alpha) - 2.85\alpha^2$$

dove i termini lineari e quadratici in $\alpha$ (deviazione angolare massima) descrivono come la risoluzione deteriora con l'apertura angolare.

#### Applicazioni

Il CMA è particolarmente diffuso in **Spettroscopia Auger (AES)**. Esiste anche una versione a **doppio stadio** (double CMA) per migliori prestazioni.