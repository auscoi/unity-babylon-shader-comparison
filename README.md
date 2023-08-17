# unity-babylon-shader-comparison
This project was created to demonstrate how Unity Shadergraph handles a 360 2:1 equirectangular panorama applied to the view direction as a spherical skybox regardless of the mesh shape, which only affects the overall silhouette.

Compare this Shadergraph shader to my shader written in BablyonJS's Node Material Editor. I use identical math and the same exact image in both projects but the Babylon NME produces terrible looking jagged seam artifacts at the moment. 

**BabylonJS NME Shader: https://nme.babylonjs.com/#E4JAZL**

At first I thought this was due to a float precision issue but it turns out that was not the case. I attempted 4 different mathmatical routes in the Babylon NME which shoudl have all worked but all produced identical results. This leads me to believe this may be a deeper issue with BabylonJS and the way it calculates the edges of the view direction. I'm hoping someone on the BabylonJS forums will be able to help with this issue. I will update this README file if it is resolved.
