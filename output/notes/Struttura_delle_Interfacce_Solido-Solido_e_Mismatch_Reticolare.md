# Struttura delle Interfacce Solido-Solido e Mismatch Reticolare

## Caratteristiche Generali delle Interfacce Solido-Solido

Le interfacce tra materiali solidi presentano due configurazioni fondamentali:
- **Interfacce nette e abrupte**: transizione netta a livello atomico tra i due materiali
- **Interfacce graduali**: transizione graduale dovuta a interdiffusione e/o formazione di nuovi composti chimici

La "nitidezza" dell'interfaccia può essere descritta mediante i profili di concentrazione dei componenti A e B in funzione della profondità.

## Ruolo della Termodinamica: Diagrammi di Fase

I diagrammi di fase determinano il tipo di interfaccia che si forma a una data temperatura T₀:

- **Miscibilità completa** → interfaccia graduale con composizione che varia continuamente
- **Miscibilità limitata** → interfaccia netta con salto brusco di concentrazione tra due fasi distinte I e II
- **Più fasi stabili** → interfacce spazialmente estese con strati multipli

**Nota importante**: le considerazioni termodinamiche forniscono solo indicazioni generali. Non tutte le fasi termodinamicamente possibili si formano necessariamente a causa di **limitazioni cinetiche** (elevate energie di attivazione per nucleazione).

## Modelli Strutturali Atomici

### Modello Amorfo (Brillouin, 1898)

Gli atomi all'interfaccia occupano posizioni energeticamente sfavorevoli rispetto ai siti cristallografici. Lo spostamento da questi siti può ridurre l'energia complessiva, favorendo la formazione di uno **strato intermedio amorfo** caratterizzato da disordine strutturale simile a una fase liquida.

### Modelli Basati su Dislocazioni

#### Grano di Inclinazione (Tilt Boundary)

Due cristalli identici ma inclinati l'uno rispetto all'altro sono separati da **dislocazioni a spigolo** (*edge dislocations*). La distanza *s* tra dislocazioni consecutive è:

$$s = \frac{a}{2\sin(\theta/2)} \approx \frac{a}{\theta}$$

dove:
- *a* = costante reticolare
- *θ* = angolo di inclinazione

#### Grano di Torsione (Twist Boundary)

Due cristalli ruotati uno rispetto all'altro sono raccordati tramite **dislocazioni a vite** (*screw dislocations*), che acomodano la rotazione relativa.

#### Interfaccia Eterofase (Eteroepitassia)

Nel caso di disadattamento reticolare (*lattice mismatch*) tra film (costante reticolare *a*) e substrato (costante reticolare *b*), si formano dislocazioni a spigolo con distanza:

$$s = \frac{ab}{|b - a|}

$$

Minore è il mismatch, maggiore è la distanza tra dislocazioni e minore la densità di difetti.

## Strain versus Dislocazioni: Spessore Critico

Nei film epitassiali sottili con basso mismatch, il disadattamento reticolare può essere accomodato attraverso due meccanismi competitivi:

### Meccanismi di Accomodamento

1. **Deformazione elastica (strain)**: il film si adatta al substrato deformandosi elasticamente
   - Energia associata: **E_ε** (cresce con lo spessore *h* del film)

2. **Formazione di dislocazioni**: rilassamento tramite difetti cristallini
   - Energia associata: **E_D** (indipendente da *h*)

### Spessore e Mismatch Critici

La scelta del meccanismo dipende da:
- **Spessore del film** (*h*)
- **Entità del disadattamento** (|b − a|)/a

**Regime di film sottile** (h < h₀): la deformazione elastica è energeticamente favorevole

**Regime di film spesso** (h > h₀): la formazione di dislocazioni diventa conveniente

Con l'aumentare del mismatch, l'interazione tra dislocazioni (sovrapposizione dei campi di strain) riduce ulteriormente l'energia, favorendo la nucleazione di dislocazioni anche a spessori inferiori.

## Confronto Teoria-Esperimento

Per sistemi reali come Si₁₋ₓGeₓ su Si, gli spessori critici sperimentali risultano **significativamente superiori** alle previsioni teoriche. Questo discrepanza dimostra l'importanza cruciale delle **limitazioni cinetiche** nel determinare il rilassamento del mismatch, inclusi fattori quali:
- Dettagli del processo di nucleazione delle dislocazioni
- Temperatura del substrato
- Condizioni di crescita del film