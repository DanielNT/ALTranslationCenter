
# AL Translation Center

[![Visual Studio Marketplace Version](https://img.shields.io/vscode-marketplace/v/daniel-nt.al-translation-center.svg?style=flat-square&label=Download%20in%20VS%20Marketplace)](https://marketplace.visualstudio.com/items?itemName=daniel-nt.al-translation-center) ![Visual Studio Marketplace Downloads](https://img.shields.io/visual-studio-marketplace/d/daniel-nt.al-translation-center.svg) ![Visual Studio Marketplace Installs](https://img.shields.io/visual-studio-marketplace/i/daniel-nt.al-translation-center.svg)


This extension allows to improve speed in multilanguage development in AL Language using `developer comments` for adding translations. Previously, the idea was used in AL Language Tools extension (thanks ClipDynamics!).

![Example of developer comments](https://i.ibb.co/ZTbGhC2/example-Label.png)

## Requirements
- AL Language extension.

## Main features
- Xliff translation, based in developer comments (property `comment`).
- Publish and package **directly with translations**, without need to create tasks or do manually.
  1) It creates the package (generate the source XLIFF).
  2) Create the translations from the new source XLIFF file.
  3) Finally, it creates the package or publish (after generating new package), now with updated and embedded translation in it.

- Included basic translation snippets (for `Label`, `Caption`, `OptionCaption`, `Action`, `Tooltip`, `AboutTitle`, `AboutText` and `AdditionalSearchTerms`).
- Generated files are compatible to use with `Microsoft© Multilingual Editor`.
- Search occurrences in case of badly formatted caption translations (prevents of translation process).
- Supports translation of the AL project in use in `multiroot workspaces`.
- You can customize the integrated language mapping, **adding** new languages or **changing** the XLIFF output language.

![Example of use](https://i.ibb.co/dMctxFW/custom-Language-Mapping.png)

## Improvements
- Added directly support for more languages (like Catalan, Galician, Basque, Portuguese, Polish).
- Translation texts can contain '=' character.
- Can translate .xlf files created with extension with invalid filenames characters (like ":").

## Known Issues
- May not work with first versions of AL Language extension.
- You tell me.
