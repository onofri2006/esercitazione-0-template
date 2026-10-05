# Osservazioni — Esercitazione 0

Gruppo:CM-B6

Componenti (nome, cognome e username GitHub di entrambi):
Angelica Gordiani angelica-gordiani2271115
Erige Onofri onofri2006

URL del repository condiviso:

Chi ha usato la tastiera nello step 1 e nello step 2: entrambe, in maniera alternata

Compilate insieme le osservazioni e discutete le risposte: entrambi dovete
saper spiegare le prove svolte.

## Step 1 — Hello World: compilazione ed esecuzione

Comando di compilazione:gcc -std=c17 -Wall -Wextra -Wpedantic hello.c -o hello

Comando di esecuzione e risultato osservato:./hello
Hello, computational physics!

Che cosa ho capito su sorgente ed eseguibile:sorgente hello.c(linguaggio programmatore) e eseguibile hello(linguaggio computer)

Output richiesto e comportamento del programma prima della modifica: l'output richiesto era far scrivere sul terminale una frase, la quale non veniva stampata inizialmente sul esso

Esito dopo la modifica e spiegazione della correzione:a seguito della modifica (aggiunta di printf) il programma stampava quanto richiesto

**domande stimoloe risposte::
Che differenza c'è tra hello.c e hello? Se modifichi il messaggio nel sorgente e avvii subito l'eseguibile, quale versione stai usando? Risposta: per hello.c si intende il linguaggio del programmatore, mentre hello sarebbe l'eseguibile (linguaggio della macchina). Se modifichiamo il messaggio nel sorgente e avviamo l'eseguibile, il messaggio non si aggiorna automticamente e si sta usando ancora la versione precedente
Che cosa cambia quando ricompili? Si genera un nuovo file eseguibile con il codice aggiornato.
Come puoi distinguere ciò che stampa il programma da ciò che mostra il terminale? Che cosa osservi se esegui aggiungendo > output.txt?
Il testo generato dal programma è quello che appare dopo aver lanciato il comando e prima che ricompaia il prompt del terminale (es. utente@pc:~$).A schermo non vedi nulla. L'output viene nascosto dal terminale e scritto direttamente all'interno del file output.txt (sovrascrivendolo se esisteva già).


## Step 1 — Git

Quali file ho incluso nel commit e perché: i file sorgente modificati (es. .c o file di testo) tramite git add, per tracciare le modifiche del laboratorio.

Come ho verificato che la versione provata sia presente su GitHub:git status

Che cosa ho osservato prima e dopo `git pull`, e perché non serve un nuovo clone: perche' e' gia' su github

## Step 2 — Eco: prima prova

Argomenti passati, comando e risultato:ciao mondo,./eco ciao mondo,Il programma ha stampato sul terminale esattamente le parole ciao mondo.

Che cosa posso concludere:A differenza del programma hello (che stampa un messaggio fisso), il programma eco è in grado di leggere dati esterni forniti dall'utente direttamente da riga di comando (gli argomenti) e di riutilizzarli istantaneamente per generare il suo output.

## Step 2 — Eco: seconda prova

Argomenti passati, comando e risultato:Ho testato il programma passando gli argomenti "ciao", "dodici" e "3.5" tramite il comando ./eco ciao dodici 3.5 > eco.txt, seguito da echo $? e cat eco.txt. Sul terminale è apparso subito un messaggio di errore, il codice di uscita restituito da echo è stato un numero diverso da zero (che segnala un'anomalia) e il file generato è risultato completamente vuoto poiché il programma si è bloccato prima di poter produrre l'output.

Che cosa ho capito su testo, conversioni e stampa:Ho compreso che il terminale legge qualsiasi input sempre come semplice testo, quindi per fare calcoli il programma deve prima convertire esplicitamente quei caratteri in numeri. Inserendo la parola testuale "dodici" al posto delle cifre "12", la conversione matematica fallisce e genera un errore. Inoltre, ho visto la netta separazione dei flussi di stampa: la redirezione ">" nasconde e salva nel file solo l'output normale (Standard Output), ma i messaggi di errore viaggiano su un canale indipendente (Standard Error) che continua a mostrarli direttamente a schermo.

## Step 2 — Risultato ed errori

Previsioni per l'esecuzione con argomenti validi e per quella con `dodici`:Prevedevo che con gli argomenti validi il programma avrebbe salvato le tre variabili correttamente formattate all'interno del file, lasciando il terminale pulito. Inserendo "dodici", mi aspettavo invece un blocco del programma a causa del fallimento della conversione matematica, lasciando il file di output vuoto e mostrando un avviso di errore sullo schermo.

Contenuto di `eco.txt`, messaggi nel terminale e codici di uscita osservati:Eseguendo il programma con gli argomenti validi, eco.txt conteneva esattamente la stringa "ciao 12 3.500000", il terminale non ha mostrato messaggi e il codice di uscita ($?) è risultato 0. Nel caso di "dodici", eco.txt è risultato vuoto, il terminale ha visualizzato il messaggio d'errore (poiché la redirezione > non intercetta lo Standard Error) e il codice di uscita osservato è stato un numero diverso da zero.

Come un controllo automatico può riconoscere un errore:Un sistema automatico o uno script può identificare un errore semplicemente leggendo il codice di uscita del programma (il valore di $?). Se il programma restituisce 0, il controllo sa che l'operazione è andata a buon fine; se restituisce qualsiasi valore diverso da 0, lo interpreta immediatamente come un'anomalia o un'esecuzione fallita, potendo così interrompere il processo o lanciare un allarme.

## Step 2 — Parametri e calcolo fisico

Quando serve ricompilare e quando basta cambiare gli argomenti:Basta cambiare gli argomenti da riga di comando quando si desidera modificare i dati di input o i parametri di un'esecuzione (come ad esempio il passo temporale o le condizioni di partenza di una simulazione fisica). È invece necessario ricompilare il programma solamente quando si modifica fisicamente il file del codice sorgente (il file .c), ad esempio per cambiare la formula matematica utilizzata, aggiungere una funzionalità o modificare la logica di calcolo.

## Step 2 — Git

Come riconosco nella cronologia i commit dei due step:Consultando la cronologia tramite il comando git log, posso distinguere chiaramente i salvataggi dei due step grazie ai messaggi di commit che ho inserito. Ogni messaggio descrive l'azione compiuta in quel momento, separando logicamente le modifiche fatte per far funzionare "hello" da quelle successive riguardanti la conversione e la stampa delle variabili in "eco".


Come ho verificato che la versione finale sia presente su GitHub:Dopo aver inviato il nuovo commit tramite il comando git push, ho utilizzato git status per assicurarmi che il mio sistema locale fosse perfettamente in pari con il server remoto (senza modifiche o commit in sospeso). Come prova definitiva, ho controllato la pagina web del repository su GitHub per accertarmi che i file modificati e l'ultimo messaggio di commit fossero effettivamente online.
