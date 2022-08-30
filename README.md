# Develhope - Esercizi SASS

## Variable Nesting

Ricreare il layout fornito utilizzando il nesting delle regole e le variabili SASS.
I colori da utilizzare sono:

- red

- blue

- green


## Mixin

Ricreare il layout fornito utilizzando un mixin tale da poter applicare lo stile necessario a tutti i tag article.
Tale mixin dovrà accettare come parametri il color, il border-color e il font-size. Il font-size dovrà anche avere un valore di default pari a 1rem.
Il font-size del footer è pari a 24px.

## Mixin Animation - 01

Vogliamo applicare una classe che permetta l'animazione dell'elemento, l'effetto dovrà fare "saltellare" l'elemento html. La classe si chiamerà .bounce ed avrà una durata di animazione di 1s.

Tramite mixin dovremmo creare una animazione di nome "bounce".

Nella mixin dovremmo parametrizzare la partenza della traslazione e la distanza con cui l'elemento dovrà traslare sull'asse Y nei vari frames.

Dunque la mixin avrà 2 valori di default nei parametri:

    partenza traslazione

    distanza traslazione

Come possiamo vedere nell'esempio che segue abbiamo intercettato che si parte da 0 e si arriva a massimo -30px (quando si trova al 40% dell'animazione) Nel momento in cui si è al 60% bisogna assegnare la metà della distanza di traslazione parametrizzata. Ad esempio se al 40% abbiamo -30px al 60% dovremmo avere -30px/2

## Function Modules

Modificare il codice dell'esercizio 2 creando un modulo per tutte le variabili dichiarate.
Creare poi un modulo con una funzione che trasformi i px in rem, quindi che accetti come parametro un numero e restituisca il valore relativo in rem.
Consideriamo che 1rem = 16px.
Tale funzione dovrà essere applicata nel foglio principale in modo che l'unica unità di misura sia il rem.

## Function Random Hex Generator

Tramite una funzione creare un generatore di colori randomici in formato esadecimale.

La funzione si chiamerà random-hex() e dovrà ritornare una stringa del tipo: "#AA11FF"

Facendo dunque affidamento alla funzione nativa random() possiamo generare dei valori randomici, dovremmo poi controllare con un if se il valore è > di 9 per apporre le lettere da A ad F

Tramite il comando @return possiamo ritornare il valore generato dalla funzione.

## Selectors Extend

Modificare il codice dell'esercizio 3 utilizzando il parent selector '&' per le classi annidate.
Stilizzare l'h2 che avrà le stesse regole di h1 con in più in padding di 1rem e un borso rosso.
Per stilizzare l'h1 e l'h2 utilizare il metodo extend.

## Extend Animation Bounce

Creare una nuova classe .bg-random che avrà un brackground generato randomicamente tramite la funzione random-hex().

Estendere la classe .bounce dell'esercizio precedente assegnandogli un colore randomico grazie alla classe .bg-random.

Assegnare la classe .bounce ad un div con forma rotonda e posizionarlo all'interno del foglio html a piacimento.

## Flow Control

Aggiungere una nuova sezione al layout come mostrato nell' immagine allegata.
I box sono quadrati di 45px (da trasformare in rem) per lato e il loro allineamento è eseguito con flex.
Il background-color, il color e il font-size dovranno essere gestiti utilizzando il flow control (@for, @if, ecc...) e i metodi darken e lighten (l'amount ha un moltiplicatore pari a 5).
In particolare bisogna creare le classi .fs-1rem, .fs-2rem e .fs-3rem utilizzando @each.
I colori aggiunti sono solo white e black.




