# Example Gun for SimplePlanes
![](https://i.imgur.com/07hOH7f.png)

This is a simple gun with a rotating barrel, simple muzzle flash effect, sound effect, and stats identical to the minigun.
[Sound effect source](https://www.freesoundeffects.com/free-sounds/machine-gun-10082/)

To make one yourself:
-Create a normal part
-Add the gun modifier
-Add an AudioSource to the part object. Disable "Play On Awake", and enable "Loop". Set it up to play whatever effect you like.
-Add a child GameObject called `BulletStartPoint`. The bullet will start wherever this is placed.
-Add another child called `BulletStartPoint`. This should be inactive (the checkbox by the GameObject name at the top of the inspector) when you save it, and will be made active when the gun is firing. You can put, for instance, a particle system on there (enable looping and play on awake). Make sure it's inactive when you save.
-Optionally add a child called `SpinningBarrels`. If you do, it will spin when firing like the barrels on the minigun.