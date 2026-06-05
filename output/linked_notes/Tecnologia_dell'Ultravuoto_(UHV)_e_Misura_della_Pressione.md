# Tecnologia dell'Ultravuoto (UHV) e Misura della Pressione

## Introduzione e Motivazione

L'**[[Tecnologia dell'Ultravuoto (UHV) e Misura della Pressione|ultravuoto (UHV)]]** è una condizione essenziale per lo studio delle interfacce superficiali in [[Introduzione alla Fisica delle Superfici e delle Interfacce|fisica delle superfici]]. Per mantenere un'interfaccia cristallina pura e non contaminata, è necessario operare a pressioni inferiori a **10⁻¹⁰ Torr** (≈ 10⁻⁸ Pa).

### Calcolo della pressione necessaria

Il tasso di impatto $\dot{z}$ [cm⁻² s⁻¹] delle molecole del gas residuo sulla superficie è legato alla pressione dalla relazione:

$$p \simeq \frac{6kT\dot{z}}{\langle v \rangle}$$

dove $m$ è la massa molecolare e $\langle v \rangle$ è la velocità termica media.

Considerando un monostrato superficiale di 3 × 10¹⁴ particelle/cm² a temperatura ambiente (T = 300 K) con peso molecolare medio di 28:

$$\dot{z} = 3 \times 10^{14} \text{ cm}^{-2}\text{s}^{-1} \simeq 5 \times 10^{-6} \cdot \frac{p}{\text{Torr}}$$

**A pressione di 10⁻⁶ Torr, le molecole sufficienti a formare un monostrato colpiscono la superficie ogni secondo.** Per mantenerla pulita durante un esperimento (~1 ora), la pressione deve rimanere al di sotto di **10⁻¹⁰ Torr**.

### Unità Langmuir

In fisica delle superfici si utilizza il **Langmuir (L)** per quantificare l'esposizione superficiale:

> **1 L** = 1 secondo di esposizione a 10⁻⁶ Torr

Per superfici con coefficiente di adesione S ≈ 1, un'esposizione di 1 L corrisponde a circa un monostrato adsorbito.

---

## Struttura e Componenti di un Sistema UHV

### Configurazione generale

Un sistema UHV è composto da:
- **Camera**: in acciaio inossidabile per resistenza alla corrosione
- **Flange Conflat**: connessioni standard disponibili in varie dimensioni, che utilizzano guarnizioni in rame monouso per garantire la tenuta
- **Connessioni ausiliarie**: raccordi in gomma o viton per parti non sottoposte a UHV

### Preparazione iniziale: Bake-out

Per raggiungere condizioni UHV, il sistema deve essere sottoposto a una procedura di **bake-out** (cottura termica a ~10⁻⁷ Torr). Questo processo rimuove l'acqua e altri contaminanti adsorbiti sulle pareti della camera, consentendo il raggiungimento del regime UHV.

---

## Pompe per il Vuoto

### Pompe di preriscaldamento (Roughing Pumps)

Stabiliscono il vuoto iniziale nel range **10⁻² – 10⁻³ Torr**.

#### Pompa a sorbimento
- Contiene **zeolite** (setaccio molecolare) con alta superficie attiva
- Attivata raffreddando le pareti con **azoto liquido**
- Limitazione: il materiale sorbente si satura, non può funzionare continuamente
- Richiede rigenerazione periodica

#### Pompa rotativa
- **Meccanismo**: rotore eccentrico con due palette che variano il volume interno
- **Fase di aspirazione**: il volume si espande, il gas entra
- **Fase di compressione**: il gas viene spinto attraverso una valvola di scarico
- **Protezione**: valvola di carico gas previene la condensazione dei vapori
- Ideale come primo stadio di pompaggio

### Pompe per il regime UHV

#### Pompa turbomolecolare
- **Principio**: rotore ad alta velocità (15.000–30.000 rpm) "spinge" le molecole dal lato UHV verso lo scarico
- **Meccanismo**: pale del rotore e dello statore hanno inclinazioni opposte, creando una geometria che favorisce il passaggio unidirezionale delle molecole
- **Rapporto di compressione**: dipende dalla massa molecolare e dalla velocità; prestazioni ridotte per gas leggeri (H₂)
- **Vantaggio**: nessuna reazione chimica indesiderata
- **Range di pressione**: efficace nel regime UHV

#### Pompa ionica (Ion-getter pump)
- **Assenza di parti rotanti**: ideale per il mantenimento a lungo termine dell'UHV
- **Meccanismo**: 
  - Scarica elettrica (migliaia di volt) in campo magnetico (migliaia di Gauss)
  - Le molecole residue vengono ionizzate
  - Gli ioni sono accelerati verso il catodo in titanio (Ti)
  - Vengono intrappolati o causano sputtering di atomi Ti che catturano ulteriori molecole
- **Range di pressione**: 10⁻⁴ – 10⁻¹² Torr
- **Limitazione**: sconsigliata per studi di adsorbimento con molecole grandi

#### Pompa a vapore (Diffusion pump)
- **Meccanismo**: flusso di vapore (olio o mercurio) trascina le molecole di gas verso lo scarico per diffusione o trascinamento viscoso
- **Principale svantaggio**: **back-streaming** delle molecole del fluido di lavoro limita la pressione finale
- **Soluzioni mitigative**:
  - **Baffle**: ostacoli che riducono il flusso inverso di vapore
  - **Trappole fredde ad azoto liquido**: condensano i vapori prima che raggiungano la camera
- **Prestazioni**: con oli UHV di alta qualità si raggiungono **10⁻¹⁰ Torr**

#### Criobomba (Cryopump)
- **Principio**: sfrutta la **condensazione dei gas** su superfici raffreddate a elio liquido (4,2 K)
- **Velocità di pompaggio**: elevatissima (10⁴ – 10⁶ ℓ/s)
- **Pressioni raggiungibili**: inferiori a 10⁻¹⁰ Torr per la maggior parte dei gas
- **Limitazioni**:
  - Non utilizzabile a pressioni > 10⁻⁴ Torr
  - He e H₂ non vengono condensati efficacemente
- **Vantaggi**: assenza di contaminanti, nessun back-streaming

---

## Misura della Pressione

### Manometri a diaframma
- **Range**: alte pressioni (> 10⁻⁴ Torr)
- **Principio**: misurano la deflessione di un diaframma metallico, proporzionale alla variazione di volume dovuta alla pressione

### Manometro a viscosità molecolare
- **Principio**: sfrutta la dipendenza della viscosità del gas dalla pressione
- **Variante spinning-ball**: sfera rotante che oscilla, con dissipazione dipendente dalla pressione
- **Range**: fino a 10⁻¹⁰ Torr

### Manometro a conduttività termica (Pirani)
- **Range**: ~10⁻³ a ~100 Torr
- **Meccanismo**:
  - Filamento riscaldato (Pt o W) in ponte di Wheatstone
  - La pressione influenza il raffreddamento del filamento modificandone la resistenza
  - La variazione di resistenza è proporzionale alla pressione
- **Limitazione**: richiede calibrazione

### Manometro a ionizzazione (Bayard-Alpert)
- **Più importante per le condizioni UHV**: misura pressioni inferiori a 10⁻⁴ Torr (fino a < 10⁻¹⁰ Torr)
- **Meccanismo**:
  - Filamento caldo emette elettroni per **emissione termoionica**
  - Gli elettroni ionizzano le molecole del gas residuo
  - La corrente ionica I⁺ è proporzionale alla pressione
  - La corrente elettronica I⁻ viene mantenuta costante
- **Innovazione costruttiva Bayard-Alpert**: collettore ionico a filo sottile che **minimizza la produzione di raggi X molli**, i quali altrimenti causerebbero fotoemissione e un segnale limite spurio

---

## Equazioni Fondamentali

### Equazione di pompaggio

La conservazione delle particelle in una camera UHV è descritta da:

$$v A_v = \frac{V_v}{kT} \frac{dp}{dt} + \frac{\tilde{S} p}{V_v}$$

dove:
- $A_v$: superficie interna della camera [cm²]
- $V_v$: volume della camera [cm³]
- $v$: tasso di desorbimento dalle pareti
- $\tilde{S}$: velocità di pompaggio [ℓ/s]
- $p$: pressione

### Conduttanza

La conduttanza descrive il flusso di gas attraverso una condotta, in analogia con la legge di Ohm:

$$I_{mol} = C \cdot \frac{p}{RT}$$

**Combinazioni di conduttanze:**
- **Serie**: $\frac{1}{C_s} = \frac{1}{C_1} + \frac{1}{C_2}$ (la conduttanza minore domina)
- **Parallelo**: $C_p = C_1 + C_2$

**Velocità di pompaggio effettiva** considerando la conduttanza della tubazione:

$$\frac{1}{\tilde{S}_{eff}} = \frac{1}{\tilde{S}_p} + \frac{1}{C_p}$$

### Conduttanza di un tubo circolare

Nel **regime di flusso viscoso** (pd > 10 mbar·mm):

$$C \, [\ell/s] = \frac{137 \, d^4 \, [\text{cm}^4]}{L \, [\text{cm}]} \cdot p \, [\text{mbar}]$$

dove $d$ è il diametro e $L$ è la lunghezza del tubo. La conduttanza aumenta significativamente con il diametro (proporzionalità a d⁴) e diminuisce con la lunghezza.