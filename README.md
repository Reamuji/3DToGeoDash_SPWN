# 3DToGeoDash_SPWN
convert .obj file into a gd level. and you can rotate it in 3 dimention inside the level

blender has the option to export as .obj file just in case you don't know

made with some unauthorized help from https://github.com/patrickbies/spwn-3d lol. 
idk how to read a file, so i take a peek to those who was already there before me. 
btw you should check out that project, it much cooler than the one you're looking at rn

you can message me on discord Reamuji#9847 for whatever reason

## How to use it
1. Put your model on whatever directory written on your terminal.
   pls help, idk how to deal with directory xd
2. type "spwn build 3DToGD.spwn" into the terminal.

you might need to change the offset and resize value based on your model size. i might gonna add some sort of auto size detection system in the future

## How to rotate it
This one is a bit complicated, but ill try to explain it.

So there's 3 object that i call triaxis, they are the obj that govern how the model would rotate. imagine a transparent ball (diameter = 2 block), and then you stick a smaller ball on top, right and front of it. these 3 ball are the triaxis, and if you rotate the ball, the triaxis would move right ? that movement is what make the illusion of the model rotating in 3D. now you need to emulate that movement in 2D

X triaxis (the one you stick on right) = group 1

Y triaxis (the one you stick on top) = group 2

Z triaxis (the one you stick on front) = group 3

the simplest movement you could do (which already written in the code) is moving X & Z triaxis oscillating left and right (with proper easing) which would make the illusion of the model rotating on the Y axis

## Thing to add
#### - system to rotate the triaxis
  im not sure how
#### - zooming in game
  we only need to increase the distance between each triaxis
#### - lower further obj opacity
  if you for expample, give an obj group 1 and 2. and you give each group 50% alpha, both alpha will multiply and your obj will be on 25% opacity
#### - group / obj reduction
  im not sure, but prob we can use less group if we group together obj with same follow value. since GD round the follow value to 2 decimal anyway
  however, it would took much longer to compile
#### - 3D rigging
  maybe we can made another mini copy of the system and while rotate together with the parent, also rotating on their own with it's own axis

this started to be confusing. so lets end it here xd
