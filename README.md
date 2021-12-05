# UABETutorial
A tutorial dedicated to newbies on retexturing AE weapons. Credits to `Toxic#8402` in the AE Discord for helping me with this process and inspiring me to write this tutorial!

I will update this to include NRM and gloss when I get to those parts.

## Prequisites
You can use Paint.NET, Affinity Photo Editor, Photoshop, GIMP, or whatever you like. I use Affinity Photo Editor.

* [Paint.NET](https://www.getpaint.net/download.html)
* [Affinity Photo Editor](https://affinity.serif.com/en-gb/photo/)
* [Photoshop](https://www.adobe.com/products/photoshop.html)
* [GIMP](https://www.gimp.org/downloads/)

## Getting the bundle files
To begin, navigate to your client items folder.

Mine is called `EscapeFromTarkov_Data\StreamingAssets\Windows\assets\content\items\`

I'll choose this bundle to edit:

`EscapeFromTarkov_Data\StreamingAssets\Windows\assets\content\items\mods\"pistol grips\pistolgrip_ar15_hera_arms_hg15.bundle`

You may have up to 3 files here.

```
pistolgrip_ar15_hera_arms_hg15.bundle

pistolgrip_ar15_hera_arms_hg15.bundle.manifest

pistolgrip_ar15_hera_arms_hg15_texture.bundle
```

Copy all you have of the item. I only have 2 -> `.bundle` and `.bundle.manifest`

![Bundles](https://github.com/minihazel/UABETutorial/blob/main/images/Screenshot%20of%20bundles.png)

Make a folder in your Desktop or Documents. Name it `Original Bundle Files`. Paste your bundle items in there.

![Bundles](https://github.com/minihazel/UABETutorial/blob/main/images/Screenshot%20of%20bundles%20in%20backup.png)

## Using UABE

Presuming you have downloaded UABE (Unity Assets Bundle Extractor), use 7Zip to extract the `64bit` folder into your Documents.

Open `64bit` -> Open `AssetBundleExtractor.exe`

![UABE](https://github.com/minihazel/UABETutorial/blob/main/images/Screenshot%20of%20UABE%20with%20no%20file%20opened.png)

Click File > Open, and find the original `pistolgrip_ar15_hera_arms_hg15.bundle` file. Select it.

![UABE Compression Window](https://github.com/minihazel/UABETutorial/blob/main/images/Screenshot%20of%20UABE%20asking%20for%20uncompression.png)

Press Yes.

Make a folder inside next to your `Original Bundle Files` folder. Name it `Uncompressed UABE Files`.

Save your new file as `pistolgrip_ar15_hera_arms_hg15` (**without the `.bundle` part**)

![UABE with file](https://github.com/minihazel/UABETutorial/blob/main/images/Screenshot%20of%20UABE%20with%20file%20opened.png)

Now, press Info.

![UABE Info](https://github.com/minihazel/UABETutorial/blob/main/images/Screenshot%20for%20UABE%20Info.png)

Now, widen the `Name` field and select `pistolgrip_ar15_hera_arms_hg15_LOD0_diff`. It's the 2nd item from the top.

Press `Plugins` -> `Export to .png`.

Make a folder next to your `Uncompressed UABE Files` folder. Name it `UABE Exported to PNG`. Place your png file in there.

Now, keep UABE open. Do NOT close it.

## Editing the texture
Open a photo editor of your choice. It needs to have a Layers feature. I've chosen Affinity Photo Editor.

![Affinity](https://github.com/minihazel/UABETutorial/blob/main/images/Screenshot%20of%20Affinity.png)

Drag and drop the new PNG file into your photo editor.

![Affinity](https://github.com/minihazel/UABETutorial/blob/main/images/Screenshot%20of%20Affinity%20with%20png.png)

**Affinity specific:** De-select the lock icon to be able to delete this layer later:

![Affinity](https://github.com/minihazel/UABETutorial/blob/main/images/Affinity%20Layers.png)

Now, find a texture you'd like to use. I'll be using a hexagon pattern I found on google:
![Hexagon](https://wallpaperaccess.com/full/2909118.jpg)

Drag and drop the jpg or png texture on top of the first PNG.
![Affinity](https://github.com/minihazel/UABETutorial/blob/main/images/Screenshot%20of%20Affinity%20with%20png%202.png)

Resize your texture accordingly to the background layer, which is normally smaller, to fit it.

Now, select the Background layer. Press `Delete`.
![Hexagon](https://github.com/minihazel/UABETutorial/blob/main/images/Affinity%20Layer%20Deletion.png)

Set the opacity of your main layer to 25%, 50% or 100%. It depends on how visible your texture should be in-game.
![Opacity](https://github.com/minihazel/UABETutorial/blob/main/images/Affinity%20Opacity.png)

Export your png to somewhere safe. `File` -> `Export As` or `Save As` and save as PNG.

## Importing into UABE
Select `Plugins` and select `Edit` on the bottom. Press OK.

At the bottom, press `Load` next to Texture. Find the PNG you just saved from your photo editor. Press OK.

`Select a quality setting` -> Press OK.

Press `File` -> `Save` then `Close`

### Optional: gloss
In UABE Info section, find the item in the list that ends with `_gloss`

It should be the 5th item from the top.

Select the item and press `Remove` bottom right.

### Saving texture to game
Press `File` -> `Save` in the main window.

Navigate to your folder:

`EscapeFromTarkov_Data\StreamingAssets\Windows\assets\content\items\mods\"pistol grips\pistolgrip_ar15_hera_arms_hg15.bundle`

Select the item you copied in the first step, and overwrite it. Press Yes.

## Launching the game
Clear the cache:

`Server\user\cache` -> Delete `cache`

Restart your server and find a gun to put your AR-15 Hera Arms HG15 grip on.

## In-game result
25% opacity texture in-game:
![25](https://github.com/minihazel/UABETutorial/blob/main/images/25.png)

100% opacity texture in-game
![100](https://github.com/minihazel/UABETutorial/blob/main/images/100.png)
