# Comunicazione tra Flowcart

Due _Flowchart_ in scena vivono indipendentemente di vita propria: come è possibile quindi farli comunicare tra di loro? In particolare, a noi interessa far sapere al _MainFlowchart_ che una moneta è stata raccolta e questo evento, al momento, è conosciuto solamente dal _Flowchart_ contenuto nella moneta stessa.

# Utilizzo dei Messaggi

Il metodo più semplice per comunicare tra due _Flowchart_ è l'utilizzo del comando [Send Flowchart](http://fungusdocs.snozbot.com/flow_commands.html#SendMessage), che permette di spedire un messaggio, che può essere intercettato da un altro blocco all'interno del medesimo _Flowchart_ oppure anche esternamente.

Nel nostro caso, la moneta, una volta raccolta, spedirà il messaggio, che verrà raccolto dal _MainFlowchart_, che si occuperà di visualizzare i punti guadagnati.