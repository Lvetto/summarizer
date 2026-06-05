# Spettroscopia Auger e Analisi Chimica Superficiale

## Spettroscopia Auger (AES)

### Il Processo Auger

La spettroscopia Auger è una tecnica spettroscopica basata su un processo a tre step:

1. Un elettrone primario crea un buco in un livello core dell'atomo
2. Un elettrone da un guscio più esterno riempie il buco, cedendo la sua energia di transizione
3. Un terzo elettrone (elettrone Auger) viene emesso dal sistema con energia cinetica ben definita

A differenza dell'emissione di raggi X, lo stato finale presenta un buco aggiuntivo. L'energia cinetica dell'elettrone Auger è direttamente correlata alle differenze tra le energie dei livelli core, consentendo l'identificazione degli elementi chimici con **alta sensibilità superficiale**.

### Nomenclatura delle Transizioni

La nomenclatura delle transizioni Auger riflette i livelli core coinvolti nel processo:

- **KL₁L₂**: buco iniziale nel guscio K, riempito da L₁, energia trasferita a L₂
- **L₁M₁M₁**: transizione con due buchi finali nello stesso guscio M₁
- **Coster-Kronig**: il buco iniziale è riempito da un elettrone dello stesso guscio
- **L₃VV**: processo in solido che coinvolge la banda di valenza

L'intensità massima si osserva quando i due buchi finali si formano in regioni ad alta densità di stati della banda di valenza.

### Formulazione Energetica

Per il processo KL₁L₂, l'energia dell'elettrone Auger è determinata da:

$$E^Z_{KL_1L_2} = E^Z_K - E^Z_{L_1} - E^Z_{L_2} - \Delta E(L_1L_2)$$

dove il termine correttivo ΔE tiene conto degli effetti di rilassamento multi-elettronico:

$$\Delta E(L_1L_2) = \frac{1}{2}\left[(E^{Z+1}_{L_2} - E^Z_{L_2}) + (E^{Z+1}_{L_1} - E^Z_{L_1})\right]$$

Le energie XPS dell'elemento e dell'elemento con numero atomico Z+1 permettono il calcolo empirico di queste correzioni.

### Caratteristiche Generali

- Gli elementi con meno di 3 elettroni non possono subire transizioni Auger
- Le energie Auger dipendono fortemente da Z (numero atomico)
- Le tre principali classi di transizioni sono: **KLL, LMM e MNN**
- Variazioni entro ogni gruppo derivano da diverse orientazioni di spin nello stato finale

### Meccanismo Fisico

La probabilità di transizione Auger è determinata principalmente dall'**interazione Coulombiana** tra due elettroni:

$$W_{KLL} \propto \left|\left\langle \psi_{1s}(r_1)e^{ik\cdot r_2}\left|\frac{e^2}{|r_1-r_2|}\right|\psi_{2s}(r_1)\psi_{2p}(r_2)\right\rangle\right|^2$$

A differenza delle transizioni radiative, i processi Auger:
- Hanno probabilità approssimativamente indipendente da Z
- Non obbediscono alle regole di selezione del dipolo (es. KL₁L₁ è opticamente proibito)

### Strumentazione

L'apparato AES standard comprende:

- **Cannone elettronico**: fornisce un fascio primario di 2000-5000 eV
- **Analizzatori energetici**: Cylindrical Mirror Analyser (CMA) o emisferico per la selezione energetica
- Il CMA è spesso integrato con il cannone sull'asse centrale, utile per il depth profiling

### Modalità di Rivelazione Derivata

Per supprimere il grande background di elettroni secondari veri, AES opera in **modalità derivata**. Una piccola tensione alternata v = v₀sin(ωt) viene sovrapposta alla tensione dell'analizzatore:

$$I(V + v_0\sin\omega t) \approx I_0 + \frac{dI}{dv}v_0\sin\omega t$$

In questa modalità, le energie Auger sono definite dalla **posizione del minimo dello spettro derivato dN/dE**, non dal massimo dello spettro non-differenziato. Questo consente una migliore risoluzione energetica e una riduzione del rumore di fondo.

---

## Secondary Ion Mass Spectroscopy (SIMS)

### Configurazione Strumentale

La SIMS utilizza un'apparecchiatura composta da:

- Sorgente ionica (camera di ionizzazione e sistema di lenti)
- Separatore magnetico di massa (analizzatore a settore)
- Camera a ultra-alto vuoto contenente il campione
- Spettrometro di massa a quadrupolo (QMS) con rivelatore a channeltron

### Spettrometro di Massa a Quadrupolo (QMS)

Il QMS contiene quattro barre quadrupolari polarizzate con una sovrapposizione di tensione DC (U) e componente AC (V cos ωt, tipicamente 1 MHz). Il potenziale elettrico è:

$$\varphi(x,y,t) = \frac{1}{r_0^2}(U + V\cos\omega t)(x^2 - y^2)$$

dove r₀ è il raggio delle barre (≈5 mm).

Le equazioni del moto per uno ione positivo sono:

$$\begin{pmatrix}\ddot{x}\\\ddot{y}\\\ddot{z}\end{pmatrix} = \frac{2q}{mr_0^2}(U + V\cos\omega t)\begin{pmatrix}-x\\y\\0\end{pmatrix}$$

**Principio di separazione di massa**: Gli ioni pesanti non riescono a seguire il campo ad alta frequenza e subiscono oscillazioni armoniche stabili nella direzione x, ma movimento illimitato nella direzione y (scaricati dalle barre). Gli ioni leggeri seguono il campo AC dominante e oscillano stabilmente attorno all'asse centrale. La separazione si ottiene mantenendo costante il rapporto V/U ≈ 6 durante la scansione delle tensioni.

La trasmittanza del QMS dipende dalla massa; pertanto è necessaria la calibrazione mediante miscele di gas inerti ben definite.

### Processo di Sputtering

L'energy transfer dal fascio di ioni primari agli atomi del substrato avviene tramite cascata di collisioni a due corpi. Si distinguono tre regimi:

1. **Single-knock-on regime** (E < 1 keV): gli atomi rimossi ricevono energia sufficiente per lo sputtering, senza generare cascate di rinculo
2. **Linear-cascade regime** (1 keV – 1 MeV): gli atomi di rinculo generano ulteriori rimbalzi a bassa densità
3. **Spike regime** (ioni pesanti ad alta energia): alta densità di atomi in movimento in un volume limitato

### Parametri Quantitativi dello Sputtering

La **yield di sputter** Y (numero di particelle sputtered per ione incidente) governa il processo:

$$-dN = NYv_{\text{atom}}A\,dt$$

dove A è l'area superficiale colpita dal fascio.

Per uno strato adsorbito con copertura θ(t) = N(t)/N_max:

$$N(t) = N_{\text{max}}\exp\left(-\frac{Yj_{\text{PI}}}{eN_{\text{max}}}t\right)$$

La **lifetime media** di un atomo superficiale è:

$$\tau = \frac{eN_{\text{max}}}{Yj_{\text{PI}}}$$

A densità di corrente di 10⁻⁴ e 10⁻⁹ A/cm², le lifetime sono rispettivamente 0.3 s e 9 h, corrispondenti a 3 e 3×10⁻⁵ monostrati rimossi al secondo.

### Ionizzazione dei Secondari

La maggior parte dei secondari è emessa come neutra (< 5% ionizzati per superfici metalliche pulite). L'ionizzazione dipende dall'interazione complessa tra particella emessa e superficie. L'analisi SIMS pratica si basa su dati empirici di yield di sputter e sezioni d'urto di ionizzazione.

### Static SIMS vs Dynamic SIMS

**Static SIMS** (densità di corrente 10⁻⁹–10⁻¹⁰ A/cm²):
- Sputtering rate: 10⁻⁴–10⁻⁵ monostrati/s
- Distruzione superficiale minima
- Applicazioni: composizione superficiale, processi di adsorbimento, reazioni chimiche superficiali
- Sensibilità: detection limit ~10⁻⁶ monostrati (superiore di ordini di grandezza rispetto alle spettroscopie elettroniche)
- Corrente di ioni secondari: ISI(M) = I_PI Y α η θ_M

**Dynamic SIMS** (densità di corrente 10⁻⁴–10⁻⁵ A/cm²):
- Sputtering rate: diversi monostrati/s
- Utilizzata per depth profiling e analisi della composizione in profondità
- Risoluzione di profondità limitata da smearing dei segnali da più strati atomici
- Richiede ottimizzazione della sputtering rate per bilanciare risoluzione di profondità e profondità massima di erosione