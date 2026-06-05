# Nucleazione e Modi di Crescita dei Film Sottili

## Processi Atomici nella Crescita dei Film

La crescita di un film su substrato solido è governata da diversi processi atomici fondamentali. Le particelle provenienti dalla fase vapore condensano sulla superficie con un flusso dato da:

$$r = p(2\pi M k T_0)^{-1/2}$$

Una volta condensata, una particella può **ri-evaporare** seguendo una legge di tipo Arrhenius:

$$v \propto \exp(E_{des}/kT)$$

oppure **diffondere** lungo la superficie, adsorbendosi in siti speciali come difetti e bordi.

La crescita cristallina è un **processo cinetico di non-equilibrio**: in equilibrio termodinamico, condensazione e ri-evaporazione si bilanciano (principio del bilancio dettagliato) e non vi è crescita netta. Lo stato finale è quindi determinato cineticamente, non dal minimo energetico globale. Per ottenere superfici lisce è necessaria un'elevata mobilità superficiale, dunque temperature elevate.

## I Tre Modi di Crescita

Esistono tre modalità principali di crescita dei film sottili, classificate sulla base dell'interazione relativa tra substrato-film e film-film:

### 1. Layer-by-Layer (Frank-van der Merwe, FM)
L'interazione substrato-film è più forte di quella film-film. Ogni nuovo strato inizia solo dopo il completamento del precedente, producendo una crescita planare strato per strato.

### 2. Island Growth (Volmer-Weber, VW)
L'interazione film-film supera quella substrato-film. Si formano direttamente aggregati tridimensionali (isole multilayer) sulla superficie del substrato.

### 3. Layer-plus-Island (Stranski-Krastanov, SK)
Dopo la formazione di uno o più monostrati completi, si avvia la crescita di isole tridimensionali. Questo comportamento è spesso causato dal **mismatch reticolare** tra film e substrato: la deformazione elastica accumulata supera progressivamente le forze di adesione oltre una certa soglia spaziale.

## Criterio Energetico per i Modi di Crescita

L'equilibrio delle forze in un punto di contatto tra un'isola 3D e il substrato fornisce l'equazione di Young:

$$\gamma_S = \gamma_{S/F} + \gamma_F \cos\phi$$

dove $\gamma_S$, $\gamma_F$ e $\gamma_{S/F}$ sono le energie libere superficiali delle interfacce substrato-vuoto, film-vuoto e substrato-film rispettivamente.

Le condizioni per i due modi limite sono:

- **Crescita a strati (FM):** $\phi = 0$, $\quad \gamma_S \geq \gamma_F + \gamma_{S/F}$
- **Crescita a isole (VW):** $\phi \neq 0$, $\quad \gamma_S < \gamma_F + \gamma_{S/F}$

## Ruolo della Fase Vapore e Supersaturazione

Il trasferimento di una particella dal vapore al solido a pressione $p \neq p_0$ comporta una variazione di entalpia libera di Gibbs:

$$\Delta G = n\Delta\mu = nkT\ln(p/p_0)$$

Il rapporto $\zeta = p/p_0$ definisce il **grado di supersaturazione**, una delle forze trainanti della crescita del film. Le condizioni energetiche si modificano in:

- **Crescita a strati:** $\gamma_S \geq \gamma_F + \gamma_{S/F} + CkT\ln(p_0/p)$
- **Crescita a isole:** $\gamma_S < \gamma_F + \gamma_{S/F} + CkT\ln(p_0/p)$

## Modello Capillare della Nucleazione

### Energia Libera per Nuclei 3D e 2D

Per un **nucleo emisferico 3D** di raggio *r*, l'entalpia libera è:

$$G_{3D} = -\frac{1}{2}\frac{4}{3}\pi r^3 \Omega^{-1}\mu + 2\pi r^2\gamma_F + \pi r^2(\gamma_{S/F} - \gamma_S)$$

Per la **nucleazione 2D** (crescita di uno strato su superficie piana), esiste un'energia di bordo $\gamma_E$ per unità di lunghezza. L'entalpia libera 2D è:

$$G_{2D} = -\pi r^2 a\Omega^{-1}\mu + \pi r^2 a\Omega^{-1/3}(\gamma_F + \gamma_{S/F} - \gamma_S) + 2\pi r\gamma_E$$

### Barriera di Nucleazione e Dimensione Critica

In entrambe le equazioni, i **termini proporzionali a μ** sono negativi e favoriscono la nucleazione, mentre gli **ultimi termini** sono positivi e costituiscono la **barriera di nucleazione**. La sovrapposizione di questi effetti genera un andamento non monotono di *G* in funzione del numero di atomi *j*, con un **massimo** alla dimensione critica *j_cr*.

- Se il nucleo supera $j_{cr}$, tende a crescere
- Se il nucleo è al di sotto di $j_{cr}$, è instabile e tende a dissolversi

### Dimensioni Critiche

**Crescita 3D:**
$$G_{3D}(j_{cr}) = \frac{4}{27}\frac{X^3}{\mu^2}, \qquad j_{cr} = \left(\frac{2X}{3\mu}\right)^3$$

**Crescita 2D:**
$$G_{2D}(j_{cr}) = \frac{1}{4}\frac{Y}{\bar{\mu}}, \qquad j_{cr} = \left(\frac{Y}{2\bar{\mu}}\right)^2$$

Per la crescita 2D, è introdotta una **quantità effettiva**:

$$\bar{\mu} = \mu - (\gamma_F + \gamma_{S/F} - \gamma_S)\Omega^{2/3}$$

### Confronto tra Crescita 2D e 3D

- La crescita **3D** richiede necessariamente **sovrasaturazione** (μ > 0)
- La crescita **2D** può avvenire anche in condizioni di **sottosaturazione** (μ ≤ 0), poiché per la crescita layer-by-layer il termine $(\gamma_F + \gamma_{S/F} - \gamma_S)$ è negativo, rendendo possibile $\bar{\mu} > 0$ anche con μ ≤ 0

### Tasso di Nucleazione

Il tasso di formazione di nuclei critici è:

$$J_N = K\exp\left(-\frac{G(j_{cr})}{kT}\right)$$

All'**aumentare della sovrasaturazione** *ζ*, la dimensione critica del nucleo diminuisce, producendo nuclei più piccoli in numero maggiore. In deposizione in vuoto (alta sovrasaturazione, bassa temperatura), il nucleo critico può contenere solo pochi atomi.