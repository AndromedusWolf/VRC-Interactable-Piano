# VRC-Interactable-Piano

## Overview
This is an interactable piano that you can you use in your VR Chat world. This is currently experimental and the physical interaction only works with some avatars. 

This is being made free to use by the community and you may alter and improve the package as you wish. All I ask is that, if you alter the package and wish to distribute it, that you do so freely. There is no need to credit me or the other people listed below, you may do so if you wish however. What I would appreciate is if you leave the UI panel on the piano that has the link to this package so that other people know where it was downloaded. 

Thank you and hope you have fun with this piano!


## Acknowledgements
The base code being used to drive the physical interaction system on the piano is by [Kovaloid on Twitter](https://twitter.com/kovaloid)

The piano model is by [Catdevpete on Sketchfab](https://sketchfab.com/3d-models/upright-piano-wip-eb76131fcae44993a532ad1b99050deb)


## Dependencies

It is VERY important that you have the following two packages downloaded already before downloading this package! The piano won't work without them!

1. You will need [Udonsharp](https://github.com/vrchat-community/UdonSharp)

2. You will need [VRC Physical Interaction](https://bitbucket.org/akovaloid/vrc-physical-interaction/src/master/)


## Preparation

Before going through the preparation process, please ensure that you have NOT imported the piano package into your Unity project yet! If you have, please delete it from your project window and only import it when told!

1. Once you have finished importing Udonsharp and Physical Interaction, head into the "Physical Interaction" folder, then the "Scripts" folder, then the "Buttons" folder and delete the files named "PIButton". This is because the piano keys will default to the PIButton code instead of the altered code I made for them. 

![unknown_2022 02 16-22 03_LI](https://user-images.githubusercontent.com/99851805/154397536-241112e7-1a3c-410e-ae1d-4a53fd9f5002.jpg)

2. Navigate back to the "Physical Interaction" folder and head into the "Prefabs" folder. Locate the "Player Height Detector" prefab and drag it into your world. The placement of it in the Hierarchy does not matter, it can be placed anywhere.

![unknown_2022 02 16-23 27_LI](https://user-images.githubusercontent.com/99851805/154405693-e788d075-ca86-4142-a27b-62982089e07e.jpg)

3. Next, click on the "Layers" tab in the upper right corner of your Unity window, go down and click "Edit Layers" .

![unknown_2022 02 16-22 28_LI](https://user-images.githubusercontent.com/99851805/154399840-7fc784e7-0052-42a3-b4fa-f7b11eb7c0cb.jpg)

4. A list of different layers will have showed up. On "User Layer 27", type in "InteractiveControls". On "User Layer 28", type in "PlayerInteractionCollider".

![unknown_2022 02 16-22 32_LI](https://user-images.githubusercontent.com/99851805/154400291-1538a4a7-98af-4953-9ed4-fe404f0a8e9d.jpg)

5. Next, you will have to navigate into the "Project Settings" window. You may have to pull it up from the "Windows" tab if you don't already have it out.

![unknown_2022 02 16-22 37](https://user-images.githubusercontent.com/99851805/154400742-dd851836-2efd-4400-8a4b-65551acaf551.png)

6. Once you are in the "Project Settings" window, look to the left side of the window and click on "Physics". You will see the "Physics" section with what looks like a right-angle triangle with a bunch of checkmarks in it. Look for the "InteractiveControls" and "PlayerInteractionCollider" sections and make it look like the image below.

![unknown_2022 02 16-22 41_LI](https://user-images.githubusercontent.com/99851805/154401268-302b1332-dd28-4c28-a3e4-77eadcf47f6e.jpg)

Once that's done, you are set! You may now import the piano package into your Unity project window! Now it's time for the Set-Up process!

## Set-Up

1. Once you have imported the package, head into the "Interactable Piano V1" folder, then the "Piano V1" folder and drag out the Piano Prefab into your world. If you don't see it, don't worry! Just look around, you'll find it floating around somewhere.

![unknown_2022 02 16-23 12_LI](https://user-images.githubusercontent.com/99851805/154404060-3f0eaee9-cf6d-42b0-98cf-47c40ed65fdf.jpg)

Once you've done that, then that's it really! Congrats! You should now (hopefully) have a working piano in your world! 

## Notes

If you wish, you may change the sounds that each piano key makes when played. To do this, first import the sound file into your project window, then click on the mesh key (You'll know when you're there when the name of the object is "PianoKey.0XX" where "XX" is the number of the key). In the inspector, scroll down to "Audio Source" and drag your sound file into the "Audio Clip" field.

![unknown_2022 02 16-23 38_LI](https://user-images.githubusercontent.com/99851805/154406633-49a8d976-d785-4a29-bcd7-b5d86d00a661.jpg)

