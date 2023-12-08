# DC COMICS

#### CONSEGNA DELL'ESERCIZIO 

```
Create un nuovo progetto utilizzando Vite e Vue 3 e definite i componenti necessari per strutturare il layout come da screenshot allegato.
Quando la struttura a macroblocchi è pronta, popolate le voci di menu dinamicamente usando i data del componente.
Per oggi diamo priorità alla struttura: quando è tutto bello solido, passiamo al Sass!
Bonus:
Creare un componente aggiuntivo per gestire la fascia azzurra con le icone.
```

#### SVOLGIMENTO

- Cominciamo ad osservare il nostro template e a capire come potremmo dividere la struttura del sito. 
In questo caso vediamo 4 componenti principali: un header, un main ancora vuoto, una sezione blu con dei collegamenti,
un footer.

- L'header si compone a sua volta di due componenti, uno è il logo, e uno è la barra di navigazione sulla destra.
Quindi creiamo questi due componenti (nel caso del logo sarà una semplice immagine,
mentre nel caso della nav ci creiamo il nostro array), e li stilizziamo dentro il tag style usando regole scss se necessario.

- La sezione blu è anch'essa una lista. In questo caso optiamo per la costruzione di oggetti in cui abbiamo un'immagine e un testo.
Cicliamo dentro il nostro template per ottenere tutti gli elementi.

- Il footer è composto da un top footer e un bottom footer.

Il top footer ha 3 colonne con una giustificate a sinistra con una lista ciascuna,
tranne la prima che ha due liste. Come struttura dati in questo caso abbiamo un array di oggetti, ognuno dei quali contiene due chiavi: un titolo,
e un array di stringhe che rappresentano i collegamenti. Possiamo cicalre direttamente sulle colonne per ottenerne tante quante sono le liste e stamparne,
i contenuti, ma avremo difficoltà nel momento in cui vorremmo inserire due liste in una colonna. Quindi per questo esercizio ho evitato di ciclare
direttamente sulle colonne, e ho solo ciclato la lista di elementi.

Il bottom footer è composto da un componente bottone a sinistra, e una call to action per fidelizzazione social dell'utente con una lista di icone.
In questo caso come struttura dati abbiamo un array di path per immagini che andremo a ciclare nella nostra lista.

Per ottenere l'illusione di un container principale abbiamo dovuto usare un wrapper per wrappare ogni macroelemento in modo da limitarne
la grandezza massima. 