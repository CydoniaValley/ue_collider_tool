## Blender Collider Tool Addon For Unreal Engine

*[Addon is stable but in Alpha stage]*

DOWNLOAD:  [UEColliderTool.zip](https://github.com/CydoniaValley/ue_collider_tool/files/13605003/UEColliderTool.zip)

![ue-collisionpanel](https://github.com/CydoniaValley/ue_collider_tool/assets/142062575/ecdcadde-9e10-4349-a5cd-45a1afee2924)
![ue-collisiontool](https://github.com/CydoniaValley/ue_collider_tool/assets/142062575/48d14b03-ab87-4324-a171-fc5334353f7b)
![ue-collisioncollection](https://github.com/CydoniaValley/ue_collider_tool/assets/142062575/d31e6e87-96df-4a6d-9a2a-2f06e64d88e5)

## What this Add-On Does

* Addon Creates and organizes colliders for exporting Static Meshes from Blender to Unreal Engine 4 and 5
* Can create, name, and position your Static Mesh colliders with as little as one or two clicks
* Quicker and simpler than setting up custom colliders inside of Unreal Engine editor.
* Automatically renames colliders for proper Unreal Engine pipeline specs
* Can be used in Edit Mode or Object Mode (currently 'Convex Hull' can only be created in Object Mode)
* Create collisions with as little as one or two clicks
* Fast - Can easily handle thousands of colliders
* Customizable Colors and Shader for better visual organization
* Although fully functional, addon is still a work in progress

Uses all four UE Static Mesh Collider Types:
* Sphere (USP)
* Capsule (UCP)
* Rectange or 'Cube' (UBX or UCX)
* Convex Hull (UCX)

## What this Add-On Does NOT Do
This Addon doesn't automatically build and calculate complex collision shapes with a single click.  There are paid addons out there that claim to do this (for a hefty price).  The collision shapes this addon makes can be done inside of the Unreal Engine editor which can be a tedious process for complex Static Mesh shapes (those who've done it, know).  I developed this addon because I was annoyed with that often slow and annoying process inside of the UE editor with mutiple colliders and complex shapes.

## Basic Useage
### For Cube, Sphere and Capsule Colliders:
1. In the addon panel, select the Rectangle, Sphere, or Capsule Button.
2. Select the Object you want to build a collider for.   Object must be a Mesh.
3. If you want to change the color, select the 'Pin' button next to the addon's color picker.
4. For more control, you can tab into edit mode and select the vertices that you want the collider to cover.
5. Press the big 'Build Collider' button at the bottom of the addon panel.
6. If collider isn't what you wanted, simply delete the collider and repeat.  The addon will automatically adjust for the proper prefix and suffix.


### For Convex Hull Colliders
1.  Select the Object you want to build a collider for.  You must be in Object Mode and the object must be a Mesh Object.
2.  Change color in the addon panel, if desired.
3.  Select the 'Convex Hull(UCX)' mode button.
4.  Press the 'Build Collider' button at the bottom of the addon panel.
5.  You can adust the the decimate rate and the symetry of the collider for more control.  The result can sometimes be hit and miss.  So delete the collider and repeat the steps until you get the desired results.


## Exporting
* Exporting using the FBX format is recommended.  Other formats should work, but I haven't tested them and can't verify this.
* Use the normal pipline as recommended by Unreal Engine.
* For example, if I have 10 objects that make up a 'Courthouse', then at least one of my exported objects will be named 'Courthouse', so my colliders must be named 'UCX_Courthouse_01', 'UBX_Courthouse_01', 'UCX_Courthouse_02'...  It doesn't matter what the other Static Mesh objects are named as long as one them matches the collider(s) root name - 'Courthouse'.  This is a UE dynamic, and has nothing to do with this addon.
* **You can change the the root name of all the colliders quite easily with the 'Renaming' features of this addon.**

*Tested with Blender 3.6 and 4.0.  You should have a fair understanding of the FBX exporting process and Static Mesh Pipeline before using.*
*See Unreal' official documentation here: https://docs.unrealengine.com/5.3/en-US/fbx-static-mesh-pipeline-in-unreal-engine/*

DOWNLOAD:
[UEColliderTool.zip](https://github.com/CydoniaValley/ue_collider_tool/files/13605003/UEColliderTool.zip)
