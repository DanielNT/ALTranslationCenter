
# AL Translation Center

[![Visual Studio Marketplace Version](https://img.shields.io/vscode-marketplace/v/daniel-nt.al-translation-center.svg?style=flat-square&label=Download%20in%20VS%20Marketplace)](https://marketplace.visualstudio.com/items?itemName=daniel-nt.al-translation-center) ![Visual Studio Marketplace Downloads](https://img.shields.io/visual-studio-marketplace/d/daniel-nt.al-translation-center.svg) ![Visual Studio Marketplace Installs](https://img.shields.io/visual-studio-marketplace/i/daniel-nt.al-translation-center.svg)


This extension allows to improve speed in multilanguage development in AL Language using `developer comments` for adding translations. Previously, the idea was used in AL Language Tools extension (thanks ClipDynamics!).

![Example of developer comments](https://i.ibb.co/ZTbGhC2/example-Label.png)

## Requirements
- AL Language extension.

## Main features
- Xliff translation, based in developer comments (property `comment`).
- Publish and package directly with translations, without need to create tasks or do manually. It creates the package (generate the source xliff), then the translations. Finally, it creates/publish after generating new package, now with embedded translation in it.
- Included basic translation snippets (for `Label`, `Caption`, `OptionCaption`, `Action`, `Tooltip`, `AboutTitle`, `AboutText` and `AdditionalSearchTerms`).
- Generated files are compatible to use with `Microsoft© Multilingual Editor`.
- Search occurrences in case of badly formatted caption translations (prevents of translation process).
- Supports translation of the AL project in use in `multiroot workspaces`.

## Improvements
- Added directly support for more languages (like Catalan, Galician, Basque, Portuguese, Polish).
- Translation texts can contain '=' character.
- Can translate .xlf files created with extension with invalid filenames characters (like ":").
- Edit or add new languages for conversion.

![Example of use](https://i.ibb.co/Z6zTc7W/example-Customization.png)

## Known Issues
- May not work with first versions of AL Language extension.
- You tell me.
