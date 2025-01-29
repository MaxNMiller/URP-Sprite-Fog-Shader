# URP-Sprite-Fog-Shader
A simple custom shader to make 2D sprites interact with Unity URP's built-in fog

![](https://github.com/MaxNMiller/URP-Sprite-Fog-Shader/blob/main/ShaderExample.gif)
---

## ❓ Problem  
In Unity’s Universal Render Pipeline (URP), **sprites are not affected by fog** due to:  
- Default sprite shaders lacking fog calculations.  
- Sprites not writing to the depth buffer, which fog relies on.  

This breaks immersion in 2.5D games where fog is critical for atmosphere.  

---

## 🚀 Features  
- ✅ Works with **perspective and orthographic cameras**.  
- ✅ Maintains sprite transparency/alpha.  
- ✅ Compatible with URP’s **post-processing**.  

---

## 📥 Installation  
1. **Add the shader** to your Unity project:  
   - Create a new shader file (e.g., `SpriteFog.shader`) and paste [the code](#shader-code).  
2. **Create a material** using the shader:  
   - Right-click in the Project window → **Create → Material**.  
   - Set the material’s shader to **Custom/SpriteURPFog**.  
3. **Assign the material** to your SpriteRenderers.  

---

## 🎮 Usage  
1. **Enable fog** in URP:  
   - Go to **Window > Rendering > Lighting > Environment**.  
   - Check **Fog** and configure settings (mode, color, density).  
2. **Assign the material** to sprites:  
   - Drag the material onto a SpriteRenderer’s **Material** slot.  
3. **Tweak settings** (optional):  
   - Adjust `_Color` in the material to tint sprites.  

---


