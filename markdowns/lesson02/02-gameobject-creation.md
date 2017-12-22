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

## Add the Trigger

Select the coin _parent_ del coin (_PickUpCoin_): we are going to add a _Collider_ so we can activate a trigger when the character enters inside it.

Let's click _Add Component_ and select _Physics > Sphere Collider_: change it in a [Trigger](https://docs.unity3d.com/Manual/CollidersOverview.html) checking the _Is Trigger_ value and, in the _Center_ field, change the _Y_ value to 1, so that it will be in the same position as the coin element.

> We are using a _Sphere Collider_ as it is pretty good for the ritating coin.

![Improving the Coin](../../images/lesson02/pic05_add_collider.png "Improving the Coin")

We are now ready to add some interactivity the the coin.
