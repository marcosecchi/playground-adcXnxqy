# Creazione della Scena

Andremo ora a creare un semplice prototipo di scena, che servirà come base per le lezioni successive.

## Creazione dell'Ambiente

Per prima cosa andremo ad aggiungere alcuni elementi al nostro scenario: datta cartella _Standard Assets > Prototyping > Prefabs_ trascinare il prefab _FloorPrototype64x01x64_ nella finestra _Hierarchy_, per creare un pavimento.

![Aggiunta del Pavimento](../../images/lesson01/pic05_floor_creation_01.png "Aggiunta del Pavimento")

![Aggiunta del Pavimento](../../images/lesson01/pic06_floor_creation_02.png "Aggiunta del Pavimento")

Aggiungiamo ora, sempre dalla stessa cartella dei prefab, alcuni elementi, per rendere la scena meno banale. La mia scena risulterà come di seguito, ma siete ovviamente liberi di creare l'ambiente a voi più congeniale!

![La Scena](../../images/lesson01/pic07_scene.png "La Scena")

Per comodità, creiamo un gameobject vuoto (_GameObject > Create Empty_), che rinominiamo (nell'_Inspector_) _Environment_ e dove andremo a spostare tutti gli elementi dell'ambiente.

![La Scena](../../images/lesson01/pic08_scene_grouped.png "La Scena")

## Aggiunta del Personaggio (Third Person Controller)

Dalla cartella _Standard Assets > Characters > ThirdPersonCharacter > Prefabs_ trasciniamo direttamente in scena il _prefab_ chiamato _ThirdPersonController_.

![Il Third Person Character](../../images/lesson01/pic09_character.png "Il Third Person Character")

Selezionando _ThirdPersonController_ in _Hierarchy_, aprire il menu _Tag_ e scegliere _Player_.

![Aggiungere un Tag](../../images/lesson01/pic20_add_tag.png "Aggiungere un Tag")


## Sostituzione della Camera

Selezioniamo la _Main Camera_ in scena, e disabilitiamola tramite il checkbox di fianco al nome, nell'_Inspector_ (La finestra _Game_ dovrebbe mostrare il messaggio _No cameras rendering_).

![La Main Camera disabilitata](../../images/lesson01/pic10_disable_camera.png "La Main Camera disabilitata")

Dalla cartella _Standard Assets > Cameras > Prefabs_, trasciniamo nella finestra _Hierarchy_ il prefab _MultipurposeCameraRig_.

![Aggiungere la Camera](../../images/lesson01/pic11_add_camera.png "Aggiungere la Camera")

> Il prefab MultipurposeCameraRig contiene una camera molto più flessibile di quella fissa, che seguirà il proprio target ovunque vada.

Come ultimo passo, selezionare _MultipurposeCameraRig_ nella _Hierarchy_ e trascinare il _ThirdPersonController_ dalla _Hierarchy_ (non dal pannello _Project_!) nel campo _Target_ del componente _Auto Cam_.

![Aggiungere la Camera](../../images/lesson01/pic12_add_target.png "Aggiungere la Camera")

## Provare la Scena

Sarà ora possibile provare la scena, tramite il pulsante _Play_ nella barra degli strumenti.

![Play](../../images/lesson01/pic13_play_scene.png "Play")
