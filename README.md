# Unity Favourites Panel

This will add a new panel with a Tree View where you add categories and can drag-and-drop objects from the Hierarchy or Project panel into.

- The panel can be opened from menu: `Window > Favourites`.
- Use the [+] button in the Favourites panel's toolbar to add a new category.
- Use the [-] button to remove the selected category and all its items or to remove a single selected item.
- Double-click on an item to open it. For example to open a scene you have added to Favourites.
- Right-click to ping a Favourites item in the Hierarchy or Project panel.
- Drag-and-drop items to new categories or other areas of Unity. You can for example drag-and-drop a Sprite from the Favourites panel into the property of a component's Inspector (if that property accept Sprites).

### Technical Info

The favourites system's main asset file is saved next to the editor scripts, so that would be in `\Assets\Favourites\Editor` by default.

The list of favourite scene objects however are saved in an object in the scene since assets/prefabs can't reference objects in the scene. This object is tagged as editor only so it will not end up in your final builds. You will also notice that when you close the scene the favourite scene objects will disapear from the list of favourites. It will be back when you open the scene and did not delete the category the objects was under.

![screenshot](https://user-images.githubusercontent.com/837362/34055429-d059f5ce-e1d7-11e7-8855-1b19dc2ad052.png)
