# Flowchart Communication

Two _Flowchart_ in a scene are independent, so how can make them communicate? In particular, we need to let the _MainFlowchart_ know that a coin has been picked up, an event that at the moment is known only by the coin _Flowchart_.

## Using Messages

The quickest way to communicate between _Flowchart_s is the [Send Flowchart](http://fungusdocs.snozbot.com/flow_commands.html#SendMessage) command, that sends a message that can be listened by the same _Flowcart_ or by another one.

In our game, when a coin will be picked up, the corresponding _Flowchart_ will send a message that will be intercepted by the _MainFlowchart_, that will store points gained.
