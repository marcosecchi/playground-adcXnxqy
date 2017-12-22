# Receiving a Message

Let's improve the _MainFlowchart_, so it will listen for an incoming message.

## Creating the Block

Select _MainFlowchart_ from the _Hierarchy_ panel and open the editing window. Add a new block called _On Coin Collect_ and add a _Debug Log_ command with some kind of message (for instance 'Coin collected!').

> The _Debug Log_ command will trace some information on the  [Console](https://docs.unity3d.com/Manual/Console.html), for instance errors. We are tracing some text just to be sure that the block is executed.

![Debug](../../images/lesson03/pic02_debug.png "Debug")

## Adding a MessageReceived event

With _On Coin Collect_ selected, choose from the _Execute On Event_ drop-down _Scene > Message Received_ and in the _Message_ field insert '_coin-collected_'.

![Receiving the Message](../../images/lesson03/pic03_receive_message.png "Receiving the Message")

Save the scene and click the _Play_ button: each time a coin is collected, the console should trace the corresponding message.
