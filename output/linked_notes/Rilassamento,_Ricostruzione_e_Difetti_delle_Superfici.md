# Rilassamento, Ricostruzione e Difetti delle Superfici

## Rilassamento vs. Ricostruzione

Le modifiche della configurazione atomica superficiale si dividono in due categorie fondamentali:

**Rilassamento**
- Gli atomi si spostano perpendicolarmente alla superficie
- La periodicità 2D del bulk rimane invariata
- Variazioni minime nella struttura cristallina sottostante

**Ricostruzione**
- Gli atomi subiscono spostamenti complessi, anche paralleli alla superficie
- Modifica della periodicità 2D rispetto al bulk
- Può includere configurazioni con atomi o file atomiche mancanti
- Comporta rottura e riformazione di legami chimici

## Esempi Significativi

### GaAs(110): Rilassamento con Tilting

- La struttura LEED mostra la stessa mesh del bulk (nessun cambio di periodicità)
- **Spostamenti atomici**:
  - Atomi di As superficiali: verso l'esterno
  - Atomi di Ga superficiali: verso l'interno
- **Inclinazione del legame**: il legame Ga–As risulta inclinato di circa 27° rispetto alla superficie
- **Meccanismo fisico**: trasferimento di carica elettronica dai dangling bond del Ga a quelli dell'As
  - Il legame Ga assume carattere più sp²
  - Il legame As assume carattere più pz

### Si(111): Ricostruzione (2×1)

- **Struttura**: doppia periodicità nella direzione [0$\bar{1}$1]
- **Modello**: *π-bonded chain model*
  - Atomi di Si si riorganizzano formando catene a zig-zag
  - Legami π si formano tra dangling bond vicini
  - Analogia con molecole organiche a catena lunga
- **Partecipazione degli strati profondi**: anche atomi subsuperficiali sono coinvolti nella ricostruzione
- **Buckling**: spostamento alternato (verso l'esterno/interno) degli atomi superficiali adiacenti
- **Conferma teorica**: i calcoli self-consistent di energia totale dimostrano che questo modello minimizza l'energia del sistema

## Meccanismi Fisici Sottostanti

### Superfici Semiconduttori

- **Meccanismo dominante**: saturazione dei dangling bond mediante formazione di nuovi legami
- **Effetto**: riduzione dell'energia libera superficiale
- **Conseguenza**: tendenza a ricostruzioni complesse

### Superfici Metalliche

**Effetti elettronici**:
- Gli elettroni liberi uniformano la densità di carica alla superficie (smearing)
- Riduzione dell'energia cinetica del sistema
- Formazione di un **dipolo elettronico superficiale** che contribuisce alla funzione lavoro

**Effetti ionici**:
- I core ionici del piano superficiale subiscono una repulsione netta dalla carica nella cella di Wigner–Seitz
- Conseguenza: **contrazione del piano superficiale** (rilassamento inward)
- La maggior parte delle superfici metalliche a basso indice **non presenta ricostruzione**

**Tabella dei rilassamenti tipici** (variazione % della distanza interplanare del primo strato):

| Superficie | Variazione |
|-----------|-----------|
| Ag(110) | −8% |
| Al(110) | −10% |
| Cu(100) | 0% |
| Cu(110) | −10% |
| Cu(311) | −5% |
| Mo(100) | −12.5% |

## Difetti Superficiali

Le superfici reali contengono difetti per ragioni entropiche; le superfici ideali con simmetria traslazionale perfetta non possono esistere. I difetti si classificano per dimensionalità:

### Difetti 0-dimensionali (Puntiformi)

- **Tipologie**: adatomi (dello stesso tipo o esteri), adatomi di ledge, kink, vacanze, interstiziali
- **Su cristalli composti** (es. GaAs):
  - Distinzione tra vacanze di Ga e di As (proprietà elettroniche diverse)
  - **Difetti anti-sito**: atomi nel sito sbagliato (es. As$_{Ga}$ o Ga$_{As}$)
  - Proprietà: centri elettricamente attivi

### Difetti 1-dimensionali (Lineari)

**Gradini (steps)**
- Separano due terrazze adiacenti
- Gli atomi di gradino espongono un numero diverso di dangling bond rispetto agli atomi in terrazza
- Importanza nella formazione di **[[Reticoli 2D, Sovrastrutture e Spazio Reciproco|superfici vicinali]]**: superfici a alto indice costituite da piccole terrazze a basso indice alternate a un'alta densità di gradini regolari

**Effetti dei gradini**:
- **Sui semiconduttori**: i dangling bond ai gradini modificano i livelli energetici elettronici
- **Sui metalli**: il gas elettronico si uniforma al gradino, formando momenti di dipolo locali

### Altri Difetti

- Legati a **dislocazioni**: es. dislocazione a spigolo con vettore di Burgers parallelo alla superficie
- Difetti complessi con periodicità alterata