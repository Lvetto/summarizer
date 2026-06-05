# Microscopia Elettronica e Tecniche di Microanalisi

## Microscopia Elettronica a Scansione (SEM)

### Principio di Funzionamento
Lo SEM utilizza un fascio di elettroni primari ad alta energia (E₀) per irradiare la superficie di un campione. L'intensità degli elettroni emessi dal campione viene amplificata e proiettata su uno schermo TV, creando un'immagine della superficie.

### Distribuzione Energetica degli Elettroni Emessi

La superficie irradiata emette elettroni di diverse origini, classificabili in quattro regioni energetiche:

- **Regione I - Elettroni elasticamente retrodiffusi**: mantengono l'energia E₀ del fascio primario
- **Regione II - Elettroni inelasticamente retrodiffusi**: subiscono perdite di energia per eccitazioni di plasmoni e transizioni interbanda (specifiche del materiale). Forniscono immagini altamente sensibili alla composizione ma con forti effetti di ombreggiatura
- **Regione III - Righe Auger**: banda piatta fino a ~50 eV che rivela le righe caratteristiche di emissione Auger per ogni elemento chimico
- **Regione IV - Elettroni secondari veri**: elettroni a bassa energia (0-50 eV) provenienti da scattering multiplo. Producono immagini topografiche della superficie con minore contrasto chimico ma buona visibilità di rugosità e variazioni di funzione lavoro

### Tecniche di Microanalisi Associata

Il fascio primario induce processi che permettono analisi chimiche spazialmente risolte:

- **[[Spettroscopia Auger]]**: gli analizzatori di elettroni (es. CMA) rilevano i processi Auger
- **Spettroscopia a Raggi X**: rivelatori a dispersione di energia (EDS) rilevano l'emissione di raggi X

Un apparato equipaggiato con queste tecniche è denominato **microprobe**.

### Profondità di Informazione

Le diverse tecniche forniscono informazioni a profondità differenti:

| Tecnica | Profondità |
|---------|-----------|
| Sonda a Raggi X | 0,1-10 µm (debole assorbimento consente penetrazione profonda) |
| Sonda Auger | 10²-10⁴ volte inferiore ai raggi X (limitata dalla libera distanza percorsa degli elettroni Auger) |

La zona di origine ha forma caratteristica a "pera": gli elettroni retrodiffusi e i raggi X originano dalla zona apicale, mentre gli elettroni secondari a bassa energia e gli elettroni Auger provengono dalla ristretta regione superficiale (il "collo" della pera).

### Limitazioni e Sviluppi Recenti

- Gli SEM standard operano sottovuoto (~10⁻⁵ Pa)
- Recenti sviluppi hanno prodotto SEM che operano in condizioni [[Tecnologie e Sistemi di Ultra-Alto Vuoto (UHV)|UHV]], collegabili via camere di trasferimento ad altri apparati per analisi in situ

---

## Microscopia a Tunneling (STM)

### Configurazione Strumentale

Lo STM utilizza un ago metallico scansionato sulla superficie del campione mediante attuatori piezoelettrici controllati nelle tre direzioni (x, y, z). 

**Configurazioni principali:**
- **Strumenti classici**: posizionatore grossolano per l'avvicinamento iniziale del campione, sistema isolato dalle vibrazioni esterne
- **Configurazioni moderne** (es. microscopio di Besocke): tre elementi piezoelettrici fungono da porta-campione e controllo della distanza, un quarto elemento piezoelettrico centrale funge da scanner per il movimento dell'ago

**Prestazioni**: accuratezza migliore di 1 Ångstrom su aree tipicamente di 100 × 100 Å²

### Sfide Sperimentali

1. **Soppressione delle vibrazioni meccaniche**: devono essere inferiori a 1 Ångstrom, ottenuto tramite sospensioni morbide e correnti di Foucault
2. **Preparazione del tip atomico**: realizzato da filo di Ir o W (1 mm di diametro), macinato a raggio di curvatura <1 µm, seguito da trattamento chimico ed esposizione a campi elettrici di 10⁸ V/cm per ~10 minuti

### Principio di Misura

La corrente di tunneling (I_T) dipende dalla distanza d tra ago e superficie e dalla [[Struttura e Morfologia di Superfici e Interfacce|funzione lavoro]] φ. Due modalità di misura principale:

- **Misura della corrugazione topografica**: mantenendo I_T costante, la tensione U_z del piezocomando z viene misurata in funzione di U_x e U_y, ottenendo la topografia z(x,y)
- **Misura della funzione lavoro**: mediante modulazione della distanza d e rilevamento sincronizzato secondo la relazione:

$$\varphi \simeq \left(\frac{\partial \ln I_T}{\partial d}\right)^2$$

### Applicazioni Strutturali

**Superficie Si(111)-(7 × 7)**: le immagini STM rivelano chiaramente le celle unitarie e mostrano che i due semi-reticoli non sono completamente equivalenti, confermando il modello dell'adatomo modificato.

**Superficie Si(111)-(2 × 1)**: variando la polarità del bias è possibile sondare separatamente gli stati occupati e vuoti. La conduttanza differenziale (dI_T/dU) fornisce informazioni sulla densità degli stati superficiali, con buon accordo con le previsioni teoriche.

### Nanotecnologia

Lo STM (insieme all'AFM) ha reso possibile il controllo di atomi e molecole a scala nanometrica:

- **Scratching**: movimentare l'ago crea linee sub-micrometriche sulla superficie
- **Indentazioni**: aumentando l'interazione tip-campione
- **Manipolazione di atomi singoli**: tramite forze di van der Waals, gli atomi possono essere trascinati o spinti sulla superficie in ultravuoto a bassa temperatura (esempio: atomi di Xe su Ni(110))
- **Nanostrutture artificiali**: il "quantum corral" costituito da 48 atomi di Fe arrangiati in anello su Cu(111) con raggio di 71.3 Å rappresenta un'applicazione notevole della manipolazione atomica