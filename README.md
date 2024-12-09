# -SPI-CanBus
<i>Appunti su approfondimento su argomenti  SPI e CAN BUS </i> <br>

<h2>SPI</h2> 
<b>Serial periphiral interface</b> = comunicazione seriale tra un microcontrollore e altri circuiti integrati o altri microcontrollori <br>
<b>bus standard di comunicazione</b> ideato da motorola <br>
Trasmissione avviene tra master e uno o più slave <br>
Il master manda segnale di clock per iniziare e poi per terminare <br>
-scambio dati tra dispositivi su stessa scheda o tra schede vicine <br>

4 segnali . variano in base a costruttore il nome specifico: 
<ul>
 <li>SCLK - SCK: Serial Clock (emesso dal master)
</li>
 <li>SDI – MISO – SOMI – DI - SO: Serial Data Input, Master Input Slave Output (ingresso per il master e uscita per lo slave)
</li>
 <li>SDO – MOSI – SIMO – DO – SI: Serial Data Output, Master Output Slave Input (uscita dal master)
</li>
 <li>
CS – SS – nCS – nSS – STE: Chip Select, Slave Select, emesso dal master per scegliere con quale dispositivo slave vuole comunicare (dalla figura, il segnale SS negato, si comprende che per comunicare con il dispositivo slave deve venire messo a livello logico basso)</li>
</ul>
Di questi il Chip Select (CS o SS) non è indispensabile in tutte le applicazioni.
