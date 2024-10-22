# CIS 5660 HW03 Procedural Buildings

My inspiration is the houses fromm the lorax movie. 



## Project Overview
In this homework you’ll gain more experience with tool creation and loops. The core of this homework will be following a Procedural House tutorial to create a multi-floor building generator. The tutorial is linked here: 
https://www.youtube.com/watch?v=uIe97023sDk&t=979s&ab_channel=SimonHoudini 

## Part 0: Setup and Planning 
### SideFX Labs 
The tutorial requires some nodes from SideFX Labs. If you haven’t already installed it, you can do so at the “Labs/Packages” tab of the Houdini Launcher.  

### Project Planning
Before you begin on this project, skim through the tutorial and then pick a building type/style you’d like to emulate (either from photos or concept art). You should watch the entirety of the tutorial  before committing to a style so you can pick something that is manageable and will be achievable using the techniques in the tutorial.  
Of course, you’re welcome to adapt the setup to support additional logic/features to match your style, and particularly complex additions could merit extra credit :) On the other hand, if you’re newer to Houdini and want to stick relatively close to the tutorial, that’s okay too. Just be sure to think through what changes your chosen buildings will require (additional assets? different placement logic?) before diving into the project so you don’t bite off more than you can chew.  
Make sure the include the reference you select in your README, and don’t forget to credit your sources.  
Here are a few examples of possible building styles that could be a decent fit for inspiration:
CIS 5660 HW03 Procedural Building 1 
https://www.behance.net/gallery/23773965/ISOBuilding-concept-art 

https://polycount.com/discussio 
low-poly-building
https://www.artstation.com/artwork/m6xYy 

## Part 1: Box Stacking HDA
First, start by following the tutorial to make a simple HDA that stacks boxes on each other.  Important note about HDA creation:  
Creating an HDA saves a .hda file at the location you specify with the definition of your HDA. Be sure to submit this .hda file along with your .hip file so we can see the contents of your tool.  
Alternatively, when you save your HDA you can choose the “Embedded in HIP File” option (rather than specifying the path), and the hda definition will be automatically embedded in your hip file (and no additional files will be needed with submission).  

## Part 2: Add Details
Next, Simon adds details to the boxes to create floors by refiing the shape and adding details like windows, doors, and balconies.  
Create your own models for windows, doors, and balconies based on your chosen style using Houdini. For each of the three types, create a Null “control” node with parameters that affect your window/door/balcony output (similar to how we made a control node for the jellyfish).  
You should have parameters to drive the width and height of the doors, windows, and balconies, as well as at least one other parameter of your choosing on each one (ex: double vs single doors, windows with and without shutters, and type of balcony railing). Apart from that, you can go as simple or complex as you like!  
Then follow Simon’s setup to integrate your windows, doors, and balconies into your buildings.  
CIS 5660 HW03 Procedural Building 2 

## Part 3: Pillars and Border
Continue following the tutorial to add pillars and borders to each floor. 

## Part 4: Supports
Continue following the tutorial to add supports to floors that overhang other floors.  
(Optional) Extra Credit 
Throughout the tutorial, Simon mentions ways you could extend his project setup. Implement any of his suggestions: 
More complex logic for creating supports (handle different length supports differently) Add more parameters to the user interface (for example, x and z offset options) UV and shade your models 
Add a “manual node” where users can control detail placement manually 
Add additional types of feature models (like fire escapes or chimneys). Note that, depending on what you choose, you might need to add new logic to integrate them into your building (ex: chimneys go on top instead of being chained on the side, fire escapes should be on one side of the building and go all the way down). We’ll award more extra credit accordingly.  
Add some flair to your scene by dressing together multiple buildings or additional procedural props or background elements 
Render your scene 

## Submission
Update your README with 
A description of your project 
A video of your building tool in action 
Create a pull request to this repository 
Submit your Houdini file to Canvas along with a link to your pull request 
IMPORTANT NOTE: make sure your HDA is either embedded in the HIP file or included with your submission (see the instructions under “Part 1: Box Stacking HDA” for additional details).
