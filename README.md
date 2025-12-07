For Paracortical Initiative, 2025, Diogo "Theklo" Duarte

Other projects:
- [Bluesky for news on any progress I've done](https://bsky.app/profile/diogo-duarte.bsky.social)
- [Itchi.io for my most stable playable projects](https://diogo-duarte.itch.io/)
- [The Github for source codes and portfolio](https://github.com/Theklo-Teal)
- [Ko-fi is where I'll accept donations](https://ko-fi.com/paracortical)

![Screenshot of dual_slider_demo.png](documentation/dual_slider_demo.png)

# DESCRIPTION
A template for the Godot Engine, for mobile apps where you can navigate different pages or menus by swiping left or right. Each page is represented as a "Card".

# INSTALLATION
This is base Godot project. Duplicate these files into your projects folder, then in the Project Manager when first running Godot, click on "Import" and select the folder with the template. You may then rename the template to the name of your own project.

# USAGE
The `Main_Scene` node includes a box container called "Cardset", this is where all the cards or pages are placed. You may select which card to show first in the inspector of `Cardset`. The project includes a generic "Card" element including both a script and a scene. You should create duplicates of `base_card.tscn` to create new cards with different content, then extend their `base_card.gd` script for the behaviors of that new card.

Theme resources are available so you can see how they were made to look as they do and change to your liking.
`Cardset` includes a signal emitted whenever a card is changed.
In each card you may set the variable `lock_swipe` to `true` to disable changing cards during some critical operation.
Both the title on top and the "Grab_Area" texture at the bottom are intended to allow a user to drag for swiping cards, whereas other UI elements would take over the swiping inputs. Regardless, any part of the card that doesn't respond to input can be dragged to change card.
