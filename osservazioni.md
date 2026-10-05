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

Argomenti passati, comando e risultato:

Che cosa ho capito su testo, conversioni e stampa:

## Step 2 — Risultato ed errori

Previsioni per l'esecuzione con argomenti validi e per quella con `dodici`:

Contenuto di `eco.txt`, messaggi nel terminale e codici di uscita osservati:

Come un controllo automatico può riconoscere un errore:

## Step 2 — Parametri e calcolo fisico

Quando serve ricompilare e quando basta cambiare gli argomenti:

## Step 2 — Git

Come riconosco nella cronologia i commit dei due step:

Come ho verificato che la versione finale sia presente su GitHub:
