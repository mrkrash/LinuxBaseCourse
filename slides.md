---
theme: light-icons
class: 'text-center'
highlighter: shiki
lineNumbers: false
info: |
  ## Slidev Starter Template
  Presentation slides for developers.

  Learn more at [Sli.dev](https://sli.dev)
# persist drawings in exports and build
drawings:
  persist: false
titleTemplate: 'Corso Base Linux'
layout: image-header-intro
imageRight: '/static/linux.png'
---

<div class="leading-snug text-black dark:text-white text-opacity-60 dark:text-opacity-60 mt-4">
  <span class="text-9xl text-opacity-60" style="font-weight:600;" >
    LINUX
  </span> 
</div>

---
layout: image-header-intro
imageRight: '/static/linux.png'
---
  <div class="text-primary dark:text-primary ">
    <span class="text-3xl" style="font-weight: 600;">
      Cos'è Linux
    </span>
  </div>

  <div class="flex justify-between pb-2">
    <span class="text-xs opacity-60">
      Linux è un sistema operativo <strong>Unix Like</strong>, ideato da Linus Torvlads nel 1991.
    </span>
  </div>

  <div class="flex justify-between pb-2">
    <span class="text-xs opacity-60">
      Linux è una reale alternativa al mondo Microsoft e Unix, presente in milioni di dispositivi e server, utilizzato 
      da migliaia di sviluppatori in un mercato in continua espansione.
    </span>
  </div>

  <div class="flex justify-between pb-2">
    <span class="text-xs opacity-60">
      Linux è oggi utilizzato in sistemi integrati, per il controllo di dispositivi robotici e sullo shuttle: 
      praticamente gira su oggetti elettronici di tutti i tipi, dai server agli smartphone, risultando il sistema
      operativo in assoluto più utilizzato.
    </span>
  </div>

  <div class="flex justify-between pb-2">
    <span class="text-xs opacity-60">
      Con Linux viene gestita la maggior parte di Internet, le più grandi piazze finanziarie del mondo, nonchè i 
      supercomputer che permettono le scoperte scientifiche.
    </span>
  </div>

---
layout: dynamic-image
image: 'static/Linus_Torvalds.jpg'
equals: false
---

<div class="text-primary dark:text-primary ">
  <span class="text-3xl" style="font-weight: 600;">
    Accenni di Storia
  </span>
</div>

<div class="text-secondary dark:text-primary pt-2">
  <span class="text-lg" style="font-weight: 400;">
    Linus Torvalds e la nascita di Linux
  </span>
</div>

<div class="flex justify-between pb-2">
  <span class="text-xs opacity-60">
    Linus Torvalds, studente finlandese di informatica, il 25 agosto del 1991, insoddisfatto del sistema operativo 
    Minix (sistema unix-like destinato alla didattica e che mal supportava la nuova architettura i386 a 32bit), decide 
    di creare un kernel unix con lo scopo di divertirsi e studiare il funzionamento del suo computer, un 80386.
  </span>
</div>

<div class="flex justify-between pb-2">
  <span class="text-xs opacity-60">
    All'inizio, il kernel programmato da Linus, chiamato Linux, aveva la necessità di girare all'interno dello 
    userspace di Minix. Questo implicava l'adesione alla licenza del Minix stesso, ovvero il libero utilizzo
    esclusivamente a fini didattici, impedendone la libera distribuzione.
    Linus decide quindi di sostituire quella parte del sistema operativo con il software del progetto GNU. Per fare ciò,
    Torvalds, cambiò la licenza e adottò la GPL.
  </span>
</div>

<div class="flex justify-between pb-2">
  <span class="text-xs opacity-60">
    Sin dalla versione 0.01 si poteva compilare e far partire la shell GNU Bash. Linus rende pubblico il suo lavoro ed
    il suo codice, trovando presto altri sviluppatori che aderiscono alla visione ed al progetto, rendendo in breve
    tempo linux un sistema operativo completo, pienamente funzionante e libero. Il 12 marzo del 1994, Linus Torvalds
    presenta all'Università di Helsinki la prima versione stabile di Linux, la 1.0.
  </span>
</div>

---
layout: image-header-intro
imageRight: '/static/gnu.png'
---
  <div class="text-primary dark:text-primary ">
    <span class="text-3xl" style="font-weight: 600;">
      Gnu Public License
    </span>
  </div>

  <div class="flex justify-between pb-2 pt-5">
    <span class="text-xs opacity-60">
      Linus Torvalds racconta nel suo libro, che linux nasce per poter dare un'alternativa libera al predominio dei 
      software propretari. Adotta quindi una licenza il cui scopo principale è mantenere tale libertà. 
    </span>
  </div>

  <div class="flex justify-between pb-2">
    <span class="text-xs opacity-60">
      La <strong>GPL</strong> sancisce che qualiasi fornitore, al momento di distribuire file binari, deve anche rendere
      il codice sorgente leggibile e disponibile sotto gli stessi termini di licenza.<br/>
      Essa garantisce agli utenti finali, come organizzazioni, imprese o semplici individui, di utilizzare, condividere 
      e persino modificare il software.
    </span>
  </div>

  <div class="flex justify-between pb-2">
    <span class="text-xs opacity-60">
      Oggi arrivata alla terza versione, è progettata per essere applicata facilmente ai programmi di cui si detengono i
      relativi diritti.
    </span>
  </div>

---
layout: center-image
equals: false
---

<div class="text-primary dark:text-primary pb-4">
  <span class="text-3xl" style="font-weight: 600;">
    Ma cos'è nella pratica
  </span>
</div>

<div class="text-left ml-20 mr-20 pb-2 opacity-60">
  <div class="pb-4">
      Possiamo definirlo, impropriamente, un sistema operativo che, come i suoi principali competitor, Windows e Mac OSX,
      permette al software applicativo di dialogare con l'hardware e gestirne le risorse.<br/>
      Senza il sistema operativo, il software non potrebbe funzionare.
  </div>

  <div class="pb-2">
      Il Sistema Operativo è composto da un certo numero di sottosistemi:
    <ul class="ml-3 pt-2">
      <li>- il <strong>Bootloader</strong>, che è il software che gestisce il processo di avvio del computer;</li>
      <li>
        - il <strong>Kernel</strong>, che è il cuore del sistema e si occupa di gestire le risorse presenti nel
        computer, rendendole disponibili alle applicazioni;
      </li>
      <li>
        - i <strong>Demoni</strong>, che sono i vari servizi che ascoltano in backgroud e si attivano all'avvio del
        computer o in seguito a specifici eventi;
      </li>
      <li>
        - la <strong>Shell</strong>, ovvero un software che emula un terminale a caratteri che permette di
        controllare il computer;
      </li>
      <li>
        - il <strong>Server Grafico</strong>, a cui è delegata la responsabilità di visualizzare le informazioni sul 
        monitor;
      </li>
      <li>
        - l'<strong>Ambiente Desktop</strong>, ovvero il sottosistema con cui l'utente interagisce con il sistema 
        operativo.
      </li>
    </ul>
  </div>
</div>

---
layout: center-image
equals: false
---

<div class="text-primary dark:text-primary pb-4">
  <span class="text-3xl" style="font-weight: 600;">
    Le Distribuzioni
  </span>
</div>

<div class="text-left ml-20 mr-20 pb-2 opacity-60">
  <div class="pb-4">
      Una distribuzione è un confezionamento di vari pacchetti software coerenti fra loro, atto a rendere comoda e
      semplice, tramite procedure guidate, l'installazione di linux.
  </div>

  <div class="pb-2">
    Tenendo a mente che:
    <ul class="ml-3 pt-2">
      <li>- linux è solo un kernel, non un vero e proprio sistema operativo;</li>
      <li>
        - le applicazioni eseguite all'interno della user-space hanno una propria versione e sono indipendenti da linux
        stesso;
      </li>
    </ul>
  </div>
  <div>
    possiamo sicuramente affermare che le distribuzioni aggiungono tutto il software necessario per avere un sistema 
    operativo completo di software applicativi e di servizio, personalizzando le versioni degli stessi e organizzando al
    meglio la procedura di installazione.
  </div>
</div>

---
layout: center-image
equals: false
---

<div class="text-primary dark:text-primary pb-4">
  <span class="text-3xl" style="font-weight: 600;">
    Quale distribuzione utilizzeremo
  </span>
</div>

<div class="text-left ml-20 mr-20 pb-2 opacity-60">
  <div class="pb-4">
      Le distribuzioni oggi disponibili sono diverse decine, tutte valide a modo loro e che si differenziano tra esse
      per delle pecularietà come l'ambiente di lavoro a cui sono destinate.
  </div>

  <div class="pb-2">
    In questo corso utilizzeremo <strong>Ubuntu 20.04 LTS</strong>, una delle distribuzioni più semplici da usare che, grazie
    proprio alla semplicità di utilizzo, risulta essere la più diffusa.
  </div>
  <div class="pb-2">
    Ubuntu nasce il 20 ottobre 2002 con l'obiettivo principale di portare linux alle masse. È una distribuzione
    fortemente pensata per essere efficiente ma allo stesso tempo semplice da utilizzare.
  </div>
  <div>
    Di proprietà di Canonical, Ubuntu si presta ad essere usata sia su workstation, che su server e infrastrutture 
    cloud.<br>
    Proprio da questi ultimi due settori, Canonical trae i propri profitti.
  </div>
</div>

---
layout: image-header-intro
imageRight: 'static/Installazione01.png'
---

<div class="text-primary dark:text-primary pb-4">
  <span class="text-3xl" style="font-weight: 600;">
    Installazione
  </span>
</div>

<div class="text-left text-sm pb-2 opacity-60 mr-6">
  <div class="pb-4">
      L'installazione avverrà tramite una procedura guidata, durante la quale ci verranno poste alcune domande.
  </div>

  <div class="pb-2">
    <span class="font-bold text-lg text-yellow-500">Attenzione</span> La procedura di installazione apporterà modifiche
    alla memoria del computer, riducendo lo spazio disponibile del sistema operativo già presente, se si intende
    mantenerlo, piuttosto che eliminando tutti i dati presenti in esso se si intende sosituirlo.<br>
    È quindi necessario prestare la dovuta attenzione prima di procedere e assicurarsi di avere una copia di backup dei
    propri dati.
  </div>
</div>

---
layout: center-image
---

<div class="text-primary dark:text-primary pb-4">
  <span class="text-3xl" style="font-weight: 600;">
    Installazione
  </span>
</div>

<div class="flex text-xs">
  <div class="mr-2" style="width: 14rem;">
    <img src="static/Installazione02.png" />
    <div class="opacity-60 mt-4">
      Decidiamo se procedere con un'installazione minimale o completa e, soprattutto, se scaricare gli aggiornamenti
      durante l'installazione ed installare driver e software di terze parti.
    </div>
  </div>
  <div class="mr-2" style="width: 14rem;">
    <img src="static/Installazione03.png" />
    <div class="opacity-60 mt-4">
      Decidiamo se cancellare il contenuto del disco o ricavare un po di spazio da quello libero.
    </div>
  </div>
  <div class="mr-2" style="width: 14rem;">
    <img src="static/Installazione04.png" />
    <div class="opacity-60 mt-4">
      Inseriamo il nome utente che desideriamo utilizzare, il nome con cui il computer sarà riconosciuto all'interno 
      della rete e la password
    </div>
  </div>
</div>

---
layout: image-header-intro
imageRight: 'static/Desktop.jpg'
---

<div class="text-primary dark:text-primary pb-4">
  <span class="text-3xl" style="font-weight: 600;">
    Primo Avvio
  </span>
</div>

<div class="text-left text-sm pb-2 opacity-60 mr-6">
  <div class="pb-4">
    Terminata l'installazione, ci troveremo dinanzi una schermata di accesso con evidenziato il nome utente che 
    abbiamo scelto nella fase precedente.<br>
    Cliccandoci sopra, ci verrà richiesta la password (anch'essa scelta nella fase precedente) e ci troveremo
    nell'ambiente desktop predefinito di Ubuntu
  </div>

</div>

---
layout: center-image
equals: false
---

<div class="text-primary dark:text-primary pb-4">
  <span class="text-3xl" style="font-weight: 600;">
    Il File System
  </span>
</div>

<div class="text-left ml-20 mr-20 pb-2 opacity-60">
  <div class="pb-4">
    Il file system è un sistema di archiviazione su un supporto di memoria che struttura e organizza in modo specifico 
    scrittura, ricerca, lettura, memorizzazione, modifica ed eliminazione dei file. La strutturazione dei file deve 
    garantire una loro identificazione rapida senza errori e un accesso il più veloce possibile da parte degli utenti. 
    Inoltre, il file system definisce, ad esempio, le seguenti proprietà:
    <ul class="ml-3">
      <li>- convenzioni sui nomi di file</li>
      <li>- attributi dei file</li>
      <li>- controllo/i di accesso</li>
    </ul>
    Inoltre il file system è un’importante componente operativa che funge da interfaccia tra il sistema operativo e 
    tutte le unità collegate interne ed esterne, ad esempio tramite una porta USB.
  </div>

</div>

---
layout: center-image
equals: false
---

<div class="text-primary dark:text-primary pb-4">
  <span class="text-3xl" style="font-weight: 600;">
    Il File System su Linux
  </span>
</div>

<div class="text-left ml-20 mr-20 pb-2 opacity-60">
  <div class="pb-4 container">
    <div class="grid grid-cols-2">
      <div class="pr-2">
        <div>
          L'organizzazione del file system di Linux è gerarchica: tutto inizia da una singola directory, non esiste 
          distinzione tra hardware e software (le periferiche hardware in Linux vengono rappresentate come dei file 
          speciali) e qualsiasi parte del sistema è figlia della directory radice.<br/>
          In parole povere, tutto inizia dalla directory root e tutto termina con essa.
        </div>
        <div class="mt-2">
          La directory <code>/</code> è accessibile digitando <code>cd /</code> da terminale, oppure scrivendo 
          <code>/</code> nella barra degli
          indirizzi del file manaager.
        </div>
      </div>
      <div class="pl-20">
        / (directory root)<br/>
        |_ /boot<br/>
        |_ /dev<br/>
        |_ /etc<br/>
        |_ /home<br/>
        |_ /lib<br/>
        |_ /llib64<br/>
        |_ /mnt<br/>
        |_ /opt<br/>
        |_ /proc<br/>
        |_ /root<br/>
        |_ /run<br/>
        |_ /sys<br/>
        |_ /tmp<br/>
        |_ /usr<br/>
        |_ /var<br/>
      </div>
    </div>
  </div>
  
</div>

---
layout: center-image
equals: false
---

<div class="text-primary dark:text-primary pb-4">
  <span class="text-3xl" style="font-weight: 600;">
    Il File System su Linux
  </span>
</div>

<div class="text-left ml-20 mr-20 pb-2 opacity-60">
  <div class="pb-2">
    La directory <code>/boot</code> contiene tutti i file relativi all'avvio del sistema.
  </div>
  <div class="pb-2">
    La directory <code>/dev</code> contiene dei file di tipo particolare che rappresentano i <code>devices</code>
    presenti e riconosciuti nella macchina;
  </div>
  <div class="pb-2">
    La directory <code>/etc</code> contiene tutti i file di configurazione del sistema;
  </div>
  <div class="pb-2">
    La directory <code>/home</code> contiene tutte le "home directory" degli utenti;
  </div>
  <div class="pb-2">
    Le directory <code>/lib</code> e <code>/lib64</code> contengono le librerie di sistema, rispettivamente a 32 ed a 
    64bit;
  </div>
  <div class="pb-2">
    La directory <code>/mnt</code> è vuota e rimane a disposizione dell'utente per montarvi manualmente i devices
    che vengono collegati alla macchina;
  </div>
  <div class="pb-2">
    La directory <code>/opt</code> contiene tutte le applicazioni installate dall'utente che risultano essere
    opzionali, non facenti parte del sistema e spesso non gestiti dal package manager utilizzato dal sistema;
  </div>
</div>

---
layout: center-image
equals: false
---

<div class="text-primary dark:text-primary pb-4">
  <span class="text-3xl" style="font-weight: 600;">
    Il File System su Linux
  </span>
</div>

<div class="text-left ml-20 mr-20 pb-2 opacity-60">
  <div class="pb-2">
    La directory <code>/proc</code> è una directory particolare: ogni processo in esecuzione in Linux, occupa delle
    risorse di sistema. Per gestire tali processi, il sistema utilizza una sorta di file system che non prende
    spazio sulla memoria di massa ma è totalmente caricato in RAM. Questo file system prende posto all'interno
    della directory <code>/proc</code>.<br/>Navigando all'interno della cartella, si scopriranno tante directory
    quanti sono i processi in esecuzione sul sistema (alcuni nomi corrisponderanno ai nomi dei processi, altri al
    pid assegnato per l'esecuzione);
  </div>
  <div class="pb-2">
    La directory <code>/root</code> è la home directory dell'utente root;
  </div>
  <div class="pb-2">
    La directory <code>/run</code> è utilizzata dalle applicazione per salvare tutto ciò che gli occorre per poter
    operare, come le informazioni sui socket, i file di lock e altre informazioni utili solamente a runtime;
  </div>
  <div class="pb-2">
    La directory <code>/sys</code> è un file system virtuale dove il kernel esporta le proprie informazioni per 
    renderle disponibili ad altri programmi;
  </div>
  <div class="pb-2">
    La directory <code>/tmp</code> è dove tutti i programmi possono scrivere i file temporanei;
  </div>
</div>

---
layout: center-image
equals: false
---

<div class="text-primary dark:text-primary pb-4">
  <span class="text-3xl" style="font-weight: 600;">
    Il File System su Linux
  </span>
</div>

<div class="text-left ml-20 mr-20 pb-2 opacity-60">
  <div class="pb-2">
    La directory <code>/usr</code> contiene file relativi alle applicazioni e al kernel
    <ul>
      <li>- in <code>/usr/bin</code> in genere sono presenti i file binari utilizzabili dai normali utenti;</li>
      <li>- in <code>/usr/lib</code> sono presenti le librerie per il funzionamento dei programmi installati;</li>
      <li>- in <code>/usr/include</code> sono presenti gli header delle librerie, utili per la compilazione
      dei programmi;</li>
      <li>- in <code>/usr/share</code>sono presenti i dati relativi alle varie applicazione, tra cui le pagine
      dei manuali;</li>
      <li>- in <code>/usr/sbin</code> in genere sono presenti i file binari utilizzabili solo da root;</li>
      <li>- in <code>/usr/local</code> spesso troviamo una struttura del tutto simile a <code>/usr</code>, al cui
      interno trovano posto le applicazioni compilate manualmente dall'utente finale.</li>
    </ul>
  </div>
  <div class="pb-2">
    Tutti gli eseguibili presenti in <code>/usr/bin</code>, <code>/usr/local/bin</code> o <code>/usr/sbin</code>,
    sono eseguibili da terminale senza specificarne il percorso.<br/>
    La directory <code>/usr</code>, e tutte le sue sottodirectory, sono accessibili da tutti, ma modificabili soltanto
    dall'utente root.
  </div>
  <div class="pb-2">
    La directory <code>/var</code> contiene i dati che i programmi cambiano durante la normale esecuzione del sistema.
  </div>
</div>

---
layout: center-image
equals: false
---

<div class="text-primary dark:text-primary pb-4">
  <span class="text-3xl" style="font-weight: 600;">
    Il File System su Linux
  </span>
</div>

<div class="text-left ml-20 mr-20 pb-2 opacity-60">
  <div class="pb-3">
    Tramite il comando <strong>stat /</strong>, otteniamo:
  </div>
  <div class="pb-3">
    <code>
      File: /<br/>
      Dim.: 4096        Blocchi: 8          Blocco di IO: 4096   directory<br/>
      Device: fc05h/64517d  Inode: 2           Coll.: 20<br/>
      Accesso: (0755/drwxr-xr-x)  Uid: (    0/    root)   Gid: (    0/    root)<br/>
    </code>
  </div>
  <div>
    Le prime due righe indicano che la directory si chiama /, è grande 4096 bytes (come ogni directory) e
    occupa 8 blocchi.<br/>
    Nella terza troviamo il device in cui risiede e il numero di ulteriori directory che contiene.<br/>
    Nell'ultima riga sono presenti i permessi, l'utente e il gruppo a cui appartiene.
  </div>
</div>

---
layout: center-image
equals: false
---

<div class="text-primary dark:text-primary pb-4">
  <span class="text-3xl" style="font-weight: 600;">
    Il File System su Linux
  </span>
</div>

<div class="text-left ml-20 mr-20 pb-2 opacity-60">
  <div class="pb-2">
    I permessi associati alla root sono <strong>drwxr-xr-x</strong>, dove:
    <ul>
      <li>- la <strong>d</strong> sta per directory;</li>
      <li>- il primo gruppo di tre caratteri <strong>rwx</strong> indica i permessi di cui gode il proprietario;</li>
      <li>- il secondo gruppo, <strong>r-x</strong>, indica i permessi di cui gode il gruppo;</li>
      <li>- l'ultimo gruppo, <strong>r-x</strong>, i permessi di cui gode qualunque altro utente.</li>
    </ul>
  </div>
  <div class="pb-2">
    I permessi <strong>r</strong>, <strong>w</strong> e <strong>x</strong>, indicano rispettivamente:<br/>
    <ul>
      <li><strong>r</strong> - diritto di lettura</li>
      <li><strong>w</strong> - diritto di scrittura</li>
      <li><strong>x</strong> - diritto di esecuzione</li>
    </ul>
  </div>
  <div class="pb-2">
    Il proprietario di <code>/</code> è l'utente con identificativo 0, quindi root, e il gruppo proprietario è il 
    gruppo 0, ovvero il gruppo root.
  </div>
</div>

---
layout: center-image
equals: false
---

<div class="text-primary dark:text-primary pb-4">
  <span class="text-3xl" style="font-weight: 600;">
    File System - Links
  </span>
</div>

<div class="text-left ml-20 mr-20 pb-2 opacity-60">
  <div class="pb-2">
    Le informazioni riguardanti un oggetto (file o directory) di un filesystem, sono contenute in un inode, che viene
    identificato da un numero progressivo e descrive le caratteristiche base di un oggetto: permessi, data di modifica,
    tipo, posizione, ecc.
  </div>
  <div class="pb-2">
    Il comando <code>ln <i>sorgente</i> <i>destinazione</i></code> crea un link (alias) di un file o di una directory
  </div>
  <div class="pb-2">
    Quando si opera sul link è come se si operasse direttametne sul file, tranne quando si rimuove il link, ovvero non
    si elimina il file.
  </div>
  <div class="pb-2">
    I link possono essere di due tipi: <strong>hard</strong> e <strong>soft</strong>:
    <ul class="ml-3">
      <li>- gli hard link sono di fatto un altro nome per un file esistente; originale e link sono indistinguibili, 
      condividono lo stesso inode e non possono risiedere su due file system diversi o far riferimento a directory;</li>
      <li>- i soft link, creabili con l'opzione <code>-s</code>, sono un tipo speciale di file che fanno riferimento a
      un inode diverso, può essere fatto su file system diversi e su file che non esistono;</li>
    </ul>
  </div>
  <div class="pb-2">
    L'uso di link è completamente transparente e non impatta sulle performance del sistema.
  </div>
</div>

---
layout: center-image
equals: false
---

<div class="text-primary dark:text-primary pb-4">
  <span class="text-3xl" style="font-weight: 600;">
    File System - Gestione
  </span>
</div>

<div class="text-left ml-20 mr-20 pb-2 opacity-60">
  <div class="pb-2">
    Prima di poter utilizzare un filesystem (ad es. CDROM, USB, condivisione di rete windows, directory nfs), questo 
    deve essere formattato e montato in una sotto-directory della root ( / ).
  </div>
  <div class="pb-2">
    Una volta montato, il file system risulta accessibile a programmi ed utenti in maniera totalmente trasparente,
    diventando parte integrante dell'albero delle directory sotto /.
  </div>
  <div class="pb-2">
    Dopo l'uso, il file system può essere smontato, operazione necessaria per le unità di memorizzazione removibili.
  </div>
  <div class="pb-2">
    La directory in cui viene montato un file system può anche non essere vuota ma, il suo contenuto non potrà essere
    visibile sino a quando non si smonta il file system
  </div>
</div>

---
layout: center-image
equals: false
---

<div class="text-primary dark:text-primary pb-4">
  <span class="text-3xl" style="font-weight: 600;">
    File System - Gestione - Comandi
  </span>
</div>

<div class="text-left ml-20 mr-20 pb-2 opacity-60">
  <div class="pb-2">
    <code>mount -t [tipo fs] [opzioni] <i>device</i> <i>destinazione</i></code> Monta un dispositivo a blocchi nella 
    directory di destinazione
  </div>
  <div class="pb-2">
    <code>umount [opzioni] <i>device</i></code> Smonta un dispositivo
  </div>
  <div class="pb-2">
    <code>df [opzioni] <i>file</i></code> Verifica lo spazio libero su disco
  </div>
  <div class="pb-2">
    <code>du [opzioni] <i>file</i></code> Verifica lo spazio occupato da file e directory
  </div>
  <div class="pb-2">
    <code>fsck [opzioni] <i>device</i></code> Verifica l'integrità e ripara il file system
  </div>
  <div class="pb-2">
    <code>mkfs [opzioni] <i>device</i></code> Crea un file system, ovvero lo formatta
  </div>
  <div class="pb-2">
    Nel file <code>/ect/fstab</code> vengono configurate le informazioni sui vari file system preimpostati sul sistema,
    impostandone i punti di mount, il tipo e altri utili parametri
  </div>
</div>

---
layout: center-image
equals: false
---

<div class="text-primary dark:text-primary pb-4">
  <span class="text-3xl" style="font-weight: 600;">
    File System - Gestione - Comandi
  </span>
</div>

<div class="text-left ml-20 mr-20 pb-2 opacity-60">
  <div class="pb-2">
    <code>chown [opzioni] [utente] <i>file</i></code> Assegna un nuovo utente proprietario, sia spefificandone il nome
    piuttosto che l'UID
  </div>
  <div class="pb-2">
    <code>chgrp [opzioni] [gruppo] <i>file</i></code> Assegna un nuovo gruppo proprietario, similmente a quanto avviene
    per il comando precedente
  </div>
  <div class="pb-2">
    <code>chmod [opzioni] [modo] <i>file</i></code> Modifica i permessi sul file, sia usando l'octal mode, dove si usano
    tre numeri, riferiti rispettivamente a owner, group e others, sia utilizzando il symbolic mode, dove si usano le 
    lettere r (read), w (write), x (execute) per assegnare i permessi a u (user), g (group) e o (others).<br/>
    I seguenti comandi sono equivalenti:<br/>
    <code><br/>
      chmod 755 nomefile<br/>
      chmod u=rwx,go=rx nomefile
    </code>
  </div>
</div>

---
layout: center-image
equals: false
---

<div class="text-primary dark:text-primary pb-4">
  <span class="text-3xl" style="font-weight: 600;">
    File System - Copia/Modifica file e directory
  </span>
</div>

<div class="text-left ml-20 mr-20 pb-2 opacity-60">
  <div class="pb-2">
    <code>cp [opzioni] <i>sorgente</i> <i>destinazione</i></code> Copia di file o directory
  </div>
  <div class="pb-2">
    <code>mv [opzioni] <i>sorgente</i> <i>destinazione</i></code> Spostamento di file o directory
  </div>
  <div class="pb-2">
    <code>rm [opzioni] <i>file</i></code> Rimozione di file o directory
  </div>
  <div class="pb-2">
    <code>ls [opzioni] <i>path</i></code> Elenca contenuto di una directory
  </div>
  <div class="pb-2">
    <code>tree [opzioni] <i>path</i></code> Elenca contenuto di una directory con visualizzazione ad albero
  </div>
  <div class="pb-2">
    <code>cd <i>path</i></code> Cambia directory corrente
  </div>
  <div class="pb-2">
    <code>mkdir [opzioni] <i>directory</i></code> Crea una directory
  </div>
  <div class="pb-2">
    <code>rmdir [opzioni] <i>directory</i></code> Elimina una directory
  </div>
</div>

---
layout: center-image
equals: false
---

<div class="text-primary dark:text-primary pb-4">
  <span class="text-3xl" style="font-weight: 600;">
    Multiutenza e Permessi
  </span>
</div>

<div class="text-left ml-20 mr-20 pb-2 opacity-60">
  <div class="pb-2">
    Linux è un sistema operativo multiutente, dove differenti utenti possono avere accesso al sistema in modo
    contemporaneo, avendo i propri dati, i propri programmi e impostazioni.<br/>
    L'operazione di autenticazione dell'utente avviene tramite nome utente e password e il login può essere eseguito
    in ambienti diversi, grafici o testuali, da locale o da remoto<br/>
    L'utente principale del sistema è l'utente <strong>root</strong>, amministratore del sistema, con tutti i 
    poteri che comporta questo ruolo. Ha poteri assoluti sul sistema:
    <ul class="pl-5">
      <li>- Aggiungere, eliminare e modificare account</li>
      <li>- Installare e configurare servizi</li>
      <li>- Accesso completo a tutti i file presenti nel file system</li>
      <li>- Aggiungere o modificare file system</li>
      <li>- Distruggere tutto con un solo comando (il potere di root sul sistema è assolluto)</li>
    </ul>
  </div>
</div>

---
layout: center-image
equals: false
---

<div class="text-primary dark:text-primary pb-4">
  <span class="text-3xl" style="font-weight: 600;">
    Multiutenza e Permessi
  </span>
</div>

<div class="text-left ml-20 mr-20 pb-2 opacity-60">
  <div class="pb-2">
    Buona parte delle distribuzioni moderne, hanno deciso di disattivare in modo predefinito l'account di 
    amministrazione, incoraggiando l'utente ad utilizzare lo strumento <code>sudo</code> per svolgere i compiti di
    amministrazione di sistema.
  </div>
  <div class="pb-2">
    Lo strumento <code>sudo</code> permette a un utente (autorizzato) di elevare temporaneamente i propdi privilegi
    usando la propria password. Per poterlo fare, l'utente deve appartenere al gruppo admin ed essere aggiunto al
    file <code>/etc/sudoers</code>.
  </div>
  <div class="pb-2">
    Se per qualche motivo si rende necessario abilitare l'account di root, basterà assegnargli semplicemente una
    password con il comando <strong>sudo passwd</strong>
  </div>
  <div class="pb-2">
    In modo predefinito, l'utente iniziale creato durante l'installazione di Ubuntu è un membro del gruppo <code>
    admin</code> ed è stato aggiunto al file <code>/etc/sudoers</code> come utente autorizzato all'utilizzo di
    sudo.
  </div>
</div>

---
layout: center-image
equals: false
---

<div class="text-primary dark:text-primary pb-4">
  <span class="text-3xl" style="font-weight: 600;">
    Shell
  </span>
</div>

<div class="text-left ml-20 mr-20 pb-2 opacity-60">
  <div class="pb-2">
    Per shell si intende l'interfaccia testuale tramite la quale l'utente può operare sul sistema. Essa si occupa
    di gestire la comunicazione fra utente e sistema operativo, interpretando ed eseguendo i comandi dell'utente.<br/>
    Pùò avere diversi utilizzi:
    <ul class="pl-5">
      <li>- <strong>Uso interattivo</strong>, nel quale il sistema attende i comandi digitati dall'utente;</li>
      <li>
        - <strong>Configurazione della sessione</strong>, con cui vengono definiti variabili e parametri utilizzati
        in ogni interazione dell'utente con la macchina;
      </li>
      <li>
        - <strong>Programmazione</strong>, con la quale, utilizzando comandi di sistema e funzionalità della shell,
        è possibile realizzare piccoli programmi (script shell), in grado di automatizzare operazioni e reagire ad
        eventi.
      </li>
    </ul>
  </div>
</div>

---
layout: center-image
equals: false
---

<div class="text-primary dark:text-primary pb-4">
  <span class="text-3xl" style="font-weight: 600;">
    Bash
  </span>
</div>

<div class="text-left ml-20 mr-20 pb-2 opacity-60">
  <div class="pb-2">
    Bash (acronimo per Bourne Again Shell) è una shell del progetto GNU usata nei sistemi operativi Unix e
    specialmente in GNU/Linux.<br/>
    Si tratta di un interprete di comandi che permette all'utente di comunicare con il sistema operativo
    attraverso una serie di funzioni predefinite o di eseguire programmi.
  </div>
  <div class="pb-2">
    Tecnicamente bash è un clone evoluto della shell standard di Unix (/bin/sh), chiamata anche Bourne Shell dal
    nome del suo autore originario, Stephen Bourne.
  </div>
  <div class="pb-2">
    Una delle funzionalità maggiormente apprezzate di bash è quella della redirezione dell'input e dell'output, grazie
    al quale è possibile eseguire più programmi in cascata, passando come input dell'uno l'output dell'altro.
  </div>
</div>

---
layout: center-image
equals: false
---

<div class="text-primary dark:text-primary pb-4">
  <span class="text-3xl" style="font-weight: 600;">
    Bash - Programmazione
  </span>
</div>

<div class="text-left ml-20 mr-20 pb-2 opacity-60">
  <div class="pb-2">
    <strong>Variabili</strong>
  </div>
  <div class="pb-2">
    Le variabili in bash scripting non hanno bisogno di essere inizializzate, l'assegnazione avviene utilizzando la
    sintassi <code>VAR=valore</code>.
  </div>
  <div class="pb-2">
    È molto importante che il valore sia scritto subito dopo l'uguale senza alcuno spazio.<br/>
    Il riferimento a tutte le variabili si fanno anteponendo il caratter <code>$</code> al nome della variabile:
    <code>
      VAR=world
      echo hello $VAR!
    </code>
  </div>
</div>

---
layout: center-image
equals: false
---

<div class="text-primary dark:text-primary pb-4">
  <span class="text-3xl" style="font-weight: 600;">
    Bash - Programmazione
  </span>
</div>

<div class="text-left ml-20 mr-20 pb-2 opacity-60">
  <div class="pb-2">
    <strong>Variabili Speciali</strong>
  </div>
  <div class="pb-2">
    <code>$N</code> dove posto N è un numero intero, corrisponde dell'argomento N-esimo passato da terminale al
    programma ($0 è il nome del programma).
  </div>
  <div class="pb-2">
    <code>$*</code> stringa che contiene tutti gli argomenti passati da terminale al programma.
  </div>
  <div class="pb-2">
    <code>$#</code> stringa che contiene tutti il numero degli argomenti passati da terminale al programma.
  </div>
  <div class="pb-2">
    <code>$@</code> stringa che contiene tutti gli argomenti passati allo script corrente (ogni paramentro viene
    opportunamente quotato, questo permette l'utilizzo di questa vairabile nei cicli for).
  </div>
  <div class="pb-2">
    <code>$?</code> stringa che contiene il valore di uscita dell'ultimo comando o funzione. Il comando ha
    successo se ritorna zero, qualsiasi altro valore indica invece un codice di errore.
  </div>
  <div class="pb-2">
    <code>$$</code>, stringa che contiene il PID del processo in esecuzione.
  </div>
</div>

---
layout: image-header-intro
imageRight: 'static/nano.png'
---

<div class="text-primary dark:text-primary pb-4">
  <span class="text-3xl" style="font-weight: 600;">
    Bash - Script
  </span>
</div>

<div class="text-left text-sm mr-10 pb-2 opacity-60">
  <div class="pb-2">
    <strong>Creazione di un semplice file di script bash</strong>
  </div>
  <div class="pb-2">
    Per iniziare sarà necessario creare un nuovo file vuoto, in cui andremo ad inserire le istruzioni che bash dovrà
    eseguire.<br/>
    Il comando per creare un file vuoto su linux è <code>touch <i>nomefile.sh</i></code>, dove <i>nomefile</i> è il
    nome che vorremo assegnargli.<br/>
  </div>
  <div class="pb-2">
    Creato il file, utilizziamo un editor di testo sufficientemente semplice: <strong>nano</strong>
  </div>
  <div class="">
    Digitiamo quindi <code>nano nomefile.sh</code> e iniziamo a scrivere il seguente testo:<br/>
    <code><br/>
      #!/bin/bash<br/>
      touch ciao_linux.txt<br/>
      echo "Imparo linux!" > ciao_linux.txt<br/>
    </code>
  </div>
  <div class="pb-2">
    e quindi salviamo e chiudiamo il file con la sequenza di comandi CTRL+O e CTRL+X
  </div>
</div>

---
layout: image-header-intro
imageRight: 'static/nano.png'
---

<div class="text-primary dark:text-primary pb-4">
  <span class="text-3xl" style="font-weight: 600;">
    Bash - Script
  </span>
</div>

<div class="text-left text-sm mr-10 pb-2 opacity-60">
  <div class="pb-2">
    <strong>Creazione di un semplice file di script bash</strong>
  </div>
  <div class="pb-2">
    Nella prima riga indichiamo al sistema qual'è il programma con il quale vogliamo interpretare il contenuto
    dei comandi.<br/>In questo caso si tratta appunto di bash.
  </div>
  <div class="pb-2">
    Nella seconda diamo il comando per creare un file vuoto con il nome <code>ciao_linux.txt</code>
  </div>
  <div class="pb-2">
    Nella terza diamo il comando <code>echo</code>, la cui funzione è quella di ridare in output la stringa che
    riceve in input. L'output di echo lo reindirizziamo verso il file appena creato.
  </div>
</div>

---
layout: image-header-intro
imageRight: 'static/nano.png'
---

<div class="text-primary dark:text-primary pb-4">
  <span class="text-3xl" style="font-weight: 600;">
    Bash - Script
  </span>
</div>

<div class="text-left text-sm mr-10 pb-2 opacity-60">
  <div class="pb-2">
    <strong>Creazione di un semplice file di script bash</strong>
  </div>
  <div class="pb-2">
    Creato il file, non ci resta che assegnargli i diritti corretti ed eseguirlo.
  </div>
  <div class="pb-2">
    Per prima cosa impostiamo i diritti di esecuzione:<br/><code>chmod u+x nomefile.sh</code>
  </div>
  <div class="pb-2">
    E quindi lanciamo lo script digitando:<br/><code>./nomefile.sh</code>
  </div>
  <div class="pb-2">
    Eseguito il comando, sembrerà non accadere nulla. In realtà bash ha creato per noi un file denominato ciao_linux.txt
    con all'interno il testo che abbiamo dato in input ad echo.<br/>
    Ci basterà aprirlo con l'editor di testo che più ci aggrada (anche nano va benissimo), oppure utilizzare
    un altro comando standard della shell che ci permmette di stampare a video il contenuto di qualunque file:
    <br/><code>cat ciao_linux.txt</code>
  </div>
</div>

---
layout: center-image
equals: false
---

<div class="text-primary dark:text-primary pb-4">
  <span class="text-3xl" style="font-weight: 600;">
    Bash - Programmi Utili
  </span>
</div>

<div class="text-left ml-20 mr-20 pb-2 opacity-60">
  <div class="pb-2">
    <code>expr</code> l'interprete bash non è in grado di eseguire operazioni matematiche, quindi questo comando
    ci viene in aiuto
  </div>
  <div class="pb-2">
    <code>grep</code> utile per mostrare solo alcune righe ricevute in input sulla base del parametro che farà da
    filtro
  </div>
  <div class="pb-2">
    <code>cut</code> serve a spezzare una stringa in tante sotto-stringhe in base a un determinato separatore
  </div>
  <div class="pb-2">
    <code>cat</code> serve per copiare, unire e manipolare il contenuto di uno o più file
  </div>
  <div class="pb-2">
    <code>touch</code> utile per creare un file vuoto
  </div>
  <div class="pb-2">
    <code>echo</code> replica in output ciò che riceve in input
  </div>
  <div class="pb-2">
    <code>man</code> mostra il manuale del comando passato come parametro
  </div>
</div>

---
layout: center-image
equals: false
---

<div class="text-primary dark:text-primary pb-4">
  <span class="text-3xl" style="font-weight: 600;">
    Bash - Esempi di <code>expr</code>
  </span>
</div>

<div class="text-left ml-20 mr-20 pb-2 opacity-60">
  <div class="pb-2">
    <code><br/>
      $ var1='10'<br/>
      $ var2='20'
    </code>
  </div>
  <div class="pb-2">
    Mostra 0 se due numeri sono uguali con operatore '='<br/>
    <code>
      $ expr $var1 = $var2<br/>
      0
    </code>
  </div>
  <div class="pb-2">
    Mostra 1 quando arg1 è minore di arg2<br/>
    <code>
      $ expr $var1 \&lt; $var2<br/>
      1
    </code>
  </div>
  <div class="pb-2">
    Mostra 1 quando arg1 è diverso da arg2<br/>
    <code>
      $ expr $var1 \ⵑ= $var2<br/>
      1
    </code>
  </div>
</div>

---
layout: center-image
equals: false
---

<div class="text-primary dark:text-primary pb-4">
  <span class="text-3xl" style="font-weight: 600;">
    Bash - Esempi di <code>grep</code>
  </span>
</div>

<div class="text-left ml-20 mr-20 pb-2 opacity-60">
  <div class="pb-2">
    Trova tutte le linee in cui viene trovato il pattern 'volpe'<br/>
    <code>
      $ grep "volpe" pinocchio.txt
    </code>
  </div>
  <div class="pb-2">
    Cerca ricorsivamente il pattern "gatto" in tutti i file di una determinata cartella e in tutte le sottocartelle<br/>
    <code>
      $ grep -r "gatto" /home/utente/libri/
    </code>
  </div>
  <div class="pb-2">
    Il pattern da ricercare può anche essere parziale.<br/>
    <code>
      $ grep -r "g..to" /home/utente/libri/
    </code>
  </div>
</div>

---
layout: center-image
equals: false
---

<div class="text-primary dark:text-primary pb-4">
  <span class="text-3xl" style="font-weight: 600;">
    Bash - Esempi di <code>cut</code>
  </span>
</div>

<div class="text-left ml-20 mr-20 pb-2 opacity-60">
  <div class="pb-2">
    Estrae il primo ed il sesto campo dal file /etc/passwd, che utilizza il carattere <code>:</code> come separatore di
    campo<br/>
    <code>
      $ cut -f 1,6 -d : /etc/passwd
    </code>
  </div>
  <div class="pb-2">
    Estrae i primi dieci caratteri da ogni linea che giunge dallo standard input<br/>
    <code>
      $ cut -c -10 pinocchio.txt
    </code>
  </div>
  <div class="pb-2">
    Estrae i byte che vanno dal quinto al decimo, il sedicesimo e dal ventesimo in poi di ogni linea del file prova.txt
    <br/>
    <code>
      $ cut -b 5-10,16,20- prova.txt
    </code>
  </div>
</div>

---
layout: center-image
equals: false
---

<div class="text-primary dark:text-primary pb-4">
  <span class="text-3xl" style="font-weight: 600;">
    Bash - Esempi di <code>cat</code>
  </span>
</div>

<div class="text-left ml-20 mr-20 pb-2 opacity-60">
  <div class="pb-2">
    Mostra il contenuto del file<br/>
    <code>
      $ cat /etc/passwd
    </code>
  </div>
  <div class="pb-2">
    Mostra il contenuto di più file<br/>
    <code>
      $ cat prova_1.txt prova_2.txt
    </code>
  </div>
  <div class="pb-2">
    Crea un file con il comando cat
    <br/>
    <code>
      $ cat &gt; prova.txt<br/>
      digito del testo<br/>
      da inserite nel mio file<br/>
      e lo salvo<br/>
      CTRL+D
    </code>
  </div>
</div>

---
layout: center-image
equals: false
---

<div class="text-primary dark:text-primary pb-4">
  <span class="text-3xl" style="font-weight: 600;">
    Bash - Esempi di <code>cat</code>
  </span>
</div>

<div class="text-left ml-20 mr-20 pb-2 opacity-60">
  <div class="pb-2">
    Copia il contenuto di un file in un altro<br/>
    <code>
      $ cat prova_1.txt &gt; prova_2.txt
    </code>
  </div>
  <div class="pb-2">
    Accoda il contenuto di un file in un altro
    <br/>
    <code>
      $ cat prova_1.txt &gt;&gt; prova_2.txt
    </code>
  </div>
  <div class="pb-2">
    Unisce il contenuto di più file in uno
    <br/>
    <code>
      $ cat prova_1.txt prova_2.txt &gt; prova_3.txt
    </code>
  </div>
  <div class="pb-2">
    Ordina le righe dell'insieme dei file elencati copiandole nel file di uscita
    <br/>
    <code>
      $ cat prova_1.txt prova_2.txt prova_3.txt | sort > prova_sorted.txt
    </code>
  </div>
</div>

---
layout: center-image
equals: false
---

<div class="text-primary dark:text-primary pb-4">
  <span class="text-3xl" style="font-weight: 600;">
    Bash - Pipes <code> | </code>
  </span>
</div>

<div class="text-left ml-20 mr-20 pb-2 opacity-60">
  <div class="pb-2">
    Dati due comandi A e B, il pipe viene utilizzato per redirigere l'output del comando all'input del comando B<br/>
    Il pipe viene spesso utilizzato su più comandi in linea e il suo simbolo è <code>|</code>, che viene posto tra due
    comandi
  </div>
  <div class="pb-2">
    Mostra tutti i file contenuti nella directory corrente che contengono '.txt'
    <br/>
    <code>
      $ ls -l | grep .txt
    </code>
  </div>
  <div class="pb-2">
    Msotra il numero di processi il cui owner è root<br/>
    <code>
      $ ps -ef | grep root | wc -l
    </code>
  </div>
</div>

---
layout: center-image
equals: false
---

<div class="text-primary dark:text-primary pb-4">
  <span class="text-3xl" style="font-weight: 600;">
    Bash - Manipolazione delle stringhe
  </span>
</div>

<div class="text-left ml-20 mr-20 pb-2 opacity-60">
  <div class="pb-2">
    In Bash una stringa non è altro che una variabile, si indica dunque con ${nome} oppure con la forma abbreviata 
    $nome.<br/>
    Il nome dentro le graffe può essere seguito da un modificatore che manipola la variabile, ad esempio:
  </div>
  <div class="pb-2">
    <code>
      VAR="stringa-di-esempio"
      echo ${VAR#stringa-}
    </code>
    elimina "stringa-" dall'inizio della variabile
  </div>
  <div class="pb-2">
    I modificatori sono molti, questi sono i tre fondamentali:
    <ul class="ml-3">
      <li><code>#</code> sottrae dall'inizio della stringa</li>
      <li><code>%</code> sottrae dalla fine della stringa</li>
      <li><code>/</code> sostituisce una sottostringa con un'altra</li>
    </ul>
  </div>
</div>

---
layout: center-image
equals: false
---

<div class="text-primary dark:text-primary pb-4">
  <span class="text-3xl" style="font-weight: 600;">
    Cron
  </span>
</div>

<div class="text-left ml-20 mr-20 pb-2 opacity-60">
  <div class="pb-2">
    Spesso capita di dover far eseguire al sistema dei comandi ad un dato momento del giorno, della settimana o 
    dell'anno (ad es. i processi di backup automatici).<br/>
    Per fare ciò, su linux, esiste <strong>Cron</strong>, sotto-sistema a cui viene delegata la schedulazione delle
    operazione.<br/>
    Per fare questo, andremo ad utilizzare <strong>crontab</strong>.
  </div>
  <div class="pb-2">
    Crontab ci permette di schedulare delle operazioni sul nostro sistema con una certa semplicità, mettendo a
    disposizione del demone cron le informazione per eseguire le operazioni impostate.
  </div>
  <div class="pb-2">
    Ogni utente del sistema può avere la propria versione di crontab.
  </div>
</div>

---
layout: center-image
equals: false
---

<div class="text-primary dark:text-primary pb-4">
  <span class="text-3xl" style="font-weight: 600;">
    Il comando crontab
  </span>
</div>

<div class="text-left ml-20 mr-20 pb-2 opacity-60">
  <div class="pb-2">
    La sintassi del comando è <code>crontab -u username -opzione</code>, dove con <code>-u</code> specifichiamo il nome
    utente che possiede il file crontab. Se l'opzione <code>-u</code> viene omessa, il sistema presumerà che si stia
    operando sul proprio crontab personale.
  </div>
  <div class="pb-2">
    Altre opzioni sono:
    <ul class="ml-3">
      <li><code>-l</code> che ci permette di visualizzare il contenuto puntuale del crontab</li>
      <li><code>-r</code> che rimuove tutte le operazioni eventualmente impostate</li>
      <li><code>-e</code> che ci permette di editare le operazioni pianificate del nostro crontab tramite l'editor di
      testo predefinito</li>
    </ul>
  </div>
  <div class="pb-2">
    Ogni riga del file crontab definisce un lavoro da eseguire e sarà simile al seguente:<br/>
    <code>30 23 * * * tar -cvzf /backup_sicuro.tgz /home</code><br/>
    dove i primi cinque parametri definiscono rispettivamente minuto, ora, giorno del mese, mese e giorno della 
    settimana e il sesto il comando da eseguire.<br/>
    L'asterisco significa "tutti".
  </div>
</div>

---
layout: center-image
equals: false
---

<div class="text-primary dark:text-primary pb-4">
  <span class="text-3xl" style="font-weight: 600;">
    Il comando crontab
  </span>
</div>

<div class="text-left ml-20 mr-20 pb-2 opacity-60">
  <div class="pb-2">
    È possibile sostituire i primi cinque valori con delle stringhe "speciali" che assolvono al medesimo compito:
  </div>
  <ul class="ml-3">
    <li><code>@reboot</code> lancia il comando all'avvio del sistema</li>
    <li><code>@yearly</code> lancia il comando una volta all'anno</li>
    <li><code>@monthly</code> lancia il comando una volta al mese</li>
    <li><code>@weekly</code> lancia il comando una volta alla settimana</li>
    <li><code>@daily</code> lancia il comando una volta al giorno</li>
    <li><code>@hourly</code> lancia il comando una volta ogni ora</li>
  </ul>
</div>

---
layout: center-image
equals: false
---

<div class="text-primary dark:text-primary pb-4">
  <span class="text-3xl" style="font-weight: 600;">
    Networking
  </span>
</div>

<div class="text-left ml-20 mr-20 pb-2 opacity-60">
  <div class="pb-2">
    Sin dalle prime versioni, per ovvi motivi, una delle funzionalità principali di linux, è quella di poter comunicare
    con l'esterno.
  </div>
  <div class="pb-2">
    Per poterlo fare, il kernel di linux supporta svariati protocolli di comunicazione, dai più obsoleti ai più
    innovativi.<br/>
    Sicuramente il più utilizzato è il protocollo TCP/IP.
  </div>
  <div class="pb-2">
    Per protocollo TCP/IP ci si riferisce a un importante protocollo internet che è responsabile della trasmissione o
    del trasferimento di pacchetti di dati in rete e su internet.<br/>
    Tramite esso, due computer riescono a scambiarsi informazioni sia se sono collegati alla stessa rete locale
    (Ethernet o WiFi), sia che si trovano ai due capi di una connessione Internet (broadband).
  </div>
</div>

---
layout: center-image
equals: false
---

<div class="text-primary dark:text-primary pb-4">
  <span class="text-3xl" style="font-weight: 600;">
    Networking
  </span>
</div>

<div class="text-left ml-20 mr-20 pb-2 opacity-60">
  <div class="pb-2">
    Ad ogni computer collegato a una rete tramite il protocollo TCP/IP, viene assegnato un 
    <strong>indirizzo IP</strong>.<br/>
    Questo indirizzo, nella sua versione 4, la più diffusa, ha un formato composto da quattro numeri, che vanno da 0 a
    255:
    <code>192.168.1.55</code>
  </div>
  <div class="pb-2">
    Per verificare quale indirizzo è stato assegnato alla nostra macchina con linux, abbiamo a disposizione il comando
    <code>ip</code>
  </div>
</div>

---
layout: center-image
equals: false
---

<div class="text-primary dark:text-primary pb-4">
  <span class="text-3xl" style="font-weight: 600;">
    Networking
  </span>
</div>

<div class="text-left ml-20 mr-20 pb-2 opacity-60">
  <div class="pb-2">
    Digitando da terminale il comando <code>ip a</code> avremo un risulto simile al seguente
    <code><br/>
      1: lo: ❬LOOPBACK,UP,LOWER_UP❭ mtu 65536 qdisc noqueue state UNKNOWN group default qlen 1000<br/>
          link/loopback 00:00:00:00:00:00 brd 00:00:00:00:00:00<br/>
          inet 127.0.0.1/8 scope host lo<br/>
          valid_lft forever preferred_lft forever<br/>
          inet6 ::1/128 scope host <br/>
          valid_lft forever preferred_lft forever<br/>
      2: enp1s0: ❬BROADCAST,MULTICAST,UP,LOWER_UP❭ mtu 1500 qdisc fq_codel state UP group default qlen 1000<br/>
          link/ether 52:54:00:7c:00:3a brd ff:ff:ff:ff:ff:ff<br/>
          inet 192.168.1.103/24 brd 192.168.1.255 scope global dynamic noprefixroute enp1s0<br/>
          valid_lft 3445sec preferred_lft 3445sec<br/>
          inet6 fe80::813a:204:8b17:1a56/64 scope link noprefixroute <br/>
          valid_lft forever preferred_lft forever<br/>
     </code>
  </div>
</div>

---
layout: center-image
equals: false
---

<div class="text-primary dark:text-primary pb-4">
  <span class="text-3xl" style="font-weight: 600;">
    Networking
  </span>
</div>

<div class="text-left ml-20 mr-20 pb-2 opacity-60">
  <div class="pb-2">
    Tra le varie informazioni riportate dal comando ip, vi sono:
    <ul class="ml-3">
      <li>- il nome dell'interfaccia di rete, in questo caso <strong>lo</strong> e <strong>enp1s0</strong>;</li>
      <li>
        - lo stato dell'interfaccia, in questo caso <strong>UNKNOWN</strong> per lo e <strong>UP</strong> per enp1s0;
      </li>
      <li>
        - l'indirizzo di rete assegnato, <strong>127.0.0.1/8</strong> per lo e <strong>192.168.1.103/24</strong> per
        enp1s0;
      </li>
    </ul>
  </div>
</div>

---
layout: center-image
equals: false
---

<div class="text-primary dark:text-primary pb-4">
  <span class="text-3xl" style="font-weight: 600;">
    Networking - lo
  </span>
</div>

<div class="text-left ml-20 mr-20 pb-2 opacity-60">
  <div class="pb-2">
    L'interfaccia di <strong>loopback</strong> o <strong>lo</strong>, è un interfaccia virtuale e fittizia, necessaria
    al nomrale funzionamento dell'ambiente linux.<br/>Tramite questa interfaccia, i vari servizi che fanno uso del 
    protocollo TCP/IP, possono dialogare tra loro e scambiarsi informazioni in tutta sicurezza.<br/>
    L'indirizzo assegnato a questa interfaccia è standard e prefissato: <strong>127.0.0.1/8</strong><br/>
  </div>
</div>

---
layout: center-image
equals: false
---

<div class="text-primary dark:text-primary pb-4">
  <span class="text-3xl" style="font-weight: 600;">
    Networking - enp1s0, eth0, altro
  </span>
</div>

<div class="text-left ml-20 mr-20 pb-2 opacity-60">
  <div class="pb-2">
    Ogni altra interfaccia, su linux, può avere o un nome generico (come ad es. eth0, eth1, ect.) oramai in disuso, o un
    nome specifico relativo all'hardware utilizzato (come ad esempio enp1s0).<br/>
    Tramite questa o altre interfacce, il computer può comunicare correttamente con l'esterno, usufruire dei servizi
    messi a disposizione dagli altri sistemi, e metterne a sua volta a disposizione.<br/>
    Non esiste un indirizzo prefissato da assegnargli, esso dipende dalla rete a cui si è collegati e quindi dalle
    politiche messe in atto dall'amministratore di rete o, più semplicemente, dal router tramite il quale guadagniamo la
    connessione alla rete.<br/>
  </div>
</div>

---
layout: center-image
equals: false
---

<div class="text-primary dark:text-primary pb-4">
  <span class="text-3xl" style="font-weight: 600;">
    Networking - file di configurazione
  </span>
</div>

<div class="text-left ml-20 mr-20 pb-2 opacity-60">
  <div class="pb-2">
    <strong>/etc/sysconfig/network</strong><br/>
    Contiene le principali configurazioni come il nome della macchina (hostname) e il default gateway. Ad esempio:
    <code><br/>
      NETWORKING=yes ;Attiva la rete<br/>
      HOSTNAME=ubuntu-pc ;Il nome della macchina<br/>
      GATEWAY=192.168.1.1 ;L'indirizzo IP del router che ci permette la connessione a internet<br/>
    </code>
  </div>
  <div class="pb-2">
    <strong>/etc/sysconfig/network-script/*</strong><br/>
    Directory contenente i file di configuraazione delle singole interfacce
  </div>
  <div class="pb-2">
    <strong>/etc/hosts</strong><br/>
    Contiene il mapping tra indirizzi e hostname (ed alias). Ad esempio:
    <code><br/>
      127.0.0.1 localhost.localdomain localhost<br/>
      192.168.1.55 ubuntu-pc<br/>
    </code>
  </div>
</div>

---
layout: center-image
equals: false
---

<div class="text-primary dark:text-primary pb-4">
  <span class="text-3xl" style="font-weight: 600;">
    Networking - file di configurazione
  </span>
</div>

<div class="text-left ml-20 mr-20 pb-2 opacity-60">
  <div class="pb-2">
    <strong>/etc/services</strong><br/>
    Contiene il mapping tra il numero delle porte e i nomi dei servizi.<br/>
    È un file che solitamente non si modifica, a meno di creare nuovi servizi personalizzati.
  </div>
  <div class="pb-2">
    <strong>/etc/resolv.conf</strong><br/>
    File di configurazione del client DNS, ovvero contiene gli indirizzi del server DNS e un possibile dominio
    dell'host e l'ordine di ricerca. Ad esempio:
    <code><br/>
      nameserver 192.168.1.1 ;IP del DNS primario, che spesso coincide con l'indirizzo del default gateway;<br/>
      nameserver 8.8.8.8 ;IP del DNS secondario<br/>
      domain miodominio.it ;Nome del dominio dove si trova l'host<br/>
      options timeout:6 ;Imposta il timeout a 6 secondi per le query DNS
    </code>
  </div>
</div>

---
layout: image-header-intro
imageRight: '/static/linux.png'
---
<div class="text-primary dark:text-primary pb-3">
  <span class="text-3xl" style="font-weight: 600;">
    In definitiva, perchè usare linux
  </span>
</div>

<div class="flex justify-between pb-2">
  <span class="text-xs opacity-60">
    Linux è un sistema operativo libero, non ha costi di licenza e c'è una vera e propria comunità di sviluppatori che
    giornalmente si adopera per migliorarlo, aggiornarlo e diffonderlo.
  </span>
</div>

<div class="flex justify-between pb-2">
  <span class="text-xs opacity-60">
    È semplice da utilizzare, la sua interfaccia grafica è molto simile a qualunque altro sistema operativo: cartelle,
    copia e incolla, browser sono uguali ai programmi presenti negli altri sistemi operativi
  </span>
</div>

<div class="flex justify-between pb-2">
  <span class="text-xs opacity-60">
    La semplicità però non ci impedisce di addentrarci nella complessità dei sistemi server, nell'esplorare funzionalità
    che tutti i giorni siamo abituati ad utilizzare come semplici utenti.
  </span>
</div>

<div class="flex justify-between pb-2">
  <span class="text-xs opacity-60">
    Inoltre linux, ad oggi, è esente da virus informatici: è di fatto l'unico sistema operativo struttura in modo
    "sicuro" e che ci permette un'immunità dai virus molto vicina al 100%.
  </span>
</div>
