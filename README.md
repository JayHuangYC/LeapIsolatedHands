LeapIsolatedHands
=====================

A Unity demo demonstrating hand isolation and display from the raw video passthrough.  Push and pull floating blocks with your real hands (tinted to a flesh tone of course).  

Ideally suited as a base for further experiments.

[Leap Motion Unity Sample](https://developer.leapmotion.com/gallery/hand-background-isolation)

This is a proof of concept to show that realistic hand isolation is possible with proper occlusion and physics.

Method: The main feed is first segmented into hand and non-hand areas using a flood-fill. The non-hand areas are then made fully transparent and the foreground is tinted flesh-tone. The image plane is then moved forward and backward to match the depth of the hand for occlusion. After that a physical model of the hand is placed on top of the rendered one. The two modified files from the original demo are Assets\LeapMotion\Scripts\Utils\LeapImageRetriever.cs and Assets\LeapMotion\Shaders\LeapUndistorted.shader, the rest of it is just how the components are arranged in the scene.

Before using, enable "Allow Images" in the Leap Motion Control Panel.

    Windows Only Binaries built with Leap SDK 2.1.2 and Oculus SDK 4.2 Beta


#Youtube video

[VR mode](https://www.youtube.com/watch?v=c8uZHaoZl_w)

[AR mode](https://www.youtube.com/watch?v=o0cnBAJmaks)
