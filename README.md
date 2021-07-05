# 3DToGeoDash_SPWN
convert .obj file into a gd level. and you can rotate it in 3 dimention inside the level

made with some unauthorized help from https://github.com/patrickbies/spwn-3d lol
idk how to read a file, so i take a peek to those who was already there before me
btw you should check out that project, it much cooler than the one you're looking at rn

# How to use it
1. Put your model on whatever directory written on your terminal.
   pls help, idk how to deal with directory xd
2. type 'spwn build 3DToGD.spwn into the terminal.

# Thing to add
- system to rotate the triaxis
  im not sure how
- zooming in game
  we only need to increase the distance between each triaxis
- group / obj reduction
  im not sure, but prob we can use less group if we group together obj with same follow value. since GD round the follow value to 2 decimal anyway
  however, it would took much longer to compile
- lower further obj opacity
  if you for expample, give an obj group 1 and 2. and you give each group 50% alpha, both alpha will multiply and your obj will be on 25% opacity
- 3D rigging
  maybe we can made another mini copy of the system and while rotate together with the parent, also rotating on their own with it's own axis

this started to be confusing. so lets end it here xd
