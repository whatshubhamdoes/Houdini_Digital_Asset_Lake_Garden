# Houdini Digital Asset : Lake Garden Builder

""" Automatically generates a Lake Garden for you """

== Overview ==

A tool that quickly creates a basic lake garden that looks appealing despite employing primitive geometry for the initial setup.
According to a set of predetermined settings, this HDA arranges, scatters, and distributes the Primitive Geometry
across a landscape grid.

Additionally, this HDA has the capacity to exchange the primitive geometry with higher-level, production-oriented geometry.

== Key References ==
As I live quite close to the Poole Park in Poole, my key reference for this assignment was that.

I saw that whereever there is a lake inside the garden/park, there is always some sand/soil beside it and then, there are multiple pathways leading upto the lake.
I have tried to incorporate these references while giving user the full control to make the garden as they desire.

P.S. the water of the lake is animated. Hit the play button and see for yourself.

Reference Images - 

Link Reference Images - https://drive.google.com/drive/folders/1GA4jplU8hnHMMlye40VDXS_Xcd4OlK1w?usp=share_link

== Using this HDA ==
1. In a new geometry, add a "Curve Beizer" node with order 4. Set view as "Top Viewport".

2. Using this, draw a closed curve as you desire.

3. Add a "Convert" node to the output of this curve. Open the parameters of this node and select "MESH" in the "Convert to" parameter. In level of detail, input the U and V values as 7.

4. Add an "Attribute Paint" node to the output of this convert node. Ensure that the created node has the attribute variable "mask".

5. In the brush parameters of the above-said node, set the "Opacity" to 1 and "Soft Edge" to 0.5 and draw the lake/lakes as you desire.

6. In the same node, set the "Opacity" to 0.5 and "Soft Edge" to 1 and draw the pathway to the lake/lakes as you desire.

7. Connect the output of this "Attribute Paint" node to this HDA and turn on the "Display/Render" flag.

8. Voila. Your lake garden is ready!

# Parameters
Garden Color:
    #id: color_garden
    This controls the color of the garden terrain.
    
Garden Terrain Controls Amplitude:
    #id: Terrain_Amplitude
    This controls the amplitude of the garden terrain.
    
Garden Terrain Controls Element Size:
    #id: Terrain_Element Size
    This controls the element size of the garden terrain.

Grass Length:
    #id: grassLength
    This controls the length of grass.
    
Grass Randomise:
    #id: grassRandomise
    This controls the randomness of grass.
    
Grass Total Count:
    #id: grassTotalCount
    This controls the total count of grass.
    
Grass Color:
    #id: grassColor
    This controls the color of grass.
    
Lake Road Color (below rocks):
    #id: color
    This controls the color of lake road color.
    
Lake Soil Color (below sand):
    #id: color
    This controls the color of lake soil color.
    
Lake Water Color:
    #id: color
    This controls the color of lake water. 
    
Lake Wave Controllers:
    #id: lakewavecontrollers
    These control the wave amplitude, element size and offset values of lake waves.
    
Bench Translate:
    #id: translate
    This controls the translate value of bench.
    
Bench Rotate:
    #id: rotate
    This helps with the rotation value of bench.
    
Bench Scale:
    #id: scale
    This controls the scale value of bench.
    
Bench Total Count:
    #id: benchtotalcount
    This controls the total count value of bench.
    
Bench Randomise:
    #id: benchrandomise
    This controls the randomise value of bench.
    
Bench Seat Color:
    #id: color
    This controls the bench seat color.
    
Bench Metal Color:
    #id: color
    This controls the bench metal color.
    
Bench Back Color:
    #id: color
    This controls the bench back color.
    
Sand Particles Scale:
    #id: scale
    This controls the scale value of Sand Particles.
    
Sand Particles Total Count:
    #id: Sand Particlestotalcount
    This controls the total count value of Sand Particles.
    
Sand Particles Randomise:
    #id: Sand Particlesrandomise
    This controls the randomise value of Sand Particles.
    
Sand Particles Color:
    #id: color
    This controls the color of Sand Particles.
    
Flower Scale:
    #id: scale
    This controls the scale value of Flower.
    
Flower Total Count:
    #id: Flowertotalcount
    This controls the total count value of Flowers.
    
Flower Randomise:
    #id: Flowerrandomise
    This controls the randomise value of Flowers.
    
Flower Bud Color:
    #id: color
    This controls the color of Flower Bud.
    
Flower Stem Color:
    #id: color
    This controls the color of Flower Stem.
    
Bush Scale:
    #id: scale
    This controls the scale value of Bush.
    
Bush Total Count:
    #id: Bushtotalcount
    This controls the total count value of Bushes.
    
Bush Randomise:
    #id: Bushrandomise
    This controls the randomise value of Bushes.
    
Bush Color:
    #id: color
    This controls the color of Bush.
    
Tree Scale:
    #id: scale
    This controls the scale value of Tree.
    
Tree Total Count:
    #id: Treetotalcount
    This controls the total count value of Trees.
    
Tree Randomise:
    #id: Treerandomise
    This controls the randomise value of Trees.
    
Tree Leaves Color:
    #id: color
    This controls the color of Tree Leaves.
    
Tree trunk Color:
    #id: color
    This controls the color of Tree trunk.
    
Rock Scale:
    #id: scale
    This controls the scale value of Rock.
    
Rocks Total Count:
    #id: Rockstotalcount
    This controls the total count value of Rocks.
    
Rock Randomise:
    #id: Rockrandomise
    This controls the randomise value of Rocks.
    
Rock Color:
    #id: color
    This controls the color of Rock.
    
Fountain Scale:
    #id: scale
    This controls the scale value of Fountain.
    
Fountain Total Count:
    #id: Fountaintotalcount
    This controls the total count value of Fountains.
    
Fountain Randomise:
    #id: Fountainrandomise
    This controls the randomise value of Fountains.
    
Lamp Scale:
    #id: scale
    This controls the scale value of Lamp.
    
Lamps Total Count:
    #id: Lamptotalcount
    This controls the total count value of Lamps.
    
Lamp Randomise:
    #id: Lamprandomise
    This controls the randomise value of Lamps.
    
Lamp Light Color:
    #id: color
    This controls the color of Lamp Lights.
