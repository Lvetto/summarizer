# Nucleazione e Crescita di Film Sottili

## Concetti Generali

La [[Nucleazione e Crescita di Film Sottili]] rappresentano i processi fondamentali nella deposizione di materiali su substrati. Questi processi determinano la [[Struttura e Morfologia di Superfici e Interfacce]], le proprietà e la qualità finale del film e sono governati da fattori termodinamici e cinetici.

## Fasi Principali della Deposizione

### Nucleazione
La nucleazione è la formazione dei primi nuclei (isole) del materiale depositato sulla superficie del substrato. Questo processo è critico perché:
- Determina la densità e le dimensioni dei nuclei iniziali
- Dipende dalle condizioni termodinamiche e cinetiche
- Influenza direttamente la qualità e la morfologia del film finale

### Crescita
Una volta nucleati, gli atomi depositati si distribuiscono sulla superficie e si integrano nella struttura cristallina, formando gradualmente uno strato continuo.

## Processi Atomici nella Crescita

Le particelle provenienti dalla fase vapore, descritte dal flusso:

$$r = p(2\pi MkT_0)^{-1/2}$$

una volta condensate sulla superficie, possono:
- Rievaporarsi immediatamente
- Diffondere sulla superficie
- Adsorbire in siti specifici (difetti, bordi)
- Rievaporarsi dopo la diffusione

La velocità di desorbimento segue una legge esponenziale di tipo Arrhenius:

$$v \propto \exp(E_{des}/kT)$$

Temperature elevate e alta mobilità superficiale sono necessarie per ottenere superfici lisce, consentendo l'interdiffusione tra substrato e film che liscia l'interfaccia.

## Natura Non-Equilibrio della Crescita

La crescita dei film è un processo cinetico non-equilibrio. In equilibrio termodinamico, tutti i processi procederebbero in direzioni opposte con velocità uguali (detailed balance), impedendo la crescita netta. Lo stato finale del film dipende dal percorso seguito attraverso i vari processi ed è determinato cineticamente, non necessariamente dal configurazione più stabile termodinamicamente.

## Tre Modalità di Crescita

Esistono tre modalità distinte di crescita dei film, classificate in base all'energia relativa tra le diverse interfacce:

### 1. Layer-by-Layer (Frank-van der Merve, FM)
- L'interazione substrato-layer è più forte dell'interazione tra layer atomici vicini
- Ogni nuovo strato inizia solo quando il precedente è completo
- Caratterizzato da soppressione significativa del segnale del substrato durante la crescita

### 2. Island Growth (Volmer-Weber, VW)
- L'interazione tra atomi del film è più forte dell'interazione film-substrato
- Si formano isole multilayer isolate
- Caratterizzato da aumento lento e graduale dei segnali con aree substrato prive di deposito

### 3. Layer-plus-Island (Stranski-Krastanov, SK)
- Caso intermedio tra i due precedenti
- Dopo la formazione di uno o più strati monocristallini completi, si innesca la crescita isolare 3D
- Può essere dovuto a disadattamento reticolare o differenze di simmetria/orientazione
- Caratterizzato da aumento lineare fino a 1-2 monostrati, seguito da crescita più lenta

## Analisi Termodinamica mediante Energie Superficiali

La distinzione tra modalità di crescita può essere formalizzata usando le energie libere superficiali (γ). L'equilibrio delle forze al punto di contatto tra substrato e isola 3D è descritto da:

$$\gamma_S = \gamma_{S/F} + \gamma_F \cos\varphi$$

dove:
- γ_S = energia libera substrato-vuoto
- γ_F = energia libera film-vuoto
- γ_{S/F} = energia libera substrato-film

Le condizioni limite sono:

**Per crescita layer-by-layer:**
$$\gamma_S \geq \gamma_F + \gamma_{S/F}$$

**Per crescita isolare:**
$$\gamma_S < \gamma_F + \gamma_{S/F}$$

## Ruolo della Supersaturazione

Considerando l'equilibrio con la fase vapore, il cambio di entalpia libera di Gibbs nel trasferimento di una particella dal vapore al solido è:

$$\Delta G = nkT \ln(p/p_0)$$

Il rapporto ζ = p/p₀ è il grado di supersaturazione, la "forza motrice" per la formazione del film. Le condizioni per la crescita si modificano come:

**Per crescita layer-by-layer:**
$$\gamma_S \geq \gamma_F + \gamma_{S/F} + CkT \ln(p_0/p)$$

**Per crescita isolare:**
$$\gamma_S < \gamma_F + \gamma_{S/F} + CkT \ln(p_0/p)$$

La supersaturazione consente la crescita anche in condizioni termodinamicamente sfavorevoli.

## Modello Capillare della Nucleazione

### Nucleazione 3D (Crescita di Isole)

Per un nucleo emisferico con raggio r, l'energia libera di Gibbs è:

$$G_{3D} = -\frac{1}{2}\frac{4}{3}\pi r^3 \Omega^{-1}\mu + 2\pi r^2 \gamma_F + \pi r^2(\gamma_{S/F} - \gamma_S)$$

La dimensione critica è data da:

$$j_{cr} = \left(\frac{2X}{3\mu}\right)^3$$

$$G_{3D}(j_{cr}) = \frac{4}{27}\frac{X^3}{\mu^2}$$

dove X è una costante energetica superficiale.

**Caratteristica:** Richiede μ > 0, quindi la supersaturazione è obbligatoria per la nucleazione 3D.

### Nucleazione 2D (Crescita per Strati)

Per la nucleazione bidimensionale su una superficie piana, interviene l'energia di bordo γ_E. L'energia libera di Gibbs per un nucleo circolare planare a singolo strato è:

$$G_{2D} = -\pi r^2 a \Omega^{-1}\mu + \pi r^2 a \Omega^{-1/3}(\gamma_F + \gamma_{S/F} - \gamma_S) + 2\pi r \gamma_E$$

La dimensione critica è:

$$j_{cr} = \left(\frac{Y}{2\bar{\mu}}\right)^2$$

$$G_{2D}(j_{cr}) = \frac{1}{4}\frac{Y}{\bar{\mu}}$$

dove:

$$\bar{\mu} = \mu - (\gamma_F + \gamma_{S/F} - \gamma_S)\Omega^{2/3}$$

è una quantità effettiva per la crescita 2D.

**Caratteristica:** Può procedere con μ̄ > 0 anche con μ ≤ 0, consentendo la crescita in condizioni di sottosaturazione.

## Velocità di Nucleazione

La velocità di formazione dei nuclei critici segue:

$$J_N = K \exp\left(-\frac{G(j_{cr})}{kT}\right)$$

dove il fattore pre-esponenziale K dipende dalla frequenza di arrivo degli atomi. All'aumentare della sovrasaturazione ζ, il numero di atomi nel nucleo critico diminuisce, causando nuclei più piccoli ma in numero maggiore. Nelle deposizioni in vuoto ad alta sovrasaturazione e bassa temperatura, la dimensione critica può contenere pochi atomi.

## Fattori Influenti sulla Crescita

- **Energia di superficie e interfaccia**: Determina le modalità di crescita
- **Temperatura del substrato**: Influenza la mobilità superficiale e le velocità di desorbimento
- **Parametri di deposizione**: Velocità di deposizione, pressione del gas, flusso di particelle
- **Natura del substrato**: Affinità chimico-fisica con il materiale depositato, disadattamento reticolare
- **Condizioni di equilibrio termodinamico**: Grado di sovrasaturazione

## Tecniche Sperimentali di Caratterizzazione

### Spettroscopia di Superficie (AES/XPS)
Durante la crescita di monostrati, l'intensità del segnale cambia linearmente con la copertura. L'inviluppo della curva, composto da segmenti lineari, è descritto da funzioni esponenziali. Consente di distinguere le tre modalità di crescita, anche se sono necessarie informazioni complementari da altre tecniche.

### Tecniche di Diffrazione
- **LEED/RHEED**: Forniscono informazioni su ordine cristallografico. RHEED distingue tra crescita 2D (strisce) e 3D (spots)

### Microscopia in Spazio Reale
- **SEM**: Risoluzione laterale fino a 10 Å, generalmente eseguito ex situ
- **STM**: Risolve strutture a livello atomico sia lateralmente che verticalmente (risoluzione in Ångström), operante in situ
- **TEM**: Analizza nucleazione 3D, dislocazioni e struttura atomica delle interfacce ad alta risoluzione

### Metodi Ottici
- **Raman**: Studia proprietà vibrazionali; la larghezza delle linee rivela il grado di ordine cristallografico
- **Ellissometria**: Misura il cambio di polarizzazione alla riflessione con sensibilità superficiale (<0.1 monostrati); l'ellissometria spettroscopica fornisce informazioni sulla struttura elettronica e sulla natura chimica

### Ion Scattering (RBS)
Fornisce analisi chimica, informazioni su qualità cristallografica, rilassamenti, mismatch reticolare e strain.

## Esempi Sperimentali

- **InSb(110)-Sn**: Mostra crescita FM con comportamento esponenziale su più di un ordine di grandezza
- **GaAs(110)-Sn**: Esibisce crescita SK con formazione di uno strato amorfo e isole emi-sferiche con diametri di centinaia di Ångström