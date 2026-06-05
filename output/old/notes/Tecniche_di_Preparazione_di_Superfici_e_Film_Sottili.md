# Tecniche di Preparazione di Superfici e Film Sottili

## Frattura in Ultra Alto Vuoto (Cleavage in UHV)

### Principi Fondamentali
La frattura controllata è una tecnica per ottenere superfici ben definite mediante rottura cristallografica controllata. Tuttavia, è applicabile solo a materiali fragili con struttura cristallina regolare.

### Materiali Idonei e Limitazioni
- **Materiali fragili**: Alogenuri alcalini (NaCl, KCl), ossidi (ZnO, TiO₂, SnO₂) e semiconduttori (Ge, Si, GaAs)
- La frattura è possibile solo lungo **direzioni cristallografiche specifiche** dipendenti dalla geometria e dalla natura del legame chimico
- Per cristalli ionici: determinanti sono il numero di legami covalenti tagliati e la compensazione dei campi elettrici nel piano di frattura

### Piani di Frattura per Diverse Strutture

| Materiale | Struttura | Piani di Frattura | Caratteristiche |
|-----------|-----------|-------------------|-----------------|
| Alogenuri alcalini | Cubica | {100} non polari | Frattura controllata |
| ZnO | Wurtzite | {1010} prismatici | Qualità superiore; {0001} polari danno più difetti |
| Si, Ge | Cubica | {111} | Unica direzione possibile |
| GaAs, InP, GaP | Cubica | {110} non polari | Carica ionica bilanciata |

### Ottimizzazione nei Semiconduttori III-V
Per superfici (110) di qualità ottimale, l'orientazione del campione è critica. L'**orientazione B** risulta più favorevole perché presenta una sola probabilità di frattura indesiderata significativa (γ = ±30°), mentre altre orientazioni mostrano multiple direzioni di frattura concorrenti. La probabilità di frattura lungo piani indesiderati dipende dall'angolo γ tra le normali ai diversi piani: valori minori di γ indicano probabilità di frattura più elevate.

---

## Bombardamento Ionico e Annealing Termico

### Bombardamento Ionico (Ion Bombardment)
Il bombardamento ionico è un processo in cui ioni ad alta energia colpiscono la superficie del materiale, causando:
- **Rimozione di atomi superficiali** (sputtering)
- **Modificazione della struttura superficiale**
- **Introduzione di danni reticolari** e difetti
- Utilizzo in pulizia, incisione e modifica controllata di superfici

### Annealing (Ricottura Termica)
Il trattamento termico ad alta temperatura consente:
- **Aumento della mobilità atomica** mediante riscaldamento
- **Riconfigurazione atomica** in posizioni più stabili
- **Riparazione dei danni** reticolari causati dal bombardamento
- **Riduzione delle tensioni interne** e ricristallizzazione
- **Miglioramento della qualità cristallina**

### Applicazione Sequenziale
Questi processi sono frequentemente utilizzati in combinazione:
1. **Bombardamento ionico**: modificazione/pulizia della superficie
2. **Annealing**: ripristino della qualità strutturale e eliminazione dei difetti

Questa sequenza è ampiamente impiegata in scienza dei materiali, microelettronica e produzione di dispositivi a semiconduttore.

---

## Evaporazione e Molecular Beam Epitaxy (MBE)

### Evaporazione di Film Sottili
L'evaporazione consente la sublimazione controllata di materiali mediante bilancia al quarzo. Per prevenire contaminazioni oltre il limite di rilevazione AES, la pressione di fondo deve essere **≤ 10⁻⁹ Torr**. I film ottenuti sono generalmente **policristallini o amorfi**, limitando gli studi cristallografici specifici, sebbene permettano ricerche su adsorbimento e barriere Schottky.

### Molecular Beam Epitaxy (MBE)
Quando i film sublimati sono **monocristallini**, il processo è denominato MBE. Esistono due varianti:
- **Homoepitassia**: substrato e film dello stesso materiale
- **Eteroepitassia**: substrato e film di materiali diversi

#### Vantaggi di MBE
- Superfici epitassiali pulite, monocristalline, stoichiometria controllabile
- Poche limitazioni sul tipo cristallografico
- **Versatilità**: applicabile a semiconduttori elementari (Si, Ge) e composti (III-V come GaAs, InP; II-VI come CdTe)
- Crescita controllata di film con profili di doping netti
- Strutture multistrato con doping alternato (n-i-p-i) o bandgap alternato (GaAs-GaAlAs)
- "Tailoring" di materiali semiconduttori a livello atomico

#### Configurazione Sperimentale
Una camera UHV tipica contiene:
- **Celle di effusione Knudsen**: cruciboli in nitruro di boro (BN) pirolitico o grafite, riscaldati da avvolgimenti di tantalio
- **Schermi criogenici**: raffreddati a N₂ liquido per ridurre impurità
- **Spettrometro di massa**: monitoraggio dei flussi dalle sorgenti
- **RHEED**: monitoraggio in situ della struttura cristallografica durante la crescita
- Substrato riscaldabile a ~700°C; crescita omoepitassiale di GaAs a 500-600°C

#### Controllo RHEED e Oscillazioni
Le **oscillazioni RHEED** forniscono controllo layer-by-layer della superficie in crescita:
- I massimi indicano il completamento di strati atomici completi
- Il conteggio dei massimi monitora il numero di strati depositati
- Consente misure di spessore a scala atomica
- L'eccesso di Ga o As produce punti di ordine non-integrale nel pattern di diffrazione

#### Crescita Omoepitassiale di GaAs

**Formula del flusso molecolare da cella Knudsen:**

$$F = \frac{P(T)a}{L^2\sqrt{2\pi mKT}} \quad [1/(s \cdot cm^2)]$$

dove:
- a = area dell'apertura della cella
- L = distanza al substrato
- m = massa della specie
- P(T) = pressione di vapor saturo di equilibrio
- T = temperatura assoluta

Con tassi di crescita convenienti di 1-10 monostrati/s (0.1-1 µm/h), corrisponde a un flusso di 10¹⁵-10¹⁶ molecole/(s·cm²), richiedendo pressioni di equilibrio di 10⁻²-10⁻³ Torr nella cella.

**Aspetto cruciale**: La crescita di GaAs è **limitata dal flusso di Ga**. A 500-600°C l'As aderisce solo in presenza di Ga (coefficiente di sticking trascurabile senza Ga). Non è necessaria **stoichiometria rigorosa** dei flussi. Procedura: scaldare il substrato in flusso di As, poi attivare il flusso di Ga per evitare vacanze di As.

**Preparazione del substrato**:
- Etching in Br-metanolo al 5%
- Risciacquo in metanolo/acqua
- Bakeout 8+ ore a 100-200°C
- Riscaldamento in flusso As a 500-600°C

#### Effetti della Sorgente
- **Sorgente singola GaAs**: As come As₂ → drogaggio n-type (Si, ~5×10¹⁵ cm⁻³)
- **Sorgenti separate Ga/As**: As come As₄ → drogaggio p-type (C, ~10¹⁴ cm⁻³)
- Drogaggio intenzionale: Sn, S, Te, Si (n-type) o Mn, Mg, Be (p-type)

#### Eteroepitassia e Compatibilità Reticolare
La qualità epitassiale dipende dal **disadattamento cristallografico**:
- **GaAs/AlAs**: costanti reticolari simili → film di alta qualità
- **AlₓGa₁₋ₓAs**: composizione arbitraria, banda proibita diretta→indiretta a x≃0.5 (1.4-2.15 eV)
- **Altre coppie**: AlP/GaP, AlSb/GaSb, II-VI con III-V (InP/CdS, InSb/PbTe)
- **Eterogeneità elementale-composta**: Ge/GaAs, Si/GaP, Sn/InSb (α-Sn metastabile sopra 287 K, stabilizzato da MBE a 300 K)

#### Composti Ternari
La variazione della composizione (es. GaAs₁₋ₓPₓ) consente di passare da semiconduttore diretto a indiretto. MBE permette **cambio rapido di composizione** (frazioni di secondo), abilitando la crescita atomicamente netta di profili e interfacce ben definite.

#### Trasferimento e Analisi
I layer sono cresciuti in camera separata e trasferiti in situ in UHV a una seconda camera di analisi mediante meccanismi di trasferimento magnetico o meccanico.

---

## Epitassia mediante Reazioni Chimiche (MOMBE/CBE)

### Tecnica Metal-Organic MBE e Chemical Beam Epitaxy
La **MOMBE** o **Chemical Beam Epitaxy** combina vantaggi delle tecniche UHV con metodi di preparazione continui, applicabili a sistemi III-V (GaAs, GaInAs, InP). Permette preparazione in situ di superfici pulite e ben definite, con trasferimento successivo in camera UHV separata per studi di superficie e interfaccia.

#### Configurazione della Camera di Crescita
- Fonti di AsH₃ e composti Metal-Organici (TMGa o TEGa)
- Crioshield raffreddato a N₂ liquido
- Substrato di GaAs riscaldato a 500-600°C
- Pompe criogeniche abbinate a pompe turbo-molecolari o a diffusione
- Pressione totale di camera: ~10⁻⁶ Torr

#### Sistemi di Iniezione dei Precursori

**Capillare a bassa pressione**:
- Decomposizione termica di AsH₃/PH₃ tramite filamento metallico (Ta o W a ~1000 K)
- Transizione da flusso laminare (10-300 Pa) a flusso molecolare (~10⁻³ Pa)
- Decomposizione di AsH₃ fino al 90%
- Controllo della pressione di fascio entro ±0.2%

**Fonte ad alta pressione**:
- AsH₃/PH₃ a 0.2-2 atm iniettati attraverso tubi in allumina
- Decomposizione in forno a 900-1000°C per collisioni di gas
- Controllo del flusso per variazione di pressione

### Crescita di GaAs e Drogaggio

I prodotti di decomposizione principali sono H₂ e idrocarburi. TMGa e TEGa non sono predissociati ma reagiscono direttamente in superficie.

#### Drogaggio di Tipo p
- **TMGa**: concentrazioni di buche 10¹⁹-10²¹ cm⁻³ a 300 K (ad alta concentrazione di C)
- **TEGa**: concentrazioni 10¹⁴-10¹⁶ cm⁻³ (meno stabile, minore contaminazione)
- **Miscele controllate**: coprono il regime intermedio (10¹⁴-10²¹ cm⁻³)

#### Drogaggio di Tipo n
- **SiH₄** (5% in H₂): concentrazioni elettroniche 10¹⁵-10¹⁹ cm⁻³
- Per >10¹⁶ cm⁻³ richiede predissociazione

Le mobilità di Hall a temperatura ambiente sono comparabili a quelle di strati MBE/MOCVD.

### Vantaggi di MOMBE
- **Qualità equivalente a MBE**: caratteristiche elettriche, cristallografiche e morfologiche
- **Superiore a MBE** nella densità di difetti superficiali (assenti i difetti ovali di ~10 μm)
- Possibilità di controllare reazioni tramite parametri esterni (irradiazione luminosa, bombardamento elettronico)
- Produzione di strutture 2D durante crescita
- Applicabile ad altri materiali (carbossili metallici, ecc.)

### Passivazione e Trasporto di Campioni
Procedura post-crescita:
1. **Passivazione**: deposizione di strato amorfo di As tramite fascio di As
2. **Trasporto**: in atmosfera conservando la qualità della superficie
3. **Recupero in UHV**: riscaldamento a ~300°C per desorbire As e esporre superficie pulita
4. Permette trasferimento tra laboratori mantenendo l'integrità della superficie

---

## Sintesi Comparativa delle Tecniche

| Tecnica | Applicabilità | Qualità Superficie | Controllo | Versatilità |
|---------|---------------|-------------------|-----------|-------------|
| Cleavage | Solo materiali fragili | Eccellente | Limitato a specifiche direzioni | Bassa |
| Ion Bombardment + Annealing | Ampia | Buona | Controllabile | Alta |
| Evaporazione | Ampia | Policristallina/amorfa | Facile | Media |
| MBE | Semiconduttori | Monocristallina, eccellente | Atomico | Molto alta |
| MOMBE/CBE | III-V composti | Monocristallina, eccellente | Atomico | Molto alta |

MBE e MOMBE rappresentano le tecniche più avanzate per preparare superfici e interfacce pulite, ben definite e studiate in ambiente UHV, essenziali sia per ricerca fondamentale che per tecnologie di dispositivi semiconduttori sofisticati.