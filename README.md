# -SPI-CanBus

_Appunti su approfondimento su argomenti SPI e CAN BUS per lezione di Telecomunicazioni_

## SPI
**Serial Peripheral Interface**

### Definizione
Comunicazione seriale tra un microcontrollore e altri microcontrollori o periferiche come sensori, display...  
**Bus standard di comunicazione** ideato da Motorola.

### Trasmissione
Full-duplex: i dati possono essere inviati e ricevuti contemporaneamente.  
Il master manda segnale di clock per iniziare e poi per terminare.

### Linee di comunicazione
- **SCLK (Serial Clock)**: segnale di clock generato dal master.
- **MOSI (Master Out Slave In)**: dati inviati dal master allo slave.
- **MISO (Master In Slave Out)**: dati inviati dallo slave al master.
- **SS/CS (Slave Select/Chip Select)**: usata per selezionare lo slave attivo.

### Caratteristiche principali
- Alta velocità di trasferimento dati.
- Può connettere più dispositivi usando linee dedicate.
- Supporta lunghezze di dati configurabili, tipicamente 8 bit.

### Pro e Contro
| Pro                                     | Contro                                           |
|-----------------------------------------|--------------------------------------------------|
| Velocità di trasferimento dati elevata | Più linee di comunicazione richieste             |
| Implementazione facile                 | Brevi distanze                                   |

## CAN Bus
**Controller Area Network**

### Definizione
Protocollo di comunicazione seriale per microcontrollori e dispositivi elettronici.

### Uso
Usato in automobili, macchinari industriali, e automazione, per consentire la comunicazione tra centraline.

### Caratteristiche principali
- **Architettura**: MULTI-MASTER, basata su priorità dei messaggi.
- **Velocità**: Fino a 1 Mbps.
- **Affidabilità**: Controllo degli errori integrato.
- **Cablaggio**: Due cavi: CAN_H e CAN_L per comunicazione differenziale.
- **Standard ISO 11898**

### Pro e Contro
| Pro                                                       | Contro                                                                 |
|-----------------------------------------------------------|------------------------------------------------------------------------|
| Affidabilità: Eccellente rilevamento e correzione degli errori. | Velocità limitata: Non adatto per applicazioni con richieste di larghezza di banda molto elevate. |
| Robustezza: Resiste al rumore elettrico grazie alla comunicazione differenziale. | Lunghezza del bus: Raggio limitato a velocità elevate (poche decine di metri a 1 Mbps). |
| Efficienza: Prioritizzazione dei messaggi; i più importanti hanno accesso immediato al bus. | Sicurezza: Mancanza di crittografia integrata; vulnerabile a intercettazioni o attacchi. |
| Costo: Economico per implementazioni su larga scala.      | Diagnosi complesse: Risoluzione dei problemi su reti CAN può essere difficile senza strumenti avanzati. |
| Flessibilità: Supporta un'ampia varietà di dispositivi sulla stessa rete. |                                                                        |
