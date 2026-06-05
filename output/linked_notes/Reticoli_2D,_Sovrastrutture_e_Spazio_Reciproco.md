# Reticoli 2D, Sovrastrutture e Spazio Reciproco

## Reticoli Bidimensionali di Bravais

Un reticolo bidimensionale è completamente definito da due vettori di base **a** e **b**, che formano un angolo γ tra loro. Qualsiasi punto del reticolo è raggiungibile tramite il vettore di traslazione:

$$\mathbf{R} = m\mathbf{a} + n\mathbf{b} \quad (m, n \in \mathbb{Z})$$

In due dimensioni esistono esattamente **5 reticoli di Bravais**, contro i 14 in tre dimensioni:

1. **Obliquo**: γ ≠ 90°, |a| ≠ |b|
2. **Rettangolare**: γ = 90°, |a| ≠ |b|
3. **Rettangolare centrato** (rombico): variante centrata del rettangolare
4. **Quadrato**: γ = 90°, |a| = |b|
5. **Esagonale**: γ = 60° o 120°, |a| = |b|

---

## Reticoli Superficiali e Sovrastrutture

### Definizione e Origine

Quando atomi o molecole adsorbiti su una superficie formano un ordine periodico **diverso** da quello del substrato sottostante, si forma una **sovrastruttura**. Questo accade perché gli esperimenti di diffrazione superficiale (come [[LEED]]) sondano non solo lo strato atomico più esterno, ma diversi strati: il substrato ideale, gli strati di [[Rilassamento, Ricostruzione e Difetti delle Superfici|ricostruzione superficiale]], e gli strati di adsorbato ordinato.

### Descrizione Formale mediante Matrice di Trasformazione

La relazione tra i vettori primitivi della sovrastruttura (**b₁**, **b₂**) e quelli del substrato (**a₁**, **a₂**) è espressa mediante una **matrice di trasformazione M** a elementi interi (o razionali):

$$\begin{pmatrix} \mathbf{b}_1 \\ \mathbf{b}_2 \end{pmatrix} = M \begin{pmatrix} \mathbf{a}_1 \\ \mathbf{a}_2 \end{pmatrix}, \quad M = \begin{pmatrix} m_{11} & m_{12} \\ m_{21} & m_{22} \end{pmatrix}$$

Il rapporto tra l'area della cella della sovrastruttura (B) e quella del substrato (A) è determinato dal determinante della matrice:

$$B = A \cdot \det M$$

### Classificazione delle Sovrastrutture

La natura di **det M** classifica il tipo di struttura risultante:

| **det M** | **Tipo di struttura** | **Caratteristiche** |
|---|---|---|
| Intero | Superlattice semplice | Periodicità razionale semplice |
| Numero razionale | Reticolo di coincidenza | Periodicità razionale complessa |
| Numero irrazionale | Struttura incommensurabile | L'adsorbato non si sincronizza con il substrato; interazione adsorbato-substrato molto debole |

Le strutture incommensurabili si formano quando l'interazione tra le particelle adsorbite è molto più forte dell'interazione adsorbato-substrato, causando il disaccoppiamento della sovrastruttura dalla periodicità del substrato.

### Notazione di Wood

La **notazione di Wood** è la convenzione standard per descrivere le sovrastrutture, utilizzata quando i vettori della sovrastruttura sono paralleli a quelli del substrato:

$$X\{hkl\}(p \times q) \quad \text{oppure} \quad X\{hkl\}\,c(p \times q)R\alpha°$$

dove:
- **X{hkl}**: materiale e indici di Miller della faccia cristallografica
- **(p × q)**: rapporto tra i moduli dei vettori primitivi della sovrastruttura e del substrato
- **c**: indica la presenza di una centratura nella cella della sovrastruttura
- **Rα°**: angolo di rotazione della sovrastruttura rispetto al substrato (omesso se assente)

---

## Spazio Reciproco 2D

### Vettori del Reticolo Reciproco

Il reticolo reciproco 2D è definito dai vettori **a\*** e **b\*** che soddisfano le condizioni di ortogonalità rispetto ai vettori dello spazio diretto:

$$\mathbf{a} \cdot \mathbf{a^*} = 2\pi, \quad \mathbf{a} \cdot \mathbf{b^*} = 0$$
$$\mathbf{b} \cdot \mathbf{a^*} = 0, \quad \mathbf{b} \cdot \mathbf{b^*} = 2\pi$$

I punti del reticolo reciproco sono identificati dai vettori:

$$\mathbf{G} = h\mathbf{a^*} + k\mathbf{b^*} \quad (h, k \in \mathbb{Z})$$

### Relazione tra Spazio Diretto e Reciproco nella Sovrastruttura

Se la matrice **M** descrive la sovrastruttura nello spazio diretto, il reticolo reciproco della sovrastruttura è descritto dalla matrice inversa trasposta $(\mathbf{M}^{-1})^T$. Questo implica una relazione **inversa** tra i due spazi:

- Una **cella grande** nello spazio reale produce punti di diffrazione **più ravvicinati** nello spazio reciproco
- Una **cella piccola** nello spazio reale produce punti di diffrazione **più separati** nello spazio reciproco

### Spot di Sovrastruttura

Quando compare una sovrastruttura rispetto al substrato, nel diagramma di diffrazione (spazio reciproco) appaiono **punti addizionali**, detti **spot di sovrastruttura**, oltre ai punti già presenti dal substrato. Questi spot aggiuntivi riflettono direttamente la periodicità più grande della sovrastruttura nello spazio diretto.

---

## Applicazioni nella Fisica delle Superfici

L'analisi dello spazio reciproco 2D è fondamentale per interpretare esperimenti di diffrazione superficiale, in particolare [[LEED]] (Low Energy Electron Diffraction). La posizione e l'intensità degli spot di diffrazione rivelano:

- La **geometria e la simmetria** del reticolo 2D della superficie
- La **periodicità** della sovrastruttura formata dagli adsorbati
- Lo **stato ordinato** dei layers superficiali
- Eventuali **rotazioni** e **disallineamenti** tra substrato e sovrastruttura