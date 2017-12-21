# Adding a Flowchart

Let's add a Fungus [Flowchart](http://files.snozbot.com/games/fungus/docs/flowcharts/index.html) which we will use in the next chapters, along with a text element (for displaying messages).

## Flowchart Creation 

From menu _Tools > Fungus > Create_ select _Flowchart_, which will add a _Flowchart_ in the scene. Select it in the _Hierarchy_ panel and click the _Open Flowchart Window_ button: the corresponding panel will pop up.

Rename the _Flowchart_ as _MainFlowchart_ in the _Inspector_ panel.

![Adding the Flowchart](../../images/lesson01/pic14_create_flowchart.png "Adding the Flowchart")

### Renaming the 'Start' Block

Inside the _Flowchart_, select _NewBlock_ and, in the _Inspector_, rename it _Start_.

![Renaming the Block](../../images/lesson01/pic15_rename_block.png "Renaming the Block")

## Creating a Text Element

From the menu _GameObject > UI_ select _Text_, and a text element will be generated in the scene. select it and give it a look you like (mine is shown below).

![Adding the Text](../../images/lesson01/pic16_add_text.png "Adding the Text")

## Show a Welcome Message

Let's add a welcome message to the text. Select the _Start_ block in the _Flowchart_ and click the _+_ button, selecting the _UI > Set Text_ command.

![Adding the SetText Command](../../images/lesson01/pic17_add_text_command.png "Adding the SetText Command")

Select the just created command and drag the _Text_ gameobject from the _Hierarchy_ panel into the _Target Text Object_ field. Lastly, add a welcome message in the _Text_ field.

![Adding the GameObject Text](../../images/lesson01/pic18_add_text_gameobject.png "Adding the GameObject Text")
