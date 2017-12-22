# Creating the GameObject

## Open tht Scene

First of all, let's open the scene we worked on last lesson (or we downloaded).

![The Starting Scene](../../images/lesson02/pic01_starting_scene.png "The Starting Scene")

## Creating the Coin

Let's create and empty gameobject (_GameObject > CreateEmpty_), posizioniamolo in _(0, 0, 0)_ and rename it _PickUpCoin_.

![The Empty GameObject](../../images/lesson02/pic02_empty_gameobject.png "The Empty GameObject")

From the _Standard Assets > Prototyping > Models_ folder, drag _PickupPrototype01x01x01_ inside _PickUpCoin_, so that it's a child element.

![Adding the Mesh](../../images/lesson02/pic03_add_coin_mesh.png "Adding the Mesh")

> We are not adding the coin prefab because we are only interested in the model. We will add the _Collider_ later on.

Select _PickupPrototype01x01x01_, and rename it _Coin_, position it in _(0, 1, 0)_ and scale it to 30% _(0.3, 0.3, 0.3)_.

With _Coin_ selected, click _Add Component_ in the _Inspector_ panel and select  _Scripts > UnityStandardAssets.Utility > AutoMoveAndRotate_ to add a rotation effect to the coin.

Open the _Rotate Degrees Per Second_ field and change _Y_ to 100.

As a last step, change the _Mesh Renderer_ from _Pink Smooth_ to _Yellow Smooth_.

The final result should be similar to the one shown in the image below.

![Improving the Coin](../../images/lesson02/pic04_improve_coin.png "Improving the Coin")

Playing the scene should start the coin rotation.

> Save the scene.

## Aggiungere il Trigger

Selezioniamo ora il _parent_ del coin, e cioè _PickUpCoin_: andremo ad aggiungere un _Collider_ in modo da poter attivare un trigger nel momento in cui il nostro personaggio entrerà a contatto con esso.

Clicchiamo su _Add Component_ e selezioniamo _Physics > Sphere Collider_. Trasformiamolo in un [Trigger](https://docs.unity3d.com/Manual/CollidersOverview.html) cliccando sul checkbox _Is Trigger_ e, nel campo _Center_ modifichiamo il valore di _Y_ a 1, in modo tale che si posizioni esattamente intorno alla moneta.

> La scelta dello _Sphere Collider_ è dovuta al fatto che ben si presta alla forma che produce la moneta mentre ruota.

![Migliorare la Moneta](../../images/lesson02/pic05_add_collider.png "Migliorare la Moneta")

Siamo ora pronti ad aggiungere interattività alla nostra moneta.