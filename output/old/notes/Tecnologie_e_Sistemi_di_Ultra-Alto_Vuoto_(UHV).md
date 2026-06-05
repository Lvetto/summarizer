# Tecnologie e Sistemi di Ultra-Alto Vuoto (UHV)

## Introduzione e Motivazione

L'**Ultra-Alto Vuoto (UHV)** è una condizione essenziale per lo studio delle interfacce superficie-vuoto. A pressioni sufficientemente basse, è possibile trascurare l'influenza della fase gassosa e della contaminazione, consentendo l'osservazione di superfici cristalline pulite in condizioni ben definite. La pressione limite per condizioni UHV è inferiore a **10⁻¹⁰ Torr** (≈10⁻⁸ Pa).

### Relazione tra Pressione e Contaminazione Superficiale

Il numero di particelle di gas residuo che colpiscono 1 cm² di superficie al secondo (tasso di impatto **ż**) è correlato alla pressione ambiente mediante:

$$p = 2m\langle v \rangle \dot{z}$$

dove m è la massa molecolare e ⟨v⟩ è la velocità termica media.

**Risultato critico**: A ~10⁻⁶ Torr, il numero di molecole necessario a formare un monostrato superficiale raggiunge la superficie ogni secondo. Quindi, per mantenere una superficie pulita per circa un'ora, è necessaria una pressione inferiore a **10⁻¹⁰ Torr**.

### Unità Langmuir

L'esposizione superficiale è quantificata in **Langmuir (L)**:
- **1 L** = esposizione per 1 s a 10⁻⁶ Torr
- Per coefficiente di adsorbimento S ≈ 1, **1 L produce circa un monostrato** di adsorbato

---

## Architettura dei Sistemi UHV

Un sistema UHV completo comprende:
- **Recipiente**: acciaio inossidabile
- **Connessioni**: flange Conflat standard sigillate con guarnizioni in rame monouso
- **Trattamento termico**: riscaldamento (bake-out) necessario per raggiungere condizioni UHV e rimuovere adsorbati dalle pareti

---

## Sistemi di Evacuazione

### Pompe di Roughing (Evacuazione Iniziale)

Portano il sistema da pressione atmosferica a ~10⁻³ Torr:

**Pompe a sorpimento (sorption pumps)**
- Utilizzano materiale poroso (zeolite) attivato a bassa temperatura con azoto liquido
- Richiedono rigenerazione periodica
- Forniscono velocità di pompaggio media

**Pompe rotanti (rotary vane pumps)**
- Comprimono il gas mediante rotore eccentrico
- Essenziali come supporto alle turbomoleccolari
- Limitano la pressione finale a ~10⁻³ Torr

### Pompe UHV

#### 1. Pompa Turbomolecolare

**Principio di funzionamento**: Rotore ad alta velocità (15.000-30.000 rpm) che "spinge" molecole dal lato UHV verso quello di backing. L'effetto pompaggio è puramente **geometrico**, basato sull'inclinazione delle pale.

**Caratteristiche**:
- Nessuna reazione chimica con il gas
- Rapporto di compressione dipende dalla massa molecolare (basso per H₂)
- Velocità di pompaggio ridotta per gas leggeri
- Intervallo di pressione: 10⁻⁴ - 10⁻¹¹ Torr
- Ideale per applicazioni generiche UHV

#### 2. Pompa Ion-Getter

**Principio di funzionamento**: Celle multicellulari con scarica elettrica tra anodo e catodo (migliaia di volt) in campo magnetico. Gli elettroni seguono percorsi elicoidali ionizzando il gas residuo; gli ioni vengono catturati sul catodo di Ti o sputterano atomi di Ti per intrappolare ulteriori molecole.

**Caratteristiche**:
- Intervallo di pressione operativa: 10⁻⁴ - <10⁻¹² Torr
- Velocità di pompaggio: 1-5000 ℓ/s
- **Problema critico**: l'argon limita significativamente la velocità di pompaggio
- **Non idonee** per studi di adsorbimento poiché ionizzano il gas
- Richiedono isolamento con valvole durante esperimenti ad alta pressione

#### 3. Pompa a Diffusione (Vapor Pump)

**Principio di funzionamento**: Il vapore (olio o mercurio) risale una colonna e collide con molecole di gas. L'interazione avviene per:
- **Diffusione**: quando il cammino libero medio > larghezza della gola
- **Trascinamento viscoso**: quando il cammino libero medio < larghezza della gola

**Caratteristiche**:
- Svantaggi: back-streaming e back-diffusione del fluido di lavoro
- Richiedono **baffle e trappole fredde** raffreddate con azoto liquido
- Pressione finale: ~10⁻¹⁰ Torr (con oli di qualità elevata)
- Ideale per sistemi di microscopia elettronica
- Elevata velocità di pompaggio a pressioni intermedie

#### 4. Pompa Criogenica

**Principio di funzionamento**: Condensazione di gas su superfici raffreddate (elio liquido a 4,2 K). Un serpentino metallico funge da superficie condensante, raffreddato da elio liquido controllato da valvola a strangolamento.

**Caratteristiche**:
- **Velocità di pompaggio straordinariamente alta**: 10⁴-10⁶ ℓ/s
- Pressione ultima determinata dalla tensione di vapore saturo: **p_min = P_v(T_v)**
- Efficace per **tutti i gas tranne He e H₂**
- **Non utilizzabile** a pressioni > 10⁻⁴ Torr (rischio di intasamento)
- Richiede manutenzione e approvvigionamento continuo di elio liquido
- Ideale per esperimenti a breve termine richiedenti UHV estremo

---

## Misurazione della Pressione

### Pirani Gauge (10⁻⁴ - 100 Torr)

Misura la conduttività termica del gas tramite variazione di resistenza di un filamento riscaldato in ponte di Wheatstone.
- Richiede calibrazione per ogni gas
- Non adatto a pressioni UHV estreme

### Ionization Gauge (< 10⁻⁴ Torr)

Gli atomi residui esposti a fascio di elettroni (energia: 12,6-24,6 eV) vengono ionizzati. La corrente ionica **I⁺** è direttamente proporzionale alla pressione.

**Configurazione Bayard-Alpert**:
- Filamenti multipli
- Griglia cilindrica per ionizzazione
- Collettore di ioni sottile e centrale
- **Misure fino a 10⁻¹² Torr**, evitando raggi X prodotti da collettori estesi

---

## Equazioni Fondamentali

### Equazione di Pompaggio

$$v A_v = V_v \frac{dp}{dt} + \widetilde{S} p$$

dove:
- **v** = tasso di desorbimento
- **A_v** = area superficiale
- **V_v** = volume del sistema
- **S** = velocità di pompaggio effettiva [ℓ/s]
- **p** = pressione

### Conduttanza (Analogia con Legge di Ohm)

$$I_{mol} = Cp/RT$$

**Combinazioni di conduttanza**:
- **Serie**: 1/C_s = 1/C₁ + 1/C₂
- **Parallelo**: C_p = C₁ + C₂

### Velocità di Pompaggio Efficace

$$\frac{1}{\widetilde{S}_{eff}} = \frac{1}{\widetilde{S}_p} + \frac{1}{C_p}$$

La velocità di pompaggio effettiva è limitata dalla conduttanza del collegamento tra pompa e camera.

### Conduttanza per Flusso Viscoso

Valida quando d > 10 mbarᐧmm:

$$C[\ell/s] = 137 \frac{d^4[cm^4]}{L[cm] \cdot p[mbar]}$$

dove d è il diametro del tubo e L è la lunghezza.

---

## Considerazioni Pratiche per la Progettazione

1. **Selezione della pompa**: Dipende dal range di pressione, dalla velocità di pompaggio richiesta e dalla compatibilità con l'esperimento
2. **Conduttanza**: Dimensionare adeguatamente i tubi di collegamento per minimizzare le perdite
3. **Bake-out**: Necessario per rimuovere adsorbati dalle pareti e raggiungere UHV stabile
4. **Monitoraggio**: Utilizzare manometri appropriati al range di pressione operativo
5. **Isolamento**: Valvole di isolamento per proteggere pompe sensibili durante modifiche al sistema