# Creating the Scene

We are now going to create a simple scene prototype for the tutorial.

## Creating the Environment

First of all let's add some elements in the scene: from the _Standard Assets > Prototyping > Prefabs_ folder drag _FloorPrototype64x01x64_ in the _Hierarchy_.

![Add a Floor](../../images/lesson01/pic05_floor_creation_01.png "Add a Floor")

![Add a Floor](../../images/lesson01/pic06_floor_creation_02.png "Add a Floor")

Let's add, from the same prefab folder, some elements. You are free to add whatever you like, my scene looks like the one in the image.

![The Scene](../../images/lesson01/pic07_scene.png "The Scene")

Let's now add an empty gameobject (_GameObject > Create Empty_), and rename it (in the _Inspector_) _Environment_. We will move inside all the environment elements.

![The Scene](../../images/lesson01/pic08_scene_grouped.png "The Scene")

## Add a Character (Third Person Controller)

From the _Standard Assets > Characters > ThirdPersonCharacter > Prefabs_ folder, add a _ThirdPersonController_ _prefab_.

![The Third Person Character](../../images/lesson01/pic09_character.png "The Third Person Character")

Select _ThirdPersonController_ from the _Hierarchy_ panel, and in the _Inspector_ open the _Tag_ menu and choose _Player_.

![Add a Tag](../../images/lesson01/pic20_add_tag.png "Add a Tag")

## Change the Camera

Select the _Main Camera_ in the scene and disable (or delete) it. The _Game_ panel should now show a _No cameras rendering_ message).

![The Main Camera disabled](../../images/lesson01/pic10_disable_camera.png "The Main Camera disabled")

From the _Standard Assets > Cameras > Prefabs_ folder, drag the in the _Hierarchy_ panel the _MultipurposeCameraRig_ prefab.

![Adding the Camera](../../images/lesson01/pic11_add_camera.png "Adding the Camera")

> The _MultipurposeCameraRig_ prefab includes some additional features that will let the camera follow a target.

As a last step, select _MultipurposeCameraRig_ in the _Hierarchy_ panel and drag the _ThirdPersonController_ from the _Hierarchy_ panel (not from the _Project_!) in the _Target_ field of the _Auto Cam_ component.

![Adding the Camera](../../images/lesson01/pic12_add_target.png "Adding the Camera")

## Test the Scene

You can now test the scene by clicking the _Play_ button in the toolbar.

![Play](../../images/lesson01/pic13_play_scene.png "Play")
