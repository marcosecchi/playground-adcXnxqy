# Managing the PickUp Logic

Let's now add some logic that will let our character pick up the coin. We are going to use a Fungus [Flowchart](http://files.snozbot.com/games/fungus/docs/flowcharts/index.html), that will be placed inside the _PickUpCoin_ element.

## Adding a Flowchart

Select _PickUpCoin_, click on _Add Component_ and select _Scripts > Fungus > Flowchart_: click _Open Flowchart Window_ to show the _Flowchart_.

![Adding a Flowchart to the PickUp](../../images/lesson02/pic06_add_flowchart.png "Adding a Flowchart to the PickUp")

## Adding a 'Trigger Enter' Block

Create a command block, by using the _+_ button in the _Flowchart_ window and rename it _TriggerEnter_.

We need the block to become active on the _MonoBehaviour > Trigger_ (_FireOn > Enter_) event, when an element enters in the GameObject _Trigger_.

Set the _TagFilter_ field to 1 and, inside _Element 0_ insert "Player" (mind the uppercase!), so that only the Controller (which we tagged as "Player" in the previous lesson) will activate it.

![Adding a Block](../../images/lesson02/pic07_add_block.png "Adding a Block")

## Adding Commands

We are now going to add some commands to the block.

### Add an Usfxr Audio

First of all, let's add an _Audio > Play Usfxr Sound_ command. In the _Settings String_ field, add:

```0,.5,,.0289,.4065,.4227,.3,.4748,,,,,,,,,.5,.5848,,,,,,,,1,,,,,,```

> You can create your audio effects using the Fungus integrated editor selecting, selezionando _Fungus > Utilities > Generate usfxr Sound Effects_ (for more info, please check [the project page on GitHub](https://github.com/zeh/usfxr)).

![Adding an Audio Effect](../../images/lesson02/pic08_add_audio_effect.png "Adding an Audio Effect")

### Destroying the PickUp

Just after the audio effect, add a _Scripting > Destroy_ command and drag the _PickUpCoin_ gameobject from the _Hierarchy_ panel into the _Target Game Object_ field.

![Destroying the PickUp](../../images/lesson02/pic09_add_destroy.png "Destroying the PickUp")

Playing the scene and moving the character on the coin, will result in the object being removed from game, just after the audio effect.

You are now ready to create a prefab out of the coin object.
