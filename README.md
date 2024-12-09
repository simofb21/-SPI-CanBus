# -SPI-CanBus
<i>Appunti su approfondimento su argomenti  SPI e CAN BUS per lezione di Telecomunicazioni</i> <br>

<h2>SPI</h2> 
 <b>Serial periphiral interface</b> <br>
 <h3>Definizione : </h3> comunicazione seriale tra un microcontrollore e  altri microcontrollori o periferiche come sensori, display ... <br>
 <b>bus standard di comunicazione</b> ideato da motorola <br>
 <h3>Trasmissione : </h3> Full-duplex: i dati possono essere inviati e ricevuti contemporaneamente. <br>
 Il master manda segnale di clock per iniziare e poi per terminare <br>
 
 <h3>Linee di comunicazione </h3>
 <ul>
  <li><b>SCLK (Serial Clock)</b>: segnale di clock generato dal master.</li>
  <li><b>MOSI (Master Out Slave In)</b>: dati inviati dal master allo slave.</li>
  <li><b>MISO (Master In Slave Out)</b>: dati inviati dallo slave al master.</li>
  <li> <b>SS/CS (Slave Select/Chip Select)</b>: usata per selezionare lo slave attivo. </li>
 </ul>
 <h3>Caratteristiche principali</h3>
 <ul>
  <li>Alta velocità di trasferimento dati.</li>
  <li>Può connettere più dispositivi usando linee dedicate.</li>
  <li>Supporta lunghezze di dati configurabili, tipicamente 8 bit.</li>
 </ul>
 <table border="1">
  <tr>
   <th>Pro</th>
   <th>Contro</th>
  </tr>
  <tr>
   <td>Velocità di trasferimento dati elevata </td>
   <td>Più linee di comunicazione richieste</td>
   </tr>
  <tr>
   <td>Implementazione facile</td>
   <td>Brevi distanze</td>
  </tr>
 </table>

<h2> CAN Bus </h2>  Controller Area Network <br>
 <h3>Definizione: </h3>
  Protocollo di comunicazione seriale per microcontrollori e dispositivi elettronici <br>
 <h3>Uso </h3> Usato in automobili, macchinari industriali, e automazione , per consentire la comunicazione tra centraline <br>
 <h3>Caratteristiche principali</h3>
 <ul>
  <li><b>Architettura</b> : MULTI-MASTER , basata su priorità dei messaggi </li>
  <li><b>Velocità</b> : Fino a 1  Mbps </li>
  <li><b>Affidabilità</b>:  Controllo degli errori integrato </li>
  <li><b>Cablaggio</b> : Due cavi : CAN_H e CAN_L per comunicazione differenziale  </li>
  <li><b>Standard ISO 11898</b> </li>
 </ul>
 <table border = "1" >
  <tr>
   <th>Pro</th>
   <th>Contro</th>
  </tr>
  <tr>
   <td>Affidabilità: Eccellente rilevamento e correzione degli errori.</td>
   <td>Velocità limitata: Non adatto per applicazioni con richieste di larghezza di banda molto elevate.</td>
  </tr>
  <tr>
   <td>Robustezza: Resiste al rumore elettrico grazie alla comunicazione differenziale.</td>
   <td>Lunghezza del bus: Raggio limitato a velocità elevate (poche decine di metri a 1 Mbps).</td>
  </tr>
  <tr>
   <td>Efficienza: Prioritizzazione dei messaggi; i più importanti hanno accesso immediato al bus.</td>
   <td>Sicurezza: Mancanza di crittografia integrata; vulnerabile a intercettazioni o attacchi.</td>
  </tr>
   <tr>
    <td>Costo: Economico per implementazioni su larga scala.</td>
    <td>Diagnosi complesse: Risoluzione dei problemi su reti CAN può essere difficile senza strumenti avanzati.</td>
   </tr>
   <tr>
    <td>Flessibilità: Supporta un'ampia varietà di dispositivi sulla stessa rete.</td>
    <td></td>
   </tr>
 </table>
        
      
       
     
 
 
