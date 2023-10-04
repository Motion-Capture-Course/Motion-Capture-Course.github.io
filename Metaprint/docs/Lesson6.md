# Lesson 6: Convert Character to Printable
After this lesson, you will learn to export a 3D print file with your character and pose!

First, please open the saved .blend file in the previous lesson.
Also, you should download 3D builder to fix the 3D model to printable.
**3D Builder** [Click Here to Download](https://3d-builder.en.uptodown.com/windows/download)

Workflow: 
1. Export Character with Pose
2. Convert File to Printable

## 1. Export Character with Pose
1. As we want to have a backup for the original model, duplicate the bone and the character by:
- selecting them 
- press **Shift + D**
- left click
![](/Lesson6/duplicate.gif)
2. Selecting the pose that you want to print by adjusting the timeline. 
- You can find the timeline at the bottom.
- You can change the "Start" and "End" number of the timeline to adjust its length. 
![](/Lesson6/timeline.gif)
3. 
- Select the face of the character. 
- Select Data Properties in the right corner. You can see there is a Shape Keys panel.
- *Shape Keys are a set of vertex positions that can be stored and manipulated. It is powerful commonly use to create different facial expressions for a character. But now we don't need them.
![](/Lesson6/shapekey1.gif)
4. - Select the second shape key. 
- Click the arrow at right. 
- Click **Delete All Shape Keys**, because we cannot apply object's modeifiers with shape keys.
![](/Lesson6/shapekey2.gif)
5. - Select Modifier Properties. 
- Click the arrow next to the Armature modifier. 
- Click **Apply**. This apply the transformation of the character affected by the armature. If we don't apply, the exported file will become T-pose.
![](/Lesson6/modifier1.gif)
6. - Select the body of the character. 
- As the body of the character doesn't have shape keys, we can go to Modifier Properties directly. 
- Click the arrow next to the Armature modifier. 
- Click **Apply**.
![](/Lesson6/modifier2.gif)
7. Select both the body and the face. You can hold **shift** and left click to multi-select objects.
![](/Lesson6/export_stl.gif)
8. Click **File** --> **export** --> **_Stl(.stl)**
![](/Lesson6/exportstl2.png)
9. Click **Include** --> enable **Selection Only**, because we only want to export the selected objects. Also name the file. Click **Export STL**.
![](/Lesson6/exportstl3.png)

## 2. Convert File to Printable
1. After export, please open 3D Builder software.
![](/Lesson6/lesson6-1.png)
2. Open the .stl file.
![](/Lesson6/lesson6-2.png)
![](/Lesson6/lesson6-3.png)
![](/Lesson6/lesson6-4.png)
3. Click **Import Model**.
![](/Lesson6/lesson6-5.png)
Click the box in the lower right corner.
![](/Lesson6/lesson6-6.png)
4. Click the item icon in the upper left corner.
Click **Save as**.
![](/Lesson6/lesson6-7.png)
5. Rename and choose .stl format.
Export the file.
![](/Lesson6/lesson6-8.png)