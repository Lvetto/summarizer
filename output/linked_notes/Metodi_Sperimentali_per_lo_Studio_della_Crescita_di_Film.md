# Metodi Sperimentali per lo Studio della Crescita di Film

## Analisi AES/XPS dei Modi di Crescita

### Caratteristiche dei Tre Modi di Crescita

La [[spettroscopia Auger (AES)]] e la fotoelettronica a raggi X (XPS) permettono di distinguere i tre modi di crescita attraverso l'andamento caratteristico dei segnali:

**[[Crescita Frank-van der Merwe (FM)]] – strato per strato:**
- Il segnale del substrato decresce esponenzialmente con la copertura
- Il segnale del film aumenta esponenzialmente
- Durante la crescita di ogni monostrato la variazione è lineare
- Per emissione non normale, il cammino libero medio λ deve essere corretto come λ·cos δ (dove δ è l'angolo rispetto alla normale)

**[[Crescita Stranski-Krastanov (SK)]] – isole su strato:**
- Variazione lineare fino a uno o pochi monostrati
- Cambio di pendenza caratteristico
- Successivamente decadimento molto più lento dovuto alla formazione di isole sul primo strato completo

**Crescita Volmer-Weber (VW) – isole:**
- Decadimento molto lentamente del segnale del substrato
- Aumento lento del segnale del film
- Grandi aree del substrato rimangono scoperte

### Limitazioni e Integrazioni Necessarie

AES/XPS da sole non sempre consentono di distinguere univocamente i tre modi. Sono necessarie:
- Tecniche complementari ([[SEM]], [[LEED]], [[RHEED]])
- Calcoli modellistici con geometrie di isole semplificate

---

## Esempi Sperimentali

### InSb(110)-Sn (Crescita FM)
- Il segnale AES dell'In decresce esponenzialmente su più di un ordine di grandezza
- Cammino libero medio degli elettroni a 400 eV: ~10 Å
- Il segnale del Sn satura intorno a 10 monostrati

### GaAs(110)-Sn (Crescita SK)
- Cambio di pendenza nel segnale Ga a 1-2 monostrati
- Modello: strato chiuso amorfo di β-Sn (~3 Å) con isole emisferiche sovrastanti
- Conferma SEM: a copertura di 38 ML si osservano isole con diametro di qualche centinaio di Ångström

### Tabella Generale dei Sistemi
- **Metalli su metalli**: prevalentemente FM
- **Metalli su semiconduttori**: tendono a SK
- **Metalli su alogenuri alcalini, MgO, grafite**: prevalentemente VW

**Nota importante:** Il modo di crescita dipende dalla temperatura del substrato e può variare al di fuori di specifici intervalli termici.

---

## Tecniche di Caratterizzazione

### Tecniche di Diffrazione

**[[LEED (Low-Energy Electron Diffraction)]]:**
- Fornisce informazioni sull'ordine cristallografico a scale di ~centinaia di Ångström (lunghezza di coerenza del fascio)
- Spot affilati indicano ordine locale, non necessariamente a lungo raggio

**[[RHEED (Reflection High-Energy Electron Diffraction)]]:**
- Distingue crescita 2D (strisce di diffrazione) da crescita 3D a isole (spot)
- Fornisce informazioni dirette sul modo di crescita

### Tecniche Microscopiche

**[[SEM (Scanning Electron Microscopy)]]:**
- Risoluzione laterale: ~10 Å
- Generalmente ex situ
- Contrasto originato da fattori geometrici e proprietà elettroniche (funzione lavoro, densità di stati superficiali)

**[[STM (Scanning Tunneling Microscopy)]]:**
- Misura la corrente di tunneling tra punta metallica e superficie
- Risoluzione angstrom sia lateralmente che verticalmente
- Sonda il contorno della densità elettronica esterna

**TEM (Transmission Electron Microscopy):**
- Studio di dislocazioni (orientamento leggermente fuori dalla condizione di Bragg)
- Alta risoluzione per la struttura atomica delle interfacce
- Richiede preparazione di sezioni sottili (10–100 nm) tramite attacco chimico e ion milling

### Tecniche Ottiche

**Spettroscopia Raman:**

Permette di caratterizzare lo stato cristallino del film:

- **Film cristallini**: linee fononi strette (Δν ~ 10 cm⁻¹), per cristalliti con diametro > 100–150 Å
- **Film policristallini**: linee allargate a causa della parziale violazione della conservazione del vettore d'onda
- **Film amorfi**: struttura larga e continua (assenza di simmetria traslazionale consente contribuzione da tutta la zona di Brillouin)

*Esempio:* Sb su GaAs(110) deposito a 300 K forma film policristallini per θ' > 10 ML e amorfi per θ' < 10 ML; a 90 K i film sono amorfi a qualsiasi copertura.

**Ellissometria:**

Misura il cambiamento dello stato di polarizzazione della luce riflessa attraverso la quantità complessa:

$$\rho = \frac{r_\parallel}{r_\perp} = \tan\psi \, e^{i\Delta}$$

dove Δ e ψ sono gli angoli ellissometrici.

- Fornisce le funzioni dielettriche del film (Re{ε_f}, Im{ε_f})
- Sensibilità superficiale < 0.1 monostrati
- In tecnologia applicata: misura spessori di film tramite formule di Fresnel

*Esempio:* Nel sistema InSb(110)-Sn, l'ellissometria rivela che per coperture < ~500 Å il Sn è nella forma semiconduttrice α-Sn; per coperture maggiori si deposita come β-Sn metallico.

### Ion Scattering (RBS – Rutherford Backscattering)

L'analisi energetica degli ioni retrodiffusi (energia primaria 5 keV – 5 MeV) fornisce:
- Analisi chimica degli strati superficiali
- Informazioni sulla qualità cristallografica
- Rilassamenti, [[mismatch reticolare]] e tensioni interne (tramite shadowing e blocking in direzioni cristallografiche specifiche)

---

## Conclusione

Lo studio della crescita di film richiede l'impiego complementare di molteplici tecniche, dalle analisi spettroscopiche superficiali (AES/XPS) alle tecniche di diffrazione (LEED/RHEED), dalla microscopia ad alta risoluzione (STM/TEM) alle caratterizzazioni ottiche (Raman/ellissometria) e all'ion scattering. Questa combinazione metodologica consente una caratterizzazione completa del modo di crescita e delle proprietà strutturali ed elettroniche dei film.