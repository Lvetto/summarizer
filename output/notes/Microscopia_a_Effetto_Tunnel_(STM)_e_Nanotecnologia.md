# Microscopia a Effetto Tunnel (STM) e Nanotecnologia

## Principio di Funzionamento

Lo Scanning Tunneling Microscope (STM) sfrutta l'effetto tunnel quantistico per ottenere immagini a risoluzione atomica. Una punta metallica viene scansionata sulla superficie del campione mediante un sistema di attuatori piezoelettrici (x, y, z), misurando la corrente tunnel che fluisce tra punta e campione. La corrente tunnel dipende sia dalla distanza punta-superficie sia dalla funzione lavoro locale, variando di un ordine di grandezza per variazioni di distanza dell'ordine di un Ångstrom.

## Architetture Strumentali

### Versione Classica
- Utilizzo di molle molto morbide per il supporto
- Smorzamento delle vibrazioni mediante correnti parassite indotte in piastre di rame da magneti permanenti
- Soppressione delle vibrazioni meccaniche a livello sub-angstrom (<1 Å)

### Versione Compatta (Besocke)
- Tre elementi piezoelettrici per il supporto del campione e controllo della distanza
- Un quarto elemento piezoelettrico centrale come scanner
- Piezoelettrici strutturati come aste con quattro elettrodi separati
- La polarizzazione degli elettrodi provoca la flessione e consente movimenti nelle tre direzioni spaziali

## Preparazione della Punta

La punta è realizzata da filo di iridio (Ir) o tungsteno (W) con diametro iniziale di 1 mm. La procedura di preparazione comprende:

1. Affilatura meccanica per ottenere un raggio di curvatura <1 µm
2. Trattamento chimico
3. Esposizione in situ a campi elettrici di 10⁸ V/cm per circa 10 minuti

Il meccanismo di formazione della punta atomica non è completamente compreso e la sua stabilità nel tempo è limitata, rappresentando una sfida tecnica significativa.

## Misurazione della Topografia e della Funzione Lavoro

### Topografia
La topografia z(x,y) si ottiene mantenendo costante la corrente tunnel IT e misurando la tensione Uz sul piezodrive z in funzione delle tensioni di scansione Ux, Uy. Poiché IT dipende fortemente dalla distanza, questo metodo fornisce una traccia accurata della struttura superficiale.

### Funzione Lavoro
La funzione lavoro media φ viene ricavata dalla derivata della corrente tunnel rispetto alla distanza:

$$\varphi \simeq \left(\frac{\partial \ln I_T}{\partial d}\right)^2$$

La misura si esegue mediante modulazione della tensione Uz e rivelazione sincrona (lock-in), registrando sia IT che la sua derivata. Questo approccio consente di distinguere variazioni topografiche da variazioni della funzione lavoro locale.

## Applicazioni alla Struttura Superficiale dei Semiconduttori

### Si(111)-(7×7)
L'immagine STM della superficie ricostruita mostra le celle unitarie attraverso i minimi profondi agli angoli. L'analisi rivela che le due metà della cella unitaria non sono equivalenti (altezze diverse di minimi e massimi), fornendo supporto sperimentale al modello ad adatomi modificato.

### Si(111)-(2×1)
Lo STM consente di sondare separatamente stati occupati e vuoti mediante il controllo della polarità della tensione applicata:

- **Bias positivo:** tunneling di elettroni dalla punta verso stati di superficie vuoti (π*)
- **Bias negativo:** tunneling di elettroni dagli stati di superficie occupati (π) verso la punta

La spaziatura misurata (~6.9 Å) è compatibile con il **modello a catene π** e non con il modello a buckling. La misura della caratteristica differenziata dIT/dU fornisce la distribuzione spettrale degli stati di superficie occupati e vuoti, in accordo quantitativo con i picchi previsti dagli stati π e π*.

## Nanotecnologia: dalla Visualizzazione alla Manipolazione

Lo STM e l'Atomic Force Microscope (AFM) correlato hanno aperto la strada alla nanotecnologia vera e propria, consentendo di passare dall'osservazione alla manipolazione diretta della materia a scala atomica.

### Scrittura e Indentazione
Scansionando la punta a contatto con la superficie è possibile:
- Tracciare linee sub-micrometriche sulla superficie
- Produrre indentazioni controllate (fori di 2–10 nm su silicio con punta di tungsteno)

### Manipolazione di Singoli Atomi
Eigler e Schweizer (1990) hanno dimostrato la manipolazione controllata di singoli atomi di Xe su Ni(110) a bassa temperatura in Ultra-High Vacuum, sviluppando due tecniche complementari:

**Sliding:** La punta viene avvicinata all'atomo aumentando l'interazione mediante forze di Van der Waals, quindi traslata lateralmente a corrente costante trascinando l'atomo, e infine ritirata lasciando l'atomo nella nuova posizione.

**Pushing:** La punta viene abbassata sull'atomo fino a raggiungere una forte interazione, quindi spostata trascinando l'atomo. La barriera di diffusione è approssimativamente 1/10 dell'energia di legame atomico.

### Quantum Corral
Crommie et al. hanno costruito un anello di 48 atomi di ferro su Cu(111) a 4 K con raggio 71.3 Å, dimostrando la possibilità di assemblare nanostrutture artificiali atomo per atomo. Questa struttura confina gli elettroni di conduzione creando stati quantici discreti (quantum confinement), segnando l'inizio della nanofabbricazione controllata.