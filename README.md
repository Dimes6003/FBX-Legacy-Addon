# FBX-Legacy-Addon
Blender Addon to support import and export of older, unsupported FBX file formats <br>
* Includes FBX version support for Autodesk products ranging between 2006 & 2013 <br>

### Requirements
Tested support for Blender versions 2.9 - 3.1
* [Blender 3.1](https://download.blender.org/release/Blender3.1/) <br>

FBX 2013.3 Converter for Windows from Autodesk's [Official FBX Converter Archives](https://aps.autodesk.com/developer/overview/fbx-converter-archives/) <br>
* [Direct-Download](https://images.autodesk.com/adsk/files/fbx20133_converter_win.exe?_gl=1*1703lrx*_ga*MTQ4ODQ4MTQzMC4xNzg3Nzk4NzY5*_ga_NZSJ72N6RX*czE3ODg5ODkyMTQkbzUkZzEkdDE3ODg5ODkyMTQkajYwJGwwJGgw) <br>

### Installation
1. Download the latest [release](https://github.com/Dimes6003/FBX-Legacy-Addon/releases/latest/)
2. In blender, go to `Edit -> Preferences -> Add-ons`
3. Press `Install` and select the `io_scene_fbx_legacy.zip` you downloaded
4. Under the Add-on's Preferences, set `FBX Converter` to the `FbxConverter.exe` from your Autodesk converter installation
	 > Install path from the **Direct-Download** would be `C:\Program Files (x86)\Autodesk\FBX\FBX Converter\2013.3\bin\FbxConverter.exe` <br>

### Updating
1. Find `Import-Export: FBX Legacy Formats` in `Edit -> Preferences -> Add-ons`
2. Disable then Remove the Addon
3. Restart Blender then follow the **Installation** steps <br>

### Additional Notes
The `FBX Version` panel in the Add-on's Preferences will determine what FBX version you wish to export in <br>
<br>

For a Maya ↔ Blender workflow, Enable `Use Maya Specialized Export Defaults` 
  > This option may also be applicable to other Autodesk products (like 3ds Max) <br>
<br>

When importing an unknown FBX version, it is highly recommended to try `File -> Import -> FBX (.fbx)` first. <br>
If the version is indeed legacy, you will get a notice clarifying the version to you. <br>
Whereas `File -> Import -> FBX Legacy (.fbx)` could cause unexpected errors when importing modern FBX versions. <br>

### License

Based on Blender's FBX import/export code and is distributed under the GNU General Public License, 2.0 or later. <br>
See [LICENSE](https://github.com/Dimes6003/FBX-Legacy-Addon/LICENSE/) for the full license text.
