# Intro CG Activity 3

**SCREENSHOT OF SHADERS**

**WHAT WAS DONE:**

<h4>Material Vertex Fragment Shader:<h4> 
  <p>This shader samples the texture and scales the UVs while applying a sine transformation distorted along the X and Y axes to create a wavy effect that is adjustable through a slider</p>

**Simple Lighting with Shadows:** This shader compute shadow coordinates using world position and gets the main light direction and computes some Lambertian lighting and samples shadow attenuation for the main light to darken areas not lit by the light

**Tinted Shadow Texture** This shader has a tint shadow and allows real time shadows to appear with a custom color that is tinted instead of making the object completely dark. It calculates the shadow amount then lerps the shadow with the tint and shadow amount and has another shadow caster pass for shadow casting. **To fix the shader I had to add a - to the main light shadows**

**Glass:**

**Water:** This shader creates an animated water effect by using a sine wave to displace vertices based on a time and position then adjusting the vertex y position. For wave effect and the wave motion is controlled by frequency, amplitude, and speed parameters






