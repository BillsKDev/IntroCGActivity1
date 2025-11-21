# Intro CG Bonus Marks

**Completed Survey Proof:**
<img width="1892" height="248" alt="image" src="https://github.com/user-attachments/assets/f883502b-2397-4e38-b415-94b1e0b8fd78" />

**PRACTICAL EXPLANATIONS**

Scene created: <img width="1003" height="835" alt="image" src="https://github.com/user-attachments/assets/ffcd7515-1c16-4ada-a6bc-6ea737cf6a2e" />


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


