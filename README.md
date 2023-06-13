# JsonToMEsh
Imports TrawlerNet in Json format and converts it to a mesh.



<b><h3>Project Details</h3></b>


This project documents our approach to exporting a net as a JSON format from the NetDesigner software. 
As we continue to expand and optimize our Unity solution to handle the real-time rendering of trawl nets with more than 100k elements, 
this repository will provide a  record of our progress and learning.

This project features a custom physics engine that applies Verlet Integration on the node intersections of the nodes.
We achieved this by mapping the indices of the vertex into a dictionary.
Next, we created a new mesh using Unity's Mesh object and assigned the indices and vertices to it. 
Please note that the MeshTopology needs to be set to lines for this process, which necessitates the use of a specific material. 
If you find that this material isn't rendering correctly, you can modify this in the project settings by adding "Unlit/Color" under Graphics.

<b><h3>What's Next (TODOs):</h3></b>

While this project represents a significant step in our research to migrate a mesh to Unity, we are aware that performance optimization is paramount in achieving our end goal. 
The current solution is effective up to 50k elements; beyond this, additional optimization will be necessary. Below are the areas of focus:

<b>-Improve performance to handle meshes with more than 50k elements.</b>

<b>-Identify and implement optimization strategies for the real-time rendering of large-scale trawl nets.</b>

<b>-Develop a more efficient material rendering process.</b>
