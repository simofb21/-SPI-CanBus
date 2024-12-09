# -SPI-CanBus
<i>Appunti su approfondimento su argomenti  SPI e CAN BUS </i> <br>

<h2>SPI</h2> 
<b>Serial periphiral interface</b> 
<br>
<h3>Definizione : </h3>comunicazione seriale tra un microcontrollore e  altri microcontrollori o periferiche come sensori, display ... <br>
<b>bus standard di comunicazione</b> ideato da motorola <br>
<h3>Trasmissione : </h3> Full-duplex: i dati possono essere inviati e ricevuti contemporaneamente. <br>

Il master manda segnale di clock per iniziare e poi per terminare <br>

<h3>Linee di comunicazione </h3>
<ul>
 <li><b>SCLK (Serial Clock)</b>: segnale di clock generato dal master.</li>
 <li><b>MOSI (Master Out Slave In)</b>: dati inviati dal master allo slave.</li>
 <li><b>MISO (Master In Slave Out)</b>: dati inviati dallo slave al master.</li>
 <li> <b>SS/CS (Slave Select/Chip Select)</b>: usata per selezionare lo slave attivo.
</li>
</ul>
<h3>Caratteristiche principali
</h3>
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
            <td>Alta velocità di trasferimento dati</td>
            <td>Richiede più linee di comunicazione</td>
        </tr>
        <tr>
            <td>Facile da implementare</td>
            <td>Supporta solo brevi distanze</td>
        </tr>
    </table>


