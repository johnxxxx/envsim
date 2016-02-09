Senior undergrad computer science project. Intended to be useful in demonstrating and understanding various techniques in graphics and artificial intelligence.  This project may be useful in gaining an idea of how to approach certain problems in game development.  I am sharing this project in the hopes it might be useful to amateur game developers or enthusiasts who are looking for some ideas on how to implement certain ideas.  Please keep in mind this project was built as I was learning the graphics and algorithms myself, so it is not intended to present the "best" solutions to each problem.

This goal of this project was to create a customizable real-time virtual environment from scratch.  This environment includes terrain, weather, and artificial intelligence demonstrated through wildlife agents.  In addition, I created my own user interface framework for XNA-based projects.  The original inspiration for this project was automated terrain generation using heightmaps, but the final product has grown into something far greater.  There’s no specific purpose to this project, but it could serve as a foundation to a computer game or simulation.


---


Please download the readme file for basic information.

Important: Note the license.  My hope is that this project will be used as an educational resource, not a commercial one.  If you try to sell copies of a game on XBOX live that uses any of this code, you also have to make the source code of your entire project available.  You also have to provide a copyright notice others can see: the GPL requires all copies to carry an appropriate copyright notice.

Known issues:

-The render targets used for shadows and bloom may not be supported by your graphics card.  Change the surface format in their definition to use the graphics device's default display mode format if this is a problem.

-Snow particles are not properly blended with distance on some graphics cards.  This has to do with how each graphics card handles the rendering of point sprites.  To resolve this issue, you must use a billboard implementation instead.

-Some bounce balls fall through the terrain mesh.  This likely has to do with my changing the terrain from being along the X/-Z axes to the X/Z axes.  I will fix this soon.