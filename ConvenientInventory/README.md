NexusMods link: https://www.nexusmods.com/stardewvalley/mods/10384

# Convenient Inventory
Adds convenience features to the player's inventory, such as quick stack to nearby chests and favorited items.

## Preview
One of the most tedious parts of any game is inventory management, and this is especially true in Stardew Valley. Every day, whether it be from farming produce, mining rewards, or freshly caught fish, you will be emptying out your backpack to store items into chests on your farm. After a while, this process becomes all too familiar: open chest, deposit items, close chest, open chest, deposit items, close chest, open chest, deposit items, close chest, ... etc.

What if you could stow away all the items taking up space in your backpack, instantly, while keeping the important ones?

![](https://imgur.com/R4QWKVI.gif)

## Features
#### Quick Stack to Nearby Chests
Click the new "Quick Stack to Nearby Chests" button in the player's inventory UI to quickly deposit items from your inventory into any nearby chests which contain that item.

#### Favorite Items
Hold the favorite-hotkey (Left Alt, by default) and select items in the player's inventory to favorite them.

Favorited items are prevented from:
 - Being quick stacked
 - Being trashed
 - Being dropped
 - Being considered when using the "Organize" button in the player's inventory
 - Being considered when using the "Add to Existing Stacks" button in a chest

#### Inventory Page Side-Warp (as of version 1.3.0)
For players using controllers, getting to the right side of your inventory menu is a hassle, as your cursor always starts at the leftmost item slot when opening your inventory. This feature allows the cursor to "warp" side-to-side when at either end of the menu.

![](https://i.imgur.com/3IplIkH.gif)

## Console Commands
 - **player_fixinventory**: Resizes the player's inventory to its correct maximum size, dropping any extra items contained in inventory.
   - Some mods directly modify the player's inventory size, causing compatibility issues and/or leaving extra null items when uninstalled; this command should fix these issues.

## Config
#### Quick Stack to Nearby Chests
 - **IsEnableQuickStack**: If enabled, adds a "Quick Stack To Nearby Chests" button to your inventory menu. Pressing this button will stack items from your inventory to any nearby chests which contain that item.
 - **QuickStackRange**: How many tiles away from the player to search for nearby chests.
 - **IsEnableQuickStackHotkey**: If enabled, pressing either of the quick stack hotkeys specified below will quick stack your items, even outside of your inventory menu.
 - **QuickStackKeyboardHotkey**: Press this key to quick stack your items.
 - **QuickStackControllerHotkey**: Press this button to quick stack your items. (For controller support)
 - **IsQuickStackIntoBuildingsWithInventories**: If enabled, nearby buildings with inventories (such as Mills or Junimo Huts) will also be checked when quick stacking.
 - **IsQuickStackOverflowItems**: If enabled, quick stack will place as many items as possible into chests which contain that item, rather than just a single stack.
 - **IsQuickStackIgnoreItemQuality**: (Requires IsQuickStackOverflowItems to be enabled.) If enabled, quick stack will place items into chests which contain ANY quality of that same item.
   - <details><summary>Preview</summary> 
 
     Before:
 
     ![](https://i.imgur.com/AsA4COq.png)
 
     Quick stack, ignoring item quality:
 
     ![](https://i.imgur.com/HMtFqcE.gif)
 
     After:
 
     ![](https://i.imgur.com/yokobZ1.png)
     </details>
 - **IsQuickStackTooltipDrawNearbyChests**: If enabled, hovering over the quick stack button will show a preview of all nearby chests, ordered by distance.

#### Favorite Items
 - **IsEnableFavoriteItems**: If enabled, items in your inventory can be favorited. Favorited items will be ignored when stacking into chests.
 - **FavoriteItemsHighlightTextureChoice**: Choose your preferred texture style for highlighting favorited items in your inventory.
   - ( 0: ![](https://i.imgur.com/fTMl0FT.png),  1: ![](https://i.imgur.com/NTlia1R.png),  2: ![](https://i.imgur.com/QGztt8Q.png),  3: ![](https://i.imgur.com/MBG2A6e.png),  4: ![](https://i.imgur.com/rZqklnN.png),  5: ![](https://i.imgur.com/FvKpyZV.png),  6: ![](https://i.imgur.com/JO8vsXS.png) )
 - **FavoriteItemsKeyboardHotkey**: Hold this key when selecting an item to favorite it.
 - **FavoriteItemsControllerHotkey**: Hold this button when selecting an item to favorite it. (For controller support)

#### Miscellaneous
 - **IsEnableInventoryPageSideWarp**: If enabled, moving your controller's cursor beyond either side of your inventory menu will warp the cursor to the opposite side.

## Compatibility
 - Supports single player, split-screen local multiplayer, and online multiplayer.
 - Supports controllers by using the left shoulder button (configurable) for favoriting.
 - Supports [Generic Mod Config Menu](https://www.nexusmods.com/stardewvalley/mods/5098) for in-game config editing.
 - Supports [Bigger Backpack](https://www.nexusmods.com/stardewvalley/mods/1845) and other inventory expansion mods (as of version 1.1.0).
 - Supports mods which directly add new inventory slots (as of version 1.3.0).
   - This includes mods such as [Vertical Toolbar](https://www.nexusmods.com/stardewvalley/mods/943), although not recommended as I don't believe it is compatible with other inventory expansion mods and it messes with shifting toolbars.
