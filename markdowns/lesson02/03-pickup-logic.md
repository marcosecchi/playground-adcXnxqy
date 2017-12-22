# Managing the PickUp Logic

Let's now add some logic that will let our character pick up the coin. We are going to use a Fungus [Flowchart](http://files.snozbot.com/games/fungus/docs/flowcharts/index.html), that will be placed inside the _PickUpCoin_ element.

## Adding a Flowchart

Select _PickUpCoin_, click on _Add Component_ and select _Scripts > Fungus > Flowchart_: click _Open Flowchart Window_ to show the _Flowchart_.

![Adding a Flowchart to the PickUp](../../images/lesson02/pic06_add_flowchart.png "Adding a Flowchart to the PickUp")

## Adding a 'Trigger Enter' Block

Create a command block, by using the _+_ button in the _Flowchart_ window and rename it _TriggerEnter_.

Il blocco deve attivarsi all'evento _MonoBehaviour > Trigger_ (_FireOn > Enter_), cioè quando un elemento in scena entra nel _Trigger_ del GameObject.

Imponiamo al _TagFilter_ il valore 1 e, nell'_Element 0_ inseriamo "Player" (attenzione alla maiuscola!), in modo che solamente il Controller (che abbiamo taggato nella lezione precedente come "Player").

![Aggiungere il Blocco al Flowchart](../../images/lesson02/pic07_add_block.png "Aggiungere il Blocco al Flowchart")

## Aggiungere i Comandi

Siamo ora pronti ad inserire i comandi nel nostro blocco.

### Aggiungere un Audio Usfxr

Per prima cosa aggiungiamo il comando _Audio > Play Usfxr Sound_. Nel campo _Settings String_ inseriamo il seguente valore:

```0,.5,,.0289,.4065,.4227,.3,.4748,,,,,,,,,.5,.5848,,,,,,,,1,,,,,,```

> E' possibile creare il proprio effetto sonoro tramite l'editor di effetti di Fungus, selezionando _Fungus > Utilities > Generate usfxr Sound Effects_ (per maggiori informazioni, consultare [la pagina del progetto](https://github.com/zeh/usfxr)).

![Aggiungere un Effetto Audio](../../images/lesson02/pic08_add_audio_effect.png "Aggiungere un Effetto Audio")

### Rimuovere il PickUp

Subito dopo l'effetto audio, aggiungiamo il comando _Scripting > Destroy_ e trasciniamo il gameobject _PickUpCoin_ dalla scena nel campo _Target Game Object_.

![Distruggere il PickUp](../../images/lesson02/pic09_add_destroy.png "Distruggere il PickUp")

Se lanciamo la scena e muoviamo il nostro personaggio sulla moneta, dovremmo udire il suono generato e la successiva distruzione della moneta dalla scena.

Siamo ora pronti a creare un prefab dal nostro pickup.