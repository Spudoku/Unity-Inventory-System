# Unity-Inventory-System
A simple inventory system for Unity. I made it for a different project.

# How to Use This Package
## Item class (Scriptable Object)
1. The default Item class doesn't do anything, so create a subclass that inherits from it.
2. Override Use() in the subclass
3. Create instances in the Editor
4. Assign public fields.
   
## Item Stack (Monobehavior)
This class is just used for the ItemGameObject and Inventory Monobehaviors.

## ItemGameObject (Monobehavior)
1. Attach to a gameobject with a trigger collider
2. Assign an Item instance

## Inventory (Monobehavior)
1. Attach to gameobject
2. if items are to be used by player input, set "isTarget" to true

##Inventory Slot (Monobehavior)
1. use on prefabs for the HUDManager class. No other setup is needed

##HUDManager
1. create a Panel UI object with a Horizontal Alignment Group Component. Attatch a HUDManager component to it.
2. Create a prefab with the following components: Image, InventorySlot, another Image in child object (for background), and finally another child object with a TMPPro text object.
3. In the prefab, assign the sprite image, count text and placeholder fields for the InventorySlot component
4. Assign the inventorySlot prefab to the HudManager
  
