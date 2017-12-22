# Sending a Message

## Adding a SendMessage Command to the Flowchart

Select the _PickUpCoin_ prefab inside the project and open its _Flowchart_.

> Modyfing the prefab inside the _Project_ panel has the side effect of modyfing all the connected element in the scene.

Add a _Flow > Send Message_ command and move it just before _Destroy_.

> If the command is placed after _Destroy_, it won't be executed as the _Flowchart_ will be destroyed before.

From the _Message Target_ menu, select _All Flowcharts_ (so the command can be 'listened' from external _Flowchart_s) and, in the _Message_ field, insert _coin-collected_.

> Pay attention: the message text is case sensitive!

![Sending the Message](../../images/lesson03/pic01_send_message.png "Sending the Message")

All our coin object in the scene should now have the _Send Message_.