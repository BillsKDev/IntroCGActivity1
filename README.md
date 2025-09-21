# IntroCGActivity1

**Screenshots of shaders:**


<img width="1160" height="536" alt="image" src="https://github.com/user-attachments/assets/e832d303-b147-46f6-82f0-0870b411fb5b" />



**What was done:**

During class, I worked on a variety of shaders and learned about the code/math behind them such as:

MultiUV Shader - This shader allows me to select two different UV coordinates for the texture on the model, and lets me switch between them in the inspector

MultiUV ViewDir Shader - This shader adds to it with lighting properties like rim color/strength/power and depending on the viewing angle, the amount of light reflected changes with the help of fresnel calculations

WorldPosDebug Shader - This shader takes the world scale and an offset, and based on the world position of the object when you move it around it colors the object differently with RGB colors. For example if an object is higher than another object, the object would appear more green (y axis) so this can be used to understand where objects are positioned in the world and the differences in coordinates

WorldReflection Shader - This shader uses a cubemap and reflects the environment on the object and is useful for things like reflections or shiny objects. You can change the intensity of the reflection or how much the base color and the cubemap color blends between eachother as the values are lerped. The cubemap color also uses fresnel effects/calculations for stronger reflections.

AllProps Shader - This shader uses properties from before and introduced more propeties such as range and vectors and shows how these different properties can affect an object and combines alot of what the other shaders have taught into one shader, with the new range being able to control how visible the shader is and vectors being used for things with multiple values. It combines difffuse, ambient, and reflections.

Lambert Shader - This shader calculates the lambert diffuse and ambient and combines them and combines the color/texture with the diffuse to get a lambert shading effect where the more an object faces toward the light the brighter it appears




**Strengths:**


Proficient with unity and github so no issues with getting things together and setup
Understood how to debug any shader code issues if I had any
Understood the basics of shader creation so the first couple shaders were simple for me to understand

**Weaknesses:**


Sometimes, the HLSL code was very new to me so it took some time to understand what exactly I am doing and how I am changing the shader
Some of the later shaders had some topics that were confusing to me like fresnel calculations and lamberts.
For me to fully understand things, I had to spend a couple hours after class and figure out things I was confused about, so writing back to back shaders makes it so I am writing code in class I don't understand yet



**Opportunities:**

This assignment pushed me to learn more about the specifics of HLSL code and introduced a lot of new CG/Lighting/math concepts for me to study.

**Self Evaluation**

I would give myself a 28/30 since I completed everything all the work in class (see prev submission) and was fully prepared, but since it does take me a long time to fully understand things at my own pace, I rushed through the reflection at the time and definitely needed the extended deadline to fully understand everything I did here.
