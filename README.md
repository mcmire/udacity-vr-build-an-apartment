# Build an Apartment Project

This project was developed for [Udacity][udacity]'s [VR Developer Nanodegree
course][vr-course]. The requirements were to create an apartment scene by
placing models (prefabs) into the scene, adding and configuring lighting
optimized for mobile, and attaching an animation to the globe that is triggered
when the screen is interacted with.

## Requirements

* **Device:** Cardboard
* **Unity:** 2017.1.0p4
* **GVR:** 1.70.0

## Thoughts

I really enjoyed this project. One thing I learned about was the Isometric view
in Unity -- I found this super handy to align objects with the floors and walls
and make sure that nothing was levitating or colliding with anything else.

I also initially attempted to set up the camera myself, but I was having issues --
for some reason, when I tested the scene out on my Cardboard, I noticed the
camera was tilted downward, and I found I had to rotate it upward to compensate.
I suspect this happened because when you hold a Cardboard to your face, you
actually tilt it downward slightly so that you can put your nose through the
nose slots. The camera's field of view was also distorted as well. In any case,
after going back through the Cameras section, I remembered about GVR, and once I
went back and installed this, both the rotation and field of view problems went
away. So this was interesting, and it led me to believe that GVR does some
things behind the scenes that I'm not aware of.

It was also fun to set up the background audio (put on some headphones and
listen closely -- you might hear some birds chirping and the light sound of
traffic!). The way I implemented this specifically was to put the audio into 2D
mode instead of 3D mode so that it does not pan when you turn your head -- I
thought that was a more realistic approach.

## Credit

* Background audio courtesy of [klankbeeld] on [freesound.org].

[udacity]: https://www.udacity.com
[vr-course]: https://www.udacity.com/course/vr-developer-nanodegree--nd017
[klankbeeld]: https://freesound.org/people/klankbeeld/sounds/259315/
[freesound.org]: https://freesound.org
