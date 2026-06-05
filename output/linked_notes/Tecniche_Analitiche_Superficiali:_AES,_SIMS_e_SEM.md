# Tecniche Analitiche Superficiali: [[AES, SIMS e SEM]]

## Auger Electron Spectroscopy (AES)

### Il Processo Auger

L'[[AES, SIMS e SEM|AES]] si basa sul **processo Auger**, un meccanismo di de-eccitazione atomica a tre elettroni:
1. Un elettrone primario crea una lacuna in un livello di core
2. Un elettrone da un guscio esterno riempie la lacuna, liberando energia
3. Questa energia viene trasferita a un terzo elettrone, che viene emesso come **elettrone Auger** con energia cinetica ben definita

Diversamente dall'emissione X, lo stato finale dell'atomo risulta più ionizzato (due lacune invece di una). L'energia caratteristica dell'elettrone Auger, legata alle differenze tra livelli di core, permette l'**analisi chimica degli elementi** con elevata sensibilità superficiale.

### Nomenclatura e Transizioni

Le transizioni Auger sono denominate in base ai livelli coinvolti (es. **KL₁L₂**: lacuna iniziale in K, riempita da L₁, elettrone emesso da L₂). Tra le varianti notevoli:
- **Transizioni Coster-Kronig**: la lacuna è riempita da un elettrone dello stesso guscio
- **L₃VV**: coinvolge la banda di valenza; massima intensità in regioni ad alta densità di stati

### Calcolo dell'Energia Auger

Per il processo KL₁L₂:

$$E^Z_{KL_1L_2} = E^Z_K - E^Z_{L_1} - E^Z_{L_2} - \Delta E(L_1L_2)$$

Il termine correttivo $\Delta E$ tiene conto degli effetti a molti elettroni:

$$\Delta E(L_1L_2) = \frac{1}{2}\left[(E^{Z+1}_{L_2} - E^Z_{L_2}) + (E^{Z+1}_{L_1} - E^Z_{L_1})\right]$$

Questo approccio fornisce risultati molto accurati (scarto sperimentale < 2%).

### Probabilità di Transizione

L'interazione determinante è quella **Coulombiana** tra l'elettrone che riempie la lacuna e quello emesso. Due caratteristiche fondamentali:
- La probabilità di transizione Auger è **sostanzialmente indipendente da Z**, diversamente dalle transizioni radiative
- Le transizioni Auger **non obbediscono alle regole di selezione di dipolo**, permettendo transizioni otticamente vietate (es. KL₁L₁)

### Strumentazione e Rilevazione

**Componenti principali:**
- Cannone elettronico con energia primaria: 2000–5000 eV
- Analizzatore emisferico o **Cylindrical Mirror Analyser (CMA)**, spesso con cannone integrato sull'asse centrale

**Modalità derivativa:** Poiché il segnale Auger è piccolo rispetto al fondo di elettroni secondari, si utilizza una tensione alternata sovrapposta ($v = v_0\sin\omega t$) e si misura **dN/dE** con un lock-in amplifier. Le energie Auger sono riportate come **posizione del minimo** dello spettro derivato (non corrisponde al massimo del picco non derivato).

### Caratteristiche Analitiche

- Atomi con meno di 3 elettroni non possono subire transizioni Auger
- Le energie Auger seguono tre rami principali: **KLL, LMM, MNN**
- La forte dipendenza da Z delle energie di legame rende l'AES efficace per l'**analisi elementale superficiale**
- Combinata con [[Preparazione di Superfici: Clivaggio, Bombardamento Ionico e Ricottura|sputtering ionico]], consente la **profilazione in profondità**

---

## Secondary Ion Mass Spectroscopy (SIMS)

### Principio di Funzionamento

La [[AES, SIMS e SEM|SIMS]] utilizza un fascio di ioni primari per bombardare la superficie del campione in camera [[Tecnologia dell'Ultravuoto (UHV) e Misura della Pressione|UHV]]. Il processo di sputtering rimuove atomi superficiali (come neutri o ioni secondari), che vengono analizzati da uno **Spettrometro di Massa a Quadrupolo (QMS)**.

### Quadrupole Mass Spectrometer (QMS)

Il QMS consiste di quattro barre quadrupolari polarizzate a coppie con una sovrapposizione di tensione DC ($U$) e componente AC ($V\cos\omega t$, $\omega/2\pi \approx 1$ MHz):

$$\phi(x,y,t) = \frac{1}{r_0^2}(U + V\cos\omega t)(x^2 - y^2)$$

Le equazioni del moto degli ioni generano soluzioni di tipo **Mathieu**:
- **Ioni pesanti**: non seguono il campo ad alta frequenza; oscillano stabilmente in x ma hanno moto illimitato in y → colpiscono gli elettrodi
- **Ioni leggeri**: seguono il campo AC dominante; il campo AC li mantiene verso l'asse con oscillazione stabile

Per $V/U \approx 6$, la finestra di trasmissione contiene una sola massa. Per acquisire uno spettro completo, $V$ e $U$ vengono variati simultaneamente mantenendo il rapporto costante. La trasmittanza dipende dalla massa (richiede calibrazione con gas inerti).

### Il Processo di Sputtering

L'energia viene trasferita tramite una **cascata di collisioni a due corpi**. Si distinguono tre regimi:

| Regime | Energia primaria | Caratteristica |
|---|---|---|
| **Single knock-on** | < 1 keV | Rinculo singolo senza cascate ulteriori |
| **Linear cascade** | 1 keV – 1 MeV | Densità di rinculo bassa, cascate multiple |
| **Spike** | Ioni pesanti ad alta E | Densità di atomi in moto elevata |

### Resa di Sputtering

La **resa di sputtering** $Y$ (particelle sputtered per ione incidente) determina la velocità di rimozione:

$$-dN = NY\nu A\, dt$$

La **vita media** di un atomo superficiale è:

$$\tau = \frac{eN_{max}}{Yj_{PI}}$$

Esempi pratici:
- $j_{PI} = 10^{-4}$ A/cm²: $\tau \approx 0.3$ s (3 monostrati/s rimossi)
- $j_{PI} = 10^{-9}$ A/cm²: $\tau \approx 9$ h ($3\times10^{-5}$ monostrati/s rimossi)

### Ionizzazione delle Particelle Secondarie

Le particelle secondarie sono emesse **prevalentemente come neutri** (< 5% ionizzate per metalli puliti). Il grado di ionizzazione dipende da complesse interazioni con la superficie e aumenta drasticamente in presenza di ossido (fino a ×1000).

### SIMS Statica vs. Dinamica

**SIMS Statica:**
- Corrente primaria: $j_{PI} \sim 10^{-9}$–$10^{-10}$ A/cm²
- Tasso di sputtering: $10^{-4}$–$10^{-5}$ monostrati/s → distruzione minima
- Studia il **singolo strato atomico superficiale**
- Corrente ionica secondaria: $I_{SI}(M) = I_{PI} Y \alpha \eta \theta_M$ (dove $\alpha$ è il grado di ionizzazione, $\eta$ la trasmissività)
- **Limite di rilevazione**: fino a $10^{-6}$ monostrati → sensibilità superiore di ordini di grandezza rispetto ad AES, UPS, XPS

**SIMS Dinamica:**
- Corrente primaria: $j_{PI} \sim 10^{-4}$–$10^{-5}$ A/cm²
- Tasso di sputtering: diversi monostrati/s
- Utilizzata per **profilazione in profondità**
- Tempo di erosione convertibile in scala di profondità
- Velocità elevata di sputtering limita la risoluzione in profondità

---

## Scanning Electron Microscopy (SEM)

### Principio di Funzionamento

Un fascio di [[Ottica delle Particelle, Lenti e Analizzatori di Energia|elettroni]] primari (energia E₀) viene scansionato sulla superficie del campione. L'intensità degli elettroni emessi modula l'intensità di un tubo TV, formando un'immagine.

### Distribuzione Energetica degli Elettroni Emessi

La superficie irradia quattro categorie di elettroni:

- **Regione I** – Elettroni elasticamente retrodiffusi (energia E₀)

- **Regione II** – Elettroni inelasticamente retrodiffusi con struttura spettrale dovuta a perdite per eccitazione di plasmoni e transizioni interbanda (specifiche per ogni solido). Il **rivelatore BE** produce immagini ad alto contrasto chimico, ma con forti effetti di ombreggiamento dovuti all'elevato forward scattering.

- **Regione III** – Zona piatta (tra Regione II e ~50 eV). Con amplificazione appropriata e modalità derivata (dN/dE), si rilevano le **righe Auger**, caratteristiche di ogni elemento.

- **Regione IV** – 0–50 eV, banda intensa dei **veri elettroni secondari**, originati da molteplici eventi di scattering. Il **rivelatore SE** produce immagini topografiche con minor contrasto chimico ma evidenzia variazioni di rugosità e funzione lavoro.

### Modalità di Imaging e Contrasto

- **Detector BE** → Contrasto chimico elevato, effetti di ombreggiatura pronunciati
- **Detector SE** → Topografia superficiale, contrasto chimico minore, ombreggiatura ridotta
- **Corrente totale del campione** → Topografia con contrasto invertito rispetto a SE

L'interpretazione richiede attenzione: il contrasto è influenzato sia da fattori geometrici (inclinazione dei piani) sia elettronici (variazioni di funzione lavoro).

### Tecniche di Microsonda

Il fascio primario induce anche:
- **Emissione di elettroni Auger** → rilevati con analizzatore elettronico (es. CMA) per analisi chimica risolta spazialmente
- **Emissione di raggi X caratteristici** → rilevati con rivelatori energy-dispersive per analisi elementale

### Profondità di Informazione

Le tecniche di microsonda differiscono significativamente nella profondità di provenienza del segnale:

| Segnale | Profondità di Informazione |
|---|---|
| Raggi X caratteristici | 0.1–10 µm |
| Elettroni Auger | 10²–10⁴ volte inferiore rispetto ai raggi X |
| Elettroni secondari/Auger | Collo stretto della zona a pera superficiale |
| Elettroni retrodiffusi e raggi X | Corpo della zona a pera sottosuperficiale |

La regione sorgente ha tipicamente forma di pera: i segnali superficiali provengono dal collo stretto superiore, i segnali profundi dal corpo della pera.

### Sviluppi Strumentali

I SEM standard operano in alto vuoto (~10⁻⁵ Pa). Sono stati sviluppati **SEM in condizioni [[Tecnologia dell'Ultravuoto (UHV) e Misura della Pressione|UHV]]**, collegabili tramite camere load-lock ad altre apparecchiature UHV, permettendo indagini **in situ** dopo la [[Preparazione di Superfici: Clivaggio, Bombardamento Ionico e Ricottura|preparazione superficiale]] senza esposizione all'aria.