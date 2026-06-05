# Struttura e Morfologia di Superfici e Interfacce

## Stress Superficiale ed Energia Superficiale

### Tensore dello Stress Superficiale
Il [[tensore dello stress]] τij descrive le forze nei materiali in risposta a deformazioni. Quando una superficie viene creata, la distribuzione di carica e le forze atomiche nelle topmost layers cambiano rispetto al bulk, comportando una variazione dello stress tensor lungo l'asse perpendicolare alla superficie entro diversi spessori atomici.

Il **tensore dello stress superficiale** è definito come:
$$\tau^{(s)}_{ij} = \int_{-\infty}^{\infty} dz \left[\tau_{ij}(z) - \tau^{(b)}_{ij}\right]$$

dove τ^(b)_ij è lo stress del bulk. Questo parametro ha dimensioni di forza per unità di lunghezza (~1 N/m) e rimane confinato entro ~1 nm dalla superficie. Uno stress positivo (tensile) indica che la superficie tende a contrarsi, mentre uno negativo è compressivo.

### Energia Superficiale Libera e Shuttleworth Equation
L'[[energia superficiale]] libera specifica γ rappresenta l'eccesso di energia libera per unità di area—il lavoro reversibile necessario per creare una nuova superficie, originato dalla rottura di legami atomici e dalla formazione di difetti superficiali.

La relazione tra lo stress superficiale e l'energia superficiale è data dalla **Shuttleworth equation**:
$$\tau^{(s)}_{ij} = \gamma \delta_{ij} + \frac{\partial \gamma}{\partial \varepsilon_{ij}}$$

Per i liquidi, il secondo termine svanisce e lo stress superficiale isotropo coincide con γ. Per i solidi, il termine ∂γ/∂ε rappresenta la forza termodinamica per il movimento di atomi dalla bulk alla superficie e favorisce la formazione di ricostruzioni superficiali.

## Forma di Equilibrio dei Cristalli

### Principio di Minima Energia
La forma di equilibrio di un cristallo minimizza l'energia libera totale:
$$\int_A \gamma(n)dA = \text{minimo}$$

L'energia superficiale γ dipende fortemente dall'orientazione del piano superficiale (hkl) nei materiali cristallini.

### Wulff Plot
Il **Wulff plot** rappresenta γ(hkl) in coordinate polari, dove:
- La lunghezza del vettore dalla origine rappresenta l'ampiezza di γ
- La direzione è quella della normale al piano (hkl)
- La forma di equilibrio è l'inviluppo interno dei piani di Wulff

### Superfici Vicinali
Le [[superfici vicinali]] sono inclinate di un angolo θ rispetto a un piano a basso indice, composte da terrazze separate da scalini atomici. Per tali superfici:
$$\gamma(\theta) = \gamma_0 \cos\theta + \gamma_1 \frac{\sin\theta}{a}$$

Nel plot di Wulff, questa relazione descrive un cerchio passante per l'origine.

## Rilassamento e Ricostruzione Superficiale

### Rilassamento (Relaxation)
Il [[rilassamento]] consiste in spostamenti atomici perpendicolari alla superficie senza variazione della periodicità 2D della struttura.

### Ricostruzione (Reconstruction)
La [[ricostruzione]] è un riarrangiamento più complesso degli atomi che altera la periodicità parallela alla superficie, includendo:
- Spostamenti atomici non solo perpendicolari alla superficie
- Assenza di atomi interi o file di atomi rispetto alla struttura bulk

**Esempi significativi:**
- **GaAs(110)**: Gli atomi di As dello strato superficiale si alzano, mentre gli atomi di Ga si spostano verso l'interno, con inclinazione del legame Ga–As di ~27° rispetto alla superficie
- **Si(111)-(2×1)**: Pattern LEED a doppia periodicità con formazione di catene zigzag di legami π tramite rottura e riformazione di legami

### Meccanismi Fisici

**Su semiconduttori:** La tendenza principale è saturare i dangling bond liberi formando nuovi legami superficiali, riducendo l'energia superficiale. Su semiconduttori polari, il trasferimento di carica elettronica tra i dangling bond causa spostamenti atomici osservati.

**Su metalli:** Il meccanismo riguarda la ridistribuzione della carica elettronica. La densità elettronica superficiale tende ad uniformarsi per ridurre l'energia cinetica degli elettroni, formando un dipolo elettronico superficiale che causa una contrazione verso l'interno (tipicamente 5-12.5%). La maggior parte delle superfici metalliche a basso indice non presenta ricostruzione.

## Difetti Superficiali

I [[difetti superficiali]] si classificano per dimensionalità:

### Difetti 0-dimensionali (Point Defects)
- Adatomi singoli, adatomi di ledge, kink, vacanze
- Su semiconduttori composti: adatomi dello stesso tipo o stranieri; adatomi superficiali o interstiziali
- Difetti anti-site (es. AsGa su GaAs): causano centri elettricamente attivi

### Difetti 1-dimensionali (Line Defects)
- **Gradini (steps):** Separano terrazzamenti di diverso livello e formano superfici vicinali orientate a piccoli angoli rispetto a superfici a basso indice
- Su semiconduttori: la struttura dei dangling bond modifica i livelli energetici elettronici
- Su metalli: il gas di elettroni liberi si uniforma creando dipoli dovuti ai nuclei ionici fissi spazialmente

### Difetti Correlati a Dislocazioni
[[Dislocazioni]] che penetrano la superficie con vettore di Burgers parallelo a essa.

## Reticoli Bidimensionali e Sovrastrutture

### Definizioni Base
Un [[reticolo bidimensionale]] è definito da due vettori di traslazione non paralleli **a₁** e **a₂**, che generano tutti i punti del reticolo tramite combinazioni lineari intere:
$$\mathbf{R} = n_1\mathbf{a}_1 + n_2\mathbf{a}_2$$

### Sovrastrutture (Superstructures)
Le [[sovrastrutture]] sono configurazioni atomiche periodiche con periodicità maggiore rispetto al reticolo primitivo sottostante, originate da:
- Ordinamento di atomi su siti equivalenti
- Occupazione selettiva di siti reticolari
- Distorsioni periodiche della struttura

Una sovrastruttura è caratterizzata da vettori **b₁** e **b₂** correlati al reticolo primitivo mediante:
$$\mathbf{b}_i = \sum_j A_{ij} \mathbf{a}_j$$

dove A_ij sono coefficienti interi.

### Reticoli di Bravais Bidimensionali
Esistono cinque possibili [[reticoli di Bravais]] bidimensionali. Nella pratica si utilizzano spesso mesh centrate (come quella quadrata) per convenienza descrittiva.

## Reticolo Reciproco 2D

### Costruzione e Proprietà Fondamentali
I vettori base del [[reticolo reciproco]] 2D (**b₁*, **b₂***) sono costruiti dai vettori base del reticolo diretto (**a₁**, **a₂**) secondo:

- **b₁*** = 2π(**a₂** × **ẑ**)/(**a₁** · (**a₂** × **ẑ**))
- **b₂*** = 2π(**ẑ** × **a₁**)/(**a₁** · (**a₂** × **ẑ**))

dove **ẑ** è il versore perpendicolare al piano 2D.

I vettori reciproci soddisfano le condizioni di ortogonalità:
$$\mathbf{a}_i \cdot \mathbf{b}^*_j = 2\pi\delta_{ij}$$

### Proprietà Chiave
- **Periodicità:** Il reticolo reciproco è periodico con vettori di traslazione interi
- **Relazione geometrica:** Se il reticolo diretto è denso, quello reciproco è rado, e viceversa
- **Applicazioni:** Fondamentale per l'analisi della [[diffrazione]] di raggi X e per la comprensione della struttura delle bande cristalline

## Descrizione Formale delle Strutture Superficiali

### Relazione tra Reticoli Superficiali e Substrato
Gli esperimenti di diffrazione sulla superficie forniscono informazioni su più strati atomici. Quando gli strati superficiali presentano periodicità diversa dal substrato (per ricostruzioni o adsorbati ordinati), un **superlattice** si sovrappone al reticolo del substrato.

Il reticolo superficiale è relazionato al substrato mediante:
$$\begin{pmatrix} \mathbf{b}_1 \\ \mathbf{b}_2 \end{pmatrix} = M \begin{pmatrix} \mathbf{a}_1 \\ \mathbf{a}_2 \end{pmatrix}$$

dove **M** è una matrice 2×2:
$$M = \begin{pmatrix} m_{11} & m_{12} \\ m_{21} & m_{22} \end{pmatrix}$$

### Relazione tra Aree
Le aree della mesh superficiale (B) e del substrato (A) sono correlate da:
$$B = |b_1 \times b_2| = A \det M$$

### Classificazione delle Superstructure
- **Simply Related** (det M intero): superstructure semplice
- **Coincidence Lattice** (det M razionale): reticoli commensurabilii
- **Incoherent Lattice** (det M irrazionale): strutture incommensurabilii

### Notazione di Wood
Per superstructure con **b₁ ∥ a₁** e **b₂ ∥ a₂**:
$$\mathbf{b}_1 = p\mathbf{a}_1, \quad \mathbf{b}_2 = q\mathbf{a}_2$$

Si utilizza la notazione:
$$X\{hkl\}(p \times q) \quad \text{o} \quad X\{hkl\}c(p \times q)$$

dove il simbolo *c* indica un possibile centraggio, e X{hkl} identifica la superficie del substrato.

## Modelli Strutturali delle Interfacce Solido-Solido

### Caratteristiche Generali
Le [[interfacce]] solido-solido possono essere:
- **Nitide e abrupte** a livello atomico
- **Diffuse** per interdiffusione e/o formazione di nuovi composti chimici

La nitidezza è caratterizzata dal profilo di concentrazione dei materiali, che dipende da costanti di diffusione, velocità di reazione e tempo di contatto.

### Ruolo dei Diagrammi di Fase
I diagrammi di fase forniscono informazioni termodinamiche essenziali:
- **Miscibilità completa:** consente interfacce graduali
- **Miscibilità limitata:** produce interfacce nitide con cambiamento abruptivo
- **Fasi multiple stabili:** generano interfacce multi-strato

Le limitazioni cinetiche possono impedire la formazione di fasi termodinamicamente possibili.

### Modello dell'Interstrato Amorfo
Assume uno strato amorfo (simile a liquido) dove la struttura cristallina è completamente disturbata. Gli atomi all'interfaccia, in posizioni energeticamente sfavorevoli, si spostano dai loro siti cristallografici riducendo l'energia.

### Modelli Basati su Dislocazioni

**Tilt Boundary (Bordo di Inclinazione):**
Separazione tra cristalli inclinati mediante dislocazioni di bordo. La distanza tra dislocazioni:
$$s = \frac{a}{2\sin(\theta/2)} \simeq \frac{a}{\theta}$$

dove θ è l'angolo di inclinazione e a la costante reticolare.

**Twist Boundary (Bordo di Torsione):**
Adattamento di reticoli ruotati mediante dislocazioni a vite.

**Interfacce Eterofasiche (Heteroepitassia):**
Film monocristallino su substrato monocristallino diverso. Con disadattamento reticolare, le dislocazioni di bordo all'interfaccia hanno distanza:
$$s = \frac{ab}{|b-a|}$$

dove a e b sono le costanti reticolari dei due materiali.

### Rilassamento del Disadattamento Reticolare
Per film epitassiali sottili con basso disadattamento, il matching può avvenire per strain elastico o dislocazioni. La scelta dipende da:
- Spessore del film (h)
- Entità del disadattamento reticolare
- Confronto delle energie libere

**Comportamento Energia-Spessore:**
- **Sotto spessore critico h₀:** film stressato con strain inferiore all'energia delle dislocazioni
- **Sopra valori critici:** formazione di dislocazioni energeticamente favorevole

I valori critici teorici di spessore sono inferiori a quelli sperimentali, dimostrando che limitazioni cinetiche (nucleazione) influenzano il tipo di rilassamento del disadattamento.