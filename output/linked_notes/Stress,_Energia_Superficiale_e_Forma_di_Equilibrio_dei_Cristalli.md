# Stress, Energia Superficiale e Forma di Equilibrio dei Cristalli

## Tensore dello Stress Superficiale

Lo stress superficiale emerge dalla redistribuzione della carica elettronica quando si crea una nuova superficie, alterando le forze sugli atomi negli strati superficiali. Viene definito attraverso l'integrazione della differenza tra lo stress locale e lo stress del bulk:

$$\tau^{(s)}_{ij} = \int_{-\infty}^{\infty} dz \left[ \tau_{ij}(z) - \tau^{(b)}_{ij} \right]$$

**Caratteristiche principali:**
- Ha dimensioni di **forza per unità di lunghezza** (N/m), diversamente dallo stress nel bulk (N/m²)
- È confinato entro circa 1 nm dalla superficie
- Assume valori tipici dell'ordine di 1 N/m
- Può essere **tensile** (positivo, la superficie tende a contrarsi) o **compressivo** (negativo)

## Energia Libera Superficiale e Relazione di Shuttleworth

L'**energia libera superficiale specifica** γ rappresenta l'eccesso di energia libera per unità di area superficiale e corrisponde al lavoro reversibile per formare una nuova superficie a volume, temperatura, potenziale chimico e numero di componenti costanti.

La variazione dell'energia libera superficiale totale è:

$$\delta F^{(s)} = \gamma\,\delta A + A\,\delta\gamma$$

dove:
- Il termine $\gamma\,\delta A$: descrive la variazione dovuta al cambio dell'area superficiale a configurazione atomica fissa
- Il termine $A\,\delta\gamma$: rappresenta la variazione dovuta a cambiamenti nelle distanze interatomiche ([[Rilassamento, Ricostruzione e Difetti delle Superfici|ricostruzioni]]) a numero di atomi costante

### La Relazione di Shuttleworth

La connessione tra stress superficiale ed energia superficiale è fornita dall'**equazione di Shuttleworth**:

$$\tau^{(s)}_{ij} = \gamma\,\delta_{ij} + \frac{\partial \gamma}{\partial \varepsilon_{ij}}$$

**Distinzioni fondamentali:**
- **Nei liquidi**: $\partial\gamma/\partial\varepsilon = 0$ (assenza di resistenza alla deformazione plastica), quindi $\tau^{(s)} = \gamma$
- **Nei solidi**: il termine $\partial\gamma/\partial\varepsilon = \tau^{(s)} - \gamma$ costituisce una **forza termodinamica** che guida il flusso di atomi verso la superficie e favorisce le ricostruzioni superficiali

## Dipendenza Orientazionale dell'Energia Superficiale

L'energia superficiale γ dipende fortemente dall'**orientazione cristallografica** (hkl) della superficie. Questa dipendenza riflette:
- Il numero di legami atomici rotti dalla creazione della superficie
- Gli effetti di compensazione di carica
- La geometria specifica di ogni faccia cristallina

La variabilità orientazionale ha conseguenze cruciali sulla forma di equilibrio dei cristalli.

## Forma di Equilibrio e Costruzione di Wulff

La forma di equilibrio di un cristallo a volume e potenziale chimico fissi è determinata dalla minimizzazione dell'energia libera totale:

$$\int_A \gamma(\mathbf{n})\, dA = \text{minimo}$$

### Metodo Costruttivo di Wulff

La **costruzione di Wulff** permette di determinare geometricamente la forma di equilibrio:

1. Si grafica γ(hkl) in coordinate polari, ottenendo il "plot di Wulff"
2. Si traccia una linea perpendicolare a ciascun vettore raggio nel punto in cui interseca la curva
3. L'**inviluppo interno** di tutti questi piani perpendicolari definisce la forma di equilibrio del cristallo

**Caso isotropo:** Per liquidi e solidi amorfi, dove γ è indipendente dall'orientazione, la forma di equilibrio è una **sfera**.

## Superfici Vicinali

Una superficie vicinale si forma inclinando leggermente un cristallo rispetto a un piano principale. Per una superficie inclinata di un angolo θ rispetto al piano (01), l'energia superficiale può essere espressa come:

$$\gamma(\theta) = \cos\theta \left[ \gamma_0 + \gamma_1 \frac{\tan\theta}{a} + \gamma_2 \left(\frac{\tan\theta}{a}\right)^2 + \cdots \right]$$

**Nel limite di piccoli angoli** (trascurando le interazioni tra gradini):

$$\gamma(\theta) = \gamma_0 \cos\theta + \frac{\gamma_1}{a} \sin\theta$$

Nel plot di Wulff, questa relazione corrisponde a un **cerchio passante per l'origine**, descrivibile dall'equazione $\gamma = 2R\cos(\theta - \Theta)$.

## Implicazioni Fisiche e Fenomeni Correlati

### Faccettatura

La dipendenza orientazionale di γ può portare a **faccettatura spontanea**: anche quando aumenta l'area totale superficiale, il cristallo può ridurre la sua energia libera esponendo preferibilmente piani a bassa energia superficiale.

### Segregazione Superficiale

Fenomeni come la segregazione atomica in superficie possono essere interpretati come processi di minimizzazione dell'energia totale attraverso l'esposizione di piani caratterizzati da valori più bassi di γ.