# Sicurezza informatica

## Cybersecurity

### Lezione 1: introduzione alla cybersecurity

- Il concetto di **sicurezza**: valutazione del *rischio*, la *minaccia*, il *danno* e la *probabilità* che si verifichi.
- La **sicurezza informatica**: implicazioni e responsabilità a livello *personale*, *aziendale* e *nazionale*.
- **Cyberwarfare**: la guerra cibernetica e l'esempio del malware *Stuxnet*.
- La **triade C.I.A.**: *confidenzialità* e *integrità* dei dati, *disponibilità del servizio*.
- Tipologie di **attacchi informatici**: *attivi* (mascheramento, ripetizione, modifica e DOS) e *passivi* (intercettazione e analisi dei metadati).
- Tipologie di attaccanti: *script kiddies*, *white/gray/black hat*, organizzazioni e *hacktivism*, le *minacce interne* all'azienda.
- Terminologia di base: le **vulnerabilità** (*zero-day*, *exploit*, *rootkit*, *backdoor*).
- Differenza tra vulnerabilità *software*, *hardware* e dei *protocolli*.
- Tipologie di **malware**: *virus*, *trojan*, *worm*, *ransomware*, *botnet*, *spyware*, *keylogger*, *scareware*.
- Esempi di scenari di attacco estremi: *thermal attack* e *keystroke attack*.

### Lezione 2: gestione delle credenziali e sicurezza delle password

- Il **controllo degli accessi**: *autenticazione* e *autorizzazione*.
- Principali **tecniche di intrusione**: password di *default*, *social engineering*, attacchi a *dizionario*, attacchi a *forza bruta*.
- Definizione e misura dell'**entropia** di una stringa per la costruzione di una password casuale.
- Calcolo dei tempi di *brute-force* per una password casuale a seconda della lunghezza e dell'alfabeto.
- Brute-force con **ricerca euristica** quando le password non sono casuali.
- Il problema del **credential stuffing**: statistiche e problemi derivanti dal riutilizzo delle password.
- Il **phishing**, le varie tipologie e strumenti di prevenzione.
- Uso dei **password manager** per gestire in sicurezza le password.
- Definizione e uso dell'**autenticazione multifattore**.
    
## Crittografia simmetrica
    
### Lezione 3: introduzione alla crittografia

- La **steganografia**: gli esempi di Demarato di Sparta e Istieo di Mileto.
- Procedimento di **crittografia** e **decrittografia**.
- Il **cifrario di Cesare** (sostituzione dell'alfabeto) e la sua crittoanalisi.
- Crittografia **monoalfabetica** e la **crittoanalisi statistica**.
- Crittografia **polialfabetica** (sostituzione e permutazione dell'alfabeto)
- Crittoanalisi complesse: il **test di Kasiski**;
- I **principi di Kerckhoffs**;
- Le **macchine cifranti**: il caso della macchina Enigma;
- Codifiche come crittografia: i *code talkers*.

### Lezione 4: la crittografia simmetrica

- Standard crittografici informatici: crittografia a **blocchi**.
- L'**algoritmo DES**.
- *Deep Crack* e la trasformazione di DES in DES3.
- L'**algoritmo AES** e cypher function:
  - *Substitute bytes*;
  - *Shift rows*;
  - *Mix columns*;
  - *Add Round key*.
- **Key schedule** di AES.
- Crittoanalisi e prestazioni di AES.

## Crittografia asimmetrica

### Lezione 5: il problema dello scambio delle chiavi crittografiche

- Il problema della gestione delle chiavi crittografiche.
- Il metodo dei lucchetti.
- Il metodo dei colori.
- Fondamenti di **algebra** per la crittografia:
  - L'insieme numerico Z;
  - Il teorema della divisione;
  - I **numeri primi**;
  - **Fattorizzazione** dei numeri;
  - **Aritmetica modulare**;
  - Funzioni **unidirezionali**.
- Funzioni crittografiche unidrezionali: il **logaritmo discreto**.
- L'algoritmo di scambio delle chiavi **Diffie-Hellman-Merkle**.
- L'attacco **Man-In-The-Middle**.
- Verifica delle chiavi crittografiche: gli esempi di Telegram e WhatsApp.
- Crittografia **end-to-end**.

### Lezione 6: crittografia asimmetrica e RSA

- Cifrari simmetrici vs asimmetrici.
- Creazione di un **canale cifrato** con crittografia a chiave pubblica.
- Funzione di autenticazione del messaggio (**firma digitale**).
- La nascita di RSA.
- Funzione crittografica **RSA**.
- La matematica di RSA:
  - La **fattorizzazione** dei numeri primi.
  - La **funzione enumerativa** dei numeri primi.
  - Il test probabilistico di **Miller-Rabin**.
  - Il calcolo del **modulo _n_**.
  - La **funzione *φ* di Euler** e **coprimalità** dei numeri.
  - Calcolo della funzione *φ(n)*.
  - La scelta dell'esponente *e*.
  - Calcolo della chiave privata *d*.
- Crittoanalisi e RSA factoring challenge.

## Sicurezza negli ambiti specifici

### [Web - Cloud - Gaming&Mobile]: funzioni di hashing e certificati digitali

- La certificazione delle informazioni pubbliche.
- La **firma digitale**.
- Gli algoritmi di **hashing**.
- La resistenza debole e forte alle **collisioni**.
- Funzioni di hashing:
  - controllo di ridondanza longitudinale;
  - **MD5**;
  - la famiglia di algoritmi **SHA**.
- I certificati digitali **X.509**.
- Funzionamento di una **Public Key Infrastructure**.
- X.509 *certificate issuance*.
- Web security: **HTTPS** e **TLS**.
- Sicurezza della posta elettronica: **S/MIME**.

### [Backend]: network security
- I **firewall**:
  - *packet filter router*;
  - *stateful packet inspection*;
  - *application layer firewall* e *proxy server*.
- **Access Control List**:
  - *open policy* e *closed policy*;
  - esempi di ACL.
- Sicurezza delle architetture di rete:
  - *Single proxy topology*;
  - *Multiple proxy vertically/orizontally topology*.
  - **DMZ**
  - Sicurezza delle architetture *2-tier*, *3-tier*, *n-tier*.

### [Backend]: sicurezza dei database
- OWASP top ten: **code injection**.
- L'**SQL injection**.
- Form di login insicuri.
- Prevenzione da SQL injection:
  - sanificazione dell'input;
  - principio *least privilege*;
  - *data reduction*;
  - *bind variables*;
  - *dynamic SQL*;
  - *stored procedure*.
- **Virtual private database**.

### [Fintech]: TBD

## Laboratorio

### Kali Linux e l'attività di *penetration testing*
- Linux e la distribuzione Kali.
- Le fasi di *penetration testing*.
- Pentest di una rete Wi-Fi:
  - modalità monitor delle schede di rete;
  - *denial of service* con pacchetti `deauth`
  - intercettare una sessione di *handshake*;
  - l'analisi dei pacchetti con **Wireshark**;
  - brute force con `AirCrack`.
- Scansione di rete con `nmap`.
- Attaccare i database con `sqlmap`.
- *Privilege escalation* e *reverse shell*.