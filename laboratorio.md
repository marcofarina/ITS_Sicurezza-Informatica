# Preparazione al laboratorio

La lezione di laboratorio è una simulazione di un'attività di *penetration testing*. Prevede l'utilizzo di *Kali Linux* e alcuni suoi tool: `Aircrack-ng`, `Wiresahrk`, `nmap` e `sqlmap`.

La lezione può essere seguita normalmente, assistendo alla dimostrazione e prendendo appunti come sempre, oppure, preparandosi adeguatamente è possibile provare i comandi in tempo reale.

Il modo più facile per seguire attivamente la lezione è necessario avere:

- un portatile BYOD;
- una pendrive USB 3 da almeno 8GB;
- una scheda di rete wireless in grado di supportare la modalità *monitor*.

## Istruzioni

1. Scaricate Kali Linux dalla [pagina di download](https://www.kali.org/get-kali/#kali-live) del sito ufficiale. Scaricate la versione **Live Boot** nella configurazione opportuna per il vostro PC/Mac. Vi raccomando la versione *Point release* (versione stabile).
2. Al termine del download verificate che l'hash del file scaricato corrisponda all'hash pubblicato sul sito (lo trovate nella tab `sum`.
3. Se avete dei dati nella pendrive, fatene un backup, perché tutti i dati verranno cancellati. Scaricate Balena Etcher dal [sito ufficiale](https://www.balena.io/etcher/). L'applicazione è facilissima da usare: selezionate l'immagine ISO di Kali, selezionate la pendrive e attendete che la preparazione (*flash*) della pendrive termini.
4. Provate ad avviare Kali Linux:
	- su PC Windows: entrate nel BIOS/UEFI e disabilitate temporaneamente l'avvio sicuro, che blocca l'avvio di OS live. Modificate l'ordine di boot impostando come primo l'USB.
	- su macOS: riavviate il Mac tenendo premuto `alt`. Nel menu di scelta selezionate l'avvio della pendrive.
5. Una parte di questo laboratorio prevede l'uso della modalità `monitor` della scheda di rete wireless. Non tutti i chipset supportano questa modalità. Se volete verificare la compatibilità, da terminale potete digitare i comandi
```
$ sudo ifconfig wlan0 down
$ sudo iwconfig wlan0 mode monitor
$ sudo ifconfig wlan0 up
```
avendo l'accortezza di sostituire `wlan0` con il nome della vostra interfaccia di rete wireless.

Se non doveste essere in grado di attivare la modalità `monitor` potete provare un adattatore wireless USB, se ne avete uno, altrimenti semplicemente salterete questo pezzo di laboratorio e proverete solo le parti successive.

Ricordate che in ogni caso **nulla** di tutto questo è **obbligattorio**. Potete seguire la lezione come una semplice dimostrazione.