# Intro CG Bonus Marks

**Completed Survey Proof:**
<img width="1892" height="248" alt="image" src="https://github.com/user-attachments/assets/f883502b-2397-4e38-b415-94b1e0b8fd78" />

**PRACTICAL EXPLANATIONS**

Scene created: <img width="1003" height="835" alt="image" src="https://github.com/user-attachments/assets/ffcd7515-1c16-4ada-a6bc-6ea737cf6a2e" />

Scene Setup Explanation: To setup the scene i have the player on a rocky/grassy environment to show the land, i used a skybox from the asset store to give the night look, i just used primitives for the floor and trees since the shaders are able to give them the exact look without actually needing an extra model. I have trees setup in the back to follow the environment with a grassy area and a rocky area with a water area at the bottom with the enemy moving side to side.

What shaders were created: Water shader, Bump Shader, and, Flat shading

Water shader explanation: A water shader was made to simulate a realistic scrolling water environment to fit the low poly look. The water shaders animates water a texture surface by scrolling two textures at different speeds based on time. For this shader it uses water and foam and these are blended together to create the unique water effect

Flat shading Explanation:  Flat shading was used to make the trees and the grass look more realistic in a low poly environment. Normal mapping has normals on each polygon face of an object so whenever light affects each face, it affects it differently for each face.

Bump Mapping Explanation: Bump mapping was used on the rocky area to give it a very defined grainy and rough look and make the ground look more realistic. This was done by using a bump texture and applying normal mapping by transforming it to tangent to world to make the lighting calculated realistically with an intensity value that I can adjust

Assets for character: https://assetstore.unity.com/packages/3d/characters/toony-tiny-people-demo-113188

**Rendering Pipepline fundamentals**

What the rendering pipeline is: A pipeline that proccesses how a 3d scene turns into a 2d screen by using different shader stages with vertex, uniform and element data to the gpu to render a scene with shaders, rasterizer and buffers

Name Components: vertex shader, fragment shader, rasterizer, framebuffers

Illustrate: <img width="624" height="337" alt="image" src="https://github.com/user-attachments/assets/79eb8e47-80bf-4dc8-aee5-490e353f7557" />

Provide examples: cpu sends data to gpu, triangle assembly takes vertices and forms them together, vertex transforms all the vertex data, rasterizer converts pixels to fragments and fills screen pixels, and the fragment shader colors each pixel and the framebuffer handles depth and color buffers for example

Examples in class: examples in class show the stencil buffer handling what part of an object is shown through the framebuffer

What is forward and deferred rendering: These are different stages as to how an object is rendered where forward is the typical way with one pass for rendering each object and applies lighting passes for EACH light and deferred has two stages with a storing data in gbuffer and waiting to render all the lighting related information through the g buffer data for lighting calculations on every pixel for more advanced lighting scenes

Typical applications: Transparent objects work well with forward, and maybe a horror environment which needs a lot of lights to set a scary mood would need deferred

How would you explain using a diagram: The 3d model is passed through a vertex modifier that alters the position and vertex data. then it moves to frag function that outputs a color, and then only accumlating the lighting passes. For deferred it uses a G buffer before the lighting stage where it waits and uses the G buffer data with stuff like textures, normals, albedo, annd specular to apply post processing effects and the final image is produced at the end

Provide and explain examples of it: For deferred rendering you can use some blurring to allow something to be the focus of the image

What are vetex/fragment shaders: programmable shader stages that run on the gpu that are written in shader languages like GLSL and HLSL

Typical applications for vertex and fragment: For vertex shaders you could be transforming an objects vertices from world space to clip space and fragment shader changes each pixel of an object

How to explain using a diagram: I would explain it by showing a vertex shader would run on each vertex of an object and transform each one, and the fragment shader would run on each pixel and adjust the color of the pixel
<img width="814" height="518" alt="image" src="https://github.com/user-attachments/assets/69c1e425-5960-482f-910f-58c1f7cedcf1" />

Examples of each: Changing the view projection for vertex shader and incorporating phong lighting for fragment shader


