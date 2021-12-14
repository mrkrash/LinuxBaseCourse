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

<!--
The last comment block of each slide will be treated as slide notes. It will be visible and editable in Presenter Mode 
along with the slide. [Read more in the docs](https://sli.dev/guide/syntax.html#notes)
-->

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

<!--
You can have `style` tag in markdown to override the style for the current page.
Learn more: https://sli.dev/guide/syntax#embedded-styles
-->

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
      Linus Torvalds racconta nel suo libro che linux nasce per poter dare un'alternativa libera al predominio dei 
      software propretari. Adotta quindi una licenza il cui scopo principale è mantenere tale libertà. 
    </span>
  </div>

  <div class="flex justify-between pb-2 pt-5">
    <span class="text-xs opacity-60">
      La <strong>GPL</strong> sancisce che qualiasi fornitore, al momento di distribuire file binari, deve anche rendere
      il codice sorgente leggibile e disponibile sotto gli stessi termini di licenza.<br/>
      Essa garantisce agli utenti finali, come organizzazioni, imprese o semplici individui, di utilizzare, condividere 
      e persino modificare il software.
    </span>
  </div>

  <div class="flex justify-between pb-2 pt-5">
    <span class="text-xs opacity-60">
      Oggi arrivata alla terza versione, è progettata per essere applicata facilmente ai programmi di cui detengono i
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
      <li>- il <strong>Bootloader</strong> che è il software che gestisce il processo di avvio del computer;</li>
      <li>
        - il <strong>Kernel</strong> che è il cuore del sistema e si occupa di gestire le risorse presenti nel
        computer, rendendole disponibili alle applicazioni;
      </li>
      <li>
        - i <strong>Demoni</strong> che sono i vari servizi che ascoltano in backgroud e si attivano all'avvio del
        computer o in seguito a specifici eventi;
      </li>
      <li>
        - la <strong>Shell</strong>, ovvero un software che emula un terminale a caratteri che permette di
        controllare il computer;
      </li>
      <li>
        - il <strong>Server Grafico</strong> a cui è delegata la responsabilità di visualizzare le informazioni sul 
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
    Le distribuzioni aggiungono tutto il software necessario per avere un sistema operativo completo di software
    applicativi e di servizio, personalizzando le versioni degli stessi e organizzando al meglio la procedura di
    installazione.
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
      per delle pecularietà come l'ambiente di lavoro a cui sono destinate
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
    <ul>
      <li>convenzioni sui nomi di file</li>
      <li>attributi dei file</li>
      <li>controllo/i di accesso</li>
    </ul>
    Inoltre il file system sono un’importante componente operativa che funge da interfaccia tra il sistema operativo e 
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
    La directory <code>/etc</code> contiene tutti i file di configuration del sistema;
  </div>
  <div class="pb-2">
    La directory <code>/home</code> contiene tutte le "home directory" degli utenti;
  </div>
  <div class="pb-2">
    Le directory <code>/lib</code> e <code>/lib64</code> contiene le librerie di sistema, rispettivamente a 32 ed a 64bit;
  </div>
  <div class="pb-2">
    La directory <code>/mnt</code> è vuota e rimane a disposizione dell'utente per montarvi manualmente i devices
    che collega alla macchina;
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
    La directory <code>/sys</code> è un file system virtuale dove il kernel esporta le lproprie informazioni per 
    renderle disponibili ad altri programmiò
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
      dei pramm;</li>
      <li>- in <code>/usr/share</code>sono presenti i dati relativi alle varie applicazione, tra cui le pagine
      dei manuali;</li>
      <li>- in <code>/usr/sbin</code> in genere sono presenti i file binary utilizzabili solo da root;</li>
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
    La directory <code>/var</code> contiene i dati che i prgrammi cambiano durante la normale esecuzione del sistema
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
    successo se tiroana a zero, qualsiasi altro valore indica invece un codice di errore.
  </div>
  <div class="pb-2">
    <code>$$</code>, stringa che contiene il PID del processo in esecuzione.
  </div>
</div>
