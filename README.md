# Intro CG Activity 3

**SCREENSHOT OF SHADERS**
<img width="1126" height="523" alt="image" src="https://github.com/user-attachments/assets/f9321b92-ccc2-4362-8974-d62a884dbba4" />

**WHAT WAS DONE:**

**Material Vertex Fragment Shader**: This shader samples the texture and scales the UVs while applying a sine transformation distorted along the X and Y axes to create a wavy effect that is adjustable through a slider

**Simple Lighting with Shadows:** This shader compute shadow coordinates using world position and gets the main light direction and computes some Lambertian lighting and samples shadow attenuation for the main light to darken areas not lit by the light

**Tinted Shadow Texture** This shader has a tint shadow and allows real time shadows to appear with a custom color that is tinted instead of making the object completely dark. It calculates the shadow amount then lerps the shadow with the tint and shadow amount and has another shadow caster pass for shadow casting. **To fix the shader I had to add a - to the main light shadows**

**Glass:** I can't fully explain this shader since in-class it didn't work but it creates a class effect by extruding vertices and distorting background using a normal map with fresnel and tinting calculations

**Water:** This shader creates an animated water effect by using a sine wave to displace vertices based on a time and position then adjusting the vertex y position. For wave effect and the wave motion is controlled by frequency, amplitude, and speed parameters

**Water Scrolling:** This shader makes a flat type of water effect by scrolling a water texture and a foam texture at different speeds over time using their UVs. Afterwards it blends them together where the foam texture scrolls half of the speed of the water for a layered effect

**Strengths:** Since I had already created a water shader scrolling UV effect for my project progression I was able to easily understand how the scrolling UV and water shader worked and was able to work around and edit them. I also found that you can invert the shadow shader for an effect that I was looking for.

**Weaknesses:** At this point in time I think my weakness is fully understanding the math behind the code fully so I can adjust it to make it my own. It takes me a little time but I want to eventually do more than just tweaking values and add my own math to the code to create more interesting effects

**Self-Evaluation:** I would give myself a 30/30 since I was able to complete everything and understand them for the most part well before the time limit and wrote my reflection without needing extra time







