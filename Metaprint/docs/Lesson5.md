# Lesson 5: Introduction to Armature Retargeting
After this lesson, you will learn to animate your own character with your motions!

# Workflow:
1.	[Introduction to Blender](#First)
2.	[Essential Tools and Add-ons Setup](#Second)
3.	[Retargeting Bones](#Third)

<a id="First"></a>
# 1 Introduction to Blender
Blender is a free and open-source 3D creation software that can be used for a variety of tasks such as modeling, animation, rendering, video editing, and more. Let’s play with its controls first!
## 1.1 Open Blender
Open Blender and click any area within the red areas to activate a new project.
![](\Lesson5\opening.png)
You will see a camera, a cube, and a light. We can call them **objects**. You can see that we are in the **Object Mode**. In this mode, we can select, create, move, and delete objects easily. 
![](\Lesson5\photo1.png)
## 1.2 Interface Control
### Mouse Control
| Drag with the small hand icon: Moves the view up, down, left, and right. | Zoom In/Out: Scroll the middle mouse. |
|     :-------------:        |            :-------------:            |
|  ![](/Lesson5/MoveScreen.gif)    |            ![](/Lesson5/Zoom.gif)         |
|        **Drag with the middle mouse button: orbit screen.** |          **Left click: Select object.**   |
|                 ![](/Lesson5/orbit.gif)                                      |            ![](/Lesson5/SelectObject.gif) |
### Keyboard Control
|        X: delete         |          Ctrl + Z: Undo.   |
|           :-------------:             |            :-------------:            |
|                 ![](/Lesson5/delete.gif)         |            ![](/Lesson5/Undo.gif)         |
 **Ctrl + Shift + Z: Redo**.   |           **Keys Positions**        |
|                 ![](/Lesson5/Redo.gif)              |![](/Lesson5/key_position.png)       |
<a id="Second"></a>
# 2. Essential Tools and Add-ons Setup
We will use add-ons to import files. An add-on is a piece of software that extends the functionality of Blender by adding new features or tools.
Here are the add-ons we will use:

**VRM Add-on for Blender** [Click Here to Download](https://vrm-addon-for-blender.info/releases/VRM_Addon_for_Blender-release.zip) \
This add-on use for importing and export VRM files

**Rokoko Studio Live for Blender** [Click Here to Download](https://github.com/Rokoko/rokoko-studio-live-blender/archive/master.zip) \
This add-on use for retargeting animations

**glTF 2.0 format**\
This is Blender Official add-on, no need to download.


## 2.1 Add-ons Installation
The downloaded addon files are zip files, but please do not unzip it, as the unzipped data will not function as an add-on.

1. Start Blender and select menu **Edit** --> **Preferences**.
![](/Lesson5/preference.png)

2. Select **Add-ons** from the left menu when the preference screen, then press the **Install** button in the upper right corner.
![](/Lesson5/addon1.png)
3. Select the addon file you just downloaded, make sure the filename ends with **.zip**, and press the **Install Add-on** button.
![](/Lesson5/addon2.png)
4. Click the checkbox to enable the add-on.
- Make sure Community is enabled. If it is not enabled, hold **Shift** and click it. 
- You can search the addon by using the search bar in the upper right corner. 
![](/Lesson5/addon3.png)
5. Select the save and load button from the lower left corner --> **Save Preferences**.
![](/Lesson5/addon4.png)
Please ensure you have already installed the 3 addons!
![](/Lesson5/enable1.png)
![](/Lesson5/enable2.png)
![](/Lesson5/enable3.png)

 Now you can close the page.

## 2.2 Importing Files
Select all objects by press and drag with left mouse button. Delete them by "X" --> delete.
![](/Lesson5/delete_all.gif)

### Import Rokoko Studio Motion File
Make sure you have already exported a .fbx file from Rokoko Studio website. Now select **file** --> **import** --> **FBX**
![](/Lesson5/Import1.png)
Select the .fbx file you have downloaded, and press the **Import FBX** button.
![](/Lesson5/Import2.png)
Now you can see a human object with bone (or just bone). You can press **space bar** to start/stop the animation of the bone.
![](/png/Import3.png)
### Import Vroid Studio Character File
Make sure you have already exported a .vrm file from Vroid Studio. Now select **file** --> **import** --> **VRM**
![](/Lesson5/Import4.png)
Select the .vrm file you have downloaded, and press the **Import** button.
![](/Lesson5/Import5.png)
Now you can see your character.
![](/Lesson5/Import6.png)
<a id="Third"></a>
# 3. Retargeting Bones
1. Select the armature of the character.
![](/Lesson5/retarget1.png)
2. Switch to edit mode. You can change the mode in the upper left corner.
![](/Lesson5/retarget2.png)
3. Select the big bone at the bottom. Press **x** --> **delete** to delete the bone, as this bone restricts the movement of the armature. Switch to object mode.
![](/Lesson5/retarget3.gif)
4. Find the Rokoko Studio addon by dragging the arrow in the right menu.
![](/Lesson5/retarget4.gif)
5. Login to Rokoko Studio.
![](/Lesson5/retarget5.png)
6. Open the Retargeting panel
- click the eyedropper near **source**, and click the armature from Rokoko Studio.
- click the eyedropper near **target**, and click the armature from Vroid Studio.
![](/Lesson5/retarget6.gif)
7. Click **Build Bone List**. This button pairs the source's bone and the target's bone automatically.
![](/Lesson5/retarget7.png)
8. Click **Retarget Animation**. This button copies the data of the source's bones to the target's bone.
![](/Lesson5/retarget8.png)
9. Now done! you can delete the source object. 
- Go to Right Menu, right click the object --> **delete Hierarchy**. 
This button is to delete all the things inside the collection or object, including its armature, mesh, animation.
- You can also hide the armature by clicking the eye button, to view the animation clearly.
![](/Lesson5/retarget9.gif)
You can now retargeting different motion to the character by 
- Changing the source
- Click **Build Bone List** 
- Click **Retarget Animation**

Remember save the file before you close Blender. 
- Select File --> Save --> give a name to your file --> **Save**
![](/Lesson5/save1.png)