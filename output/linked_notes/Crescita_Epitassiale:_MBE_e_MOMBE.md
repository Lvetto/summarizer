# Crescita Epitassiale: MBE e MOMBE

## Molecular Beam Epitaxy (MBE)

### Principi Fondamentali

L'**[[Crescita Epitassiale: MBE e MOMBE|MBE]]** è una tecnica di crescita epitassiale in cui film sublimati crescono in modo monocristallino in condizioni di [[Tecnologia dell'Ultravuoto (UHV) e Misura della Pressione|ultra-alto vuoto]] (UHV, P ≤ 10⁻⁹ Torr). Si distingue tra:
- **Homoepitassia**: substrato e film dello stesso materiale
- **Heteroepitassia**: substrato e film di materiali diversi

I vantaggi principali includono film monocristallini, puliti, con stechiometria controllabile e possibilità di realizzare strutture multistrato con profili di drogaggio netti e variazioni composizionali su scala di pochi Ångström.

### Apparato Sperimentale

L'apparato MBE comprende:
- **Celle di effusione Knudsen**: crogioli tubolari in BN pirolitico o grafite riscaldati da spirali di tantalio
- **Criostato ad azoto liquido** attorno alle sorgenti per minimizzare impurezze
- **Otturatori automatici** per ogni cella
- **Spettrometro di massa** per monitoraggio dei flussi
- **Substrato riscaldato** fino a ≥700°C (500–600°C per GaAs homoepitassiale)

### Flusso dalla Cella di Knudsen

Il flusso F al substrato è descritto da:

$$F = \frac{P(T) \cdot a}{\pi L^2 \sqrt{2\pi m K T}} \quad \left[\frac{1}{\text{s·cm}^2}\right]$$

dove:
- *a* = area dell'apertura della cella
- *L* = distanza al substrato
- *m* = massa delle specie effuse
- *P(T)* = pressione di vapore d'equilibrio a temperatura *T*

Le velocità di crescita tipiche sono **1–10 monostrati/s** (0,1–1 µm/h), corrispondenti a flussi di 10¹⁵–10¹⁶ molecole/(s·cm²) e pressioni nella cella di 10⁻²–10⁻³ Torr.

### Crescita di GaAs

La crescita stechiometrica è possibile anche con flussi non stechiometrici grazie a:
- Velocità di crescita limitata dal flusso di Ga
- Coefficiente di adesione trascurabile dell'As in assenza di Ga (500–600°C)
- Lavoro in leggero eccesso di As

Il drogaggio residuo dipende dalla sorgente:
- Sorgenti separate (As come As₄): drogaggio p-type (~10¹⁴ cm⁻³ di C)
- Sorgente unica di GaAs (As come As₂): drogaggio n-type (~5·10¹⁵ cm⁻³ di Si)

### Controllo della Crescita con RHEED

Il **RHEED** (Reflection High Energy Electron Diffraction) consente controllo strato per strato mediante **oscillazioni RHEED**:
- Ogni **massimo** di intensità corrisponde al completamento di uno strato atomico
- La **diminuzione di intensità** tra massimi indica la presenza di disordine (isole incomplete)
- Il periodo τ indica il tempo di deposizione di una monostrato

### Eterostrutture e Alligazioni

L'MBE permette la crescita di composti ternari e quaternari con composizione controllata:

**AlₓGa₁₋ₓAs:**
- Transizione diretto→indiretto a x ≈ 0,5
- Gap variabile da 1,4 eV (GaAs) a 2,15 eV (AlAs)

**GaAs₁₋ₓPₓ:**
- Transizione da semiconduttore diretto a indiretto a x = 0,45
- Il minimo della banda di conduzione si sposta dal punto Γ al punto X

Le interfacce sono **atomicamente nette** grazie ai cambi di composizione realizzabili in frazioni di secondo.

### Qualità delle Interfacce Heteroepitassiali

La qualità dipende dal **[[Struttura delle Interfacce Solido-Solido e Mismatch Reticolare|mismatch reticolare]]**: materiali con costanti di reticolo simili formano interfacce di alta qualità. Esempi:
- GaAs/AlAs
- AlP/GaP
- AlSb/GaSb
- InP/CdS, InSb/PbTe/CdTe
- Ge su GaAs, Si su GaP

Un caso particolare è l'**α-Sn su InSb**: α-Sn (gap nullo, struttura sp³) è stabile come bulk solo sotto 287 K, ma stabilizzato via MBE su InSb(100) a 300 K dal vincolo epitassiale del substrato.

---

## Metal-Organic MBE (MOMBE) / Chemical Beam Epitaxy (CBE)

### Principi e Applicazioni

La tecnica **MOMBE** combina i vantaggi dell'UHV dell'MBE con i processi a flusso continuo della tecnologia dei dispositivi. È applicabile a sistemi III–V (GaAs, GaInAs, InP) e consente la preparazione *in situ* di superfici pulite e ben definite di semiconduttori composti.

### Configurazione Sperimentale

La camera è analoga all'MBE ma con caratteristiche specifiche:
- **Criopannello** ad azoto liquido per minimizzare contaminazione
- **Substrato** (wafer GaAs) riscaldato a 500–600°C per conducibilità termica o irraggiamento
- **Sorgenti in fase gassosa**: valvole di perdita UHV seguiti da capillari di iniezione
- **Sistema di pompaggio**: criopompe in combinazione con pompe turbo/diffusione (a differenza dell'MBE che usa pompe ioniche)

I composti metal-organici (TMGa, TEGa) richiedono solo lieve riscaldamento per evitare condensazione, mentre i precursori del gruppo V (AsH₃, PH₃) devono essere predecomposti.

### Sorgenti per i Precursori del Gruppo V

**1. Capillare a bassa pressione:**
- Decomposizione termica di AsH₃/PH₃ tramite filamento di Ta o W a ≈1000 K
- Flusso da regime idrodinamico (10–300 Pa) a regime molecolare (≈10⁻³ Pa)
- Decomposizione di AsH₃ fino al 90%
- Controllo tramite valvola di perdita (riproducibilità ≈0,2%)

**2. Sorgente ad alta pressione:**
- AsH₃ e PH₃ a 0,2–2 atm iniettati in tubi di allumina
- Decomposizione per collisioni in fase gassosa a 900–1000°C
- Controllo mediante variazione della pressione nel tubo

### Sorgenti Metal-Organiche

Composti come **TEIn** e **TEAl** (per InAs e AlAs) richiedono riscaldamento moderato di contenitore e linee di gas a causa della bassa pressione di vapore, necessario per ottenere velocità di crescita dell'ordine di µm/h.

### Processo di Crescita e Drogaggio

**Condizioni operative:**
- Pressione di fondo: ≈10⁻¹⁰ Torr (dopo bake-out)
- Pressione durante crescita: ≈10⁻⁶ Torr (H₂ e idrocarburi da decomposizione)

**Drogaggio p-type (carbonio su sito As):**
- TMGa: concentrazione di lacune **10¹⁹–10²¹ cm⁻³**
- TEGa: concentrazione di lacune **10¹⁴–10¹⁶ cm⁻³**
- Miscele calibrate coprono l'intervallo **10¹⁴–10²¹ cm⁻³**

**Drogaggio n-type:**
- SiH₄ (5% in H₂): concentrazioni **10¹⁵–10¹⁹ cm⁻³**
- Per >10¹⁶ cm⁻³, SiH₄ deve essere predissociato

Le mobilità di Hall a temperatura ambiente sono comparabili a MBE e MOCVD. La qualità cristallografica e morfologica è equivalente all'MBE; i difetti superficiali di tipo *oval* (≈10 µm diametro) presenti in MBE sono **assenti** in MOMBE.

### Passivazione e Trasferimento delle Superfici

Le superfici cresciute possono essere **passivate** con uno strato di As amorfo depositato durante il raffreddamento. Questo strato protegge da inquinamento atmosferico. Una **ricottura a ≈300°C** in UHV causa la desorbimento dell'As, esponendo la superficie pulita e cristallograficamente integra. Questa temperatura è sufficientemente bassa da evitare decomposizione superficiale, permettendo il **trasferimento di superfici III–V** tra laboratori diversi.

### Vantaggi Relativi e Prospettive

Rispetto all'MBE, le reazioni chimiche superficiali più complesse in MOMBE permettono:
- **Controllo esterno del processo di crescita** mediante irradiazione luminosa o bombardamento elettronico
- Produzione di **strutture bidimensionali** direttamente durante la crescita

MBE e MOMBE sono strumenti preziosi sia per la ricerca su superfici e interfacce in ambiente UHV, sia per la tecnologia dei dispositivi a semiconduttore.