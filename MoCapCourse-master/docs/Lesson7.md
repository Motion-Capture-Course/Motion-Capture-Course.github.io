# Lesson 7: Export the character file with animation

First of all, open the saved .blend file at the previous lesson. We delete all the characters that duplicated last lesson.
![](\Lesson7\lesson7-1-1.gif)
We should fix two problem before export the character file with animation. 
1. Texture
2. File size

Othewise the character will have no color, or cannot upload the file to Oncyber.

Workflow:
1. Converting Texture
2. Reducing File Size
3. Export the File

## 1. Converting Texture
We will export the character file to .gltf format. But this file format cannot read the original texture of the VRM file.

1. Go to shading mode. You can find it at the top menu.
![](\Lesson7\lesson7-2-1.gif)
2. Select the face. you will see many nodes at the bottoms. But don't worry! It isn't too difficult.
![](\Lesson7\lesson7-15.gif)
3. Let's learn about the controls in Shader Editor:
- You can drag by mouse middle button to move the screen.
- You can scroll the mouse to zoom in/out.
- You can add new nodes by pressing **Shift + A**.
![](\Lesson7\lesson7-16.gif)
4. Delete all the nodes except the **Lit Color Texture**. You can delete the selected nodes by pressing **X**.
The **Lit Color Texture** is at the top area. It is the main texture of the character.
* If you delete wrong, press **Ctrl + Z** to undo.
![](\Lesson7\lesson7-24.png)
![](\Lesson7\lesson7-17.gif)
5. Create a **Principled BSDF Node**. You can create it by pressing **Shift + A** --> Search, find "Principled BSDF". 
![](\Lesson7\lesson7-18.gif)
6. Create a **Material Output Node**. You can create it by pressing **Shift + A** --> Search, find "Material Output". 
![](\Lesson7\lesson7-19.gif)
7. Connect the nodes. You can connect them by dragging the points.
![](\Lesson7\lesson7-20.gif)
Color --> Base Color
Color --> Emission
Alpha --> Alpha
BSDF --> Surface
![](\Lesson7\lesson7-25.png)
8. Select the body. Repeat the step 4-7.
![](\Lesson7\lesson7-21.gif)
![](\Lesson7\lesson7-22.gif)
![](\Lesson7\lesson7-23.gif)
![](\Lesson7\lesson7-25.png)
**Finished!**
## 2. Reducing File Size
Let's go back to **Layout**. You can find it at the top menu.
![](\Lesson7\lesson7-8.gif)

We need to delete shape keys of the face like the last lesson to reduce the file size.
1. select the character face
2. Go to Data Properties in the right panel.
3. select the 2nd shape key
4. click the arrow at the right
5. click "Delete All Shape Keys"
![](\Lesson7\lesson7-13.gif)
## 3. Export the File
1. Select the original character and armature.
Go to **File** --> **export** --> **glTF 2.0 (.glb/.gltf)**
Remember to enable "limited to selected Objects", otherwise all objects in this blender file will be exported.
Rename the file and save it.
![](\Lesson7\lesson7-14.gif)
Make sure file size is under 8MB. 
2. You can preview the .gltf file here. Go to "Animation" and select different animations.
<iframe src="https://gltf-viewer.donmccurdy.com/" width="700px" height="500px" frameborder="0" > </iframe>
![](\Lesson7\lesson7-15.png)