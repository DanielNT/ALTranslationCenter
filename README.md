# AL Translation Center

[![Visual Studio Marketplace Version](https://img.shields.io/vscode-marketplace/v/daniel-nt.al-translation-center.svg?style=flat-square&label=Download%20in%20VS%20Marketplace)](https://marketplace.visualstudio.com/items?itemName=daniel-nt.al-translation-center) ![Visual Studio Marketplace Downloads](https://img.shields.io/visual-studio-marketplace/d/daniel-nt.al-translation-center.svg) ![Visual Studio Marketplace Installs](https://img.shields.io/visual-studio-marketplace/i/daniel-nt.al-translation-center.svg)


This extension allows to improve speed in multilanguage development in AL Language using `developer comments` for adding translations. Previously, the idea was used in AL Language Tools extension (thanks ClipDynamics!).

![Example of developer comments](https://github.com/user-attachments/assets/c77c77ba-8939-43ce-a9ea-ab2c127d2538)

## Requirements
- AL Language extension for Microsoft Dynamics 365 Business Central.
- Visual Studio Code v1.56.0 (April 2021) or higher.

## Main features
- Xliff translation, based in developer comments (property `comment`).
- Commands for directly packaging/publishing with the updated translation.
- Included basic translation snippets (for `Label`, `Caption`, `OptionCaption`, `Action`, `Tooltip`, `AboutTitle`, `AboutText` and `AdditionalSearchTerms`).
- Generated files are compatible to use with `Microsoft© Multilingual Editor`.
- Search occurrences in case of badly formatted caption translations (prevents of translation process).
- Supports translation of the AL project in use in `multiroot workspaces`.
- You can customize the integrated language mapping, **adding** new languages or **changing** the XLIFF output language.

![Example of use](https://github.com/user-attachments/assets/c5a9d53d-b6af-497d-b878-f9a9d81efb81)

- You can map from one abbreviation to multiple languages, separated with `|` character.

![Example of use](https://github.com/user-attachments/assets/a56a5e28-2bad-4371-8776-d1406c9c565e)

## Commands
| Command                                        |                                                                                                                                                                                                                                                                                                                                          |
| ---------------------------------------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| `ATC: Generate Xliff translations from source` | This command generates the translations (based in developer comments) for the current `NameOfExtension.g.xlf` at folder `Translations` (the source XLIFF). This file is created after executing `AL: Package` or `AL: Publish`. Because the file is created after the package, you need to recreate the package to add the translations. |
| `ATC: Package with translations`               | Package *directly with translations*, without need to create tasks or do a repacking manually.                                                                                                                                                                                                                                           |
| `ATC: Publish with translations`               | Generate and publish the package *directly with translations*, without need to create tasks or do manually. You can customize the behavior in settings, and set if you want to publish always with or without debugging without asking.

## Snippets included
- `tcaptionWithTranslation`  
- `ttoolTipWithTranslation`  
- `tlabelWithTranslation`  
- `toptionCaptionWithTranslation`  
- `tprofileWithTranslation`  
- `tprofileDescriptionWithTranslation`  
- `tactionWithTranslation`  
- `tcommentWithTranslation`  
- `taboutTitleWithTranslation`  
- `tadditionalSearchTermsWithTranslation`  
- `taboutTextWithTranslation`  
- `tlockedTrue`  
- `tlockedLabel` 
- `tlockedCaption`  

For a customizable version of language-dependent snippets, use:

- **AL Translation Snippets** &emsp;[![Download AL Translation Snippets](https://img.shields.io/vscode-marketplace/v/daniel-nt.al-translation-snippets.svg?style=flat-square&label=Download%20AL%20Translation%20Snippets)](https://marketplace.visualstudio.com/items?itemName=daniel-nt.al-translation-snippets)


## Improvements
- Added directly support for more languages (like Catalan, Galician, Basque, Portuguese, Polish).
- Translation texts can contain '=' character.
- Can translate .xlf files created with extension with invalid filenames characters (like ":").

## Known Issues
-  `ATC: Package with translations` and `ATC: Publish with translations` will not work with version of AL Language extension lower than `v4.0.182565`.
- You can report an issue at https://github.com/DanielNT/ALTranslationCenter/issues.
