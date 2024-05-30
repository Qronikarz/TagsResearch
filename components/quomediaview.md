# QuoMediaView
[Glossary](glossary.md) - explanation of below features

## File info
. | . |
---|---
File considered complete | ✔
Fact checked by the developer | ✔ Qronikarz(GitHub)-(v0.3)-(2024-05-30)
Last updated | 2024-05-30

## General info
. | . |
---|---
Name | QuoMediaView
Newest version | 0.3
Type | Media board
Website | ❌
Tag/key words support | ✔
Tag specification | ❌
Supported OS | Windows 7 and above, Linux, macOS, Android, Web
OSs default | ❌
Supported file systems | all [^1]
Required dependencies | Internet browser with JavaScript support
Price | free
Open-source | ✔ AGPL 3
Repository | https://github.com/Qronikarz/QuoMediaView
Roadmap | https://github.com/Qronikarz/QuoMediaView/issues
Documentation | ❌
Written in | HTML 5, CSS 3, JavaScript
Architectures | 32 bit, 64 bit, ARM 32 bit, ARM 64 bit
Updates | ✔
Last update date | 2024-05-30
Works offline | ✔
Language support | English
UI type | GUI
Interface toolkit | ❌
Dark mode | ✔
Accessibility support | ❌
Cross-platform | ✔
Portable | ✔
Install methods | portable version in archive
Theming support | ✔
Tag support links | ❌

## Tagging specific features
. | . |
---|---
Type of tagging | JSON code
Supported files/items | jpg, png, gif, mp4, webm, webp, custom item
Modifies items | ❌
Can modify items | ❌
Modifies metadata | ❌
Tags prevail item modification | ✔ and ❌ [^2]
Custom tags | ✔
Tag groups | ✔
All available tags view | ✔
Multiple items tagging | ❌
Search combining | ✔
Tag autocomplete | ✔
Tag colors | ✔
Exclude tags from search | ❌
Tag blocking | ✔
Tag deleting | ✔
Tag renaming | ✔
Tag aliases | ❌
Tag implications | ❌
Other tag relations | ❌
Tag descriptions | ✔
Not allowed naming symbols | whitespace, JSON control characters, backslash, double quote
Tag sorting | ✔ A-Z
Tags backup | ✔ JSON code, text export
Single item tags view | ✔
Tag statistics | ✔
Hidden tags | ✔
Tagging with AI | ❌
Auto saving | ❌
Auto loading | ✔ [^3]
Cloud saving | ❌

## Tagged items features
. | . |
---|---
Search view types | Grid view, List
View item inside program | ✔
Items view types | Lightbox, Side panel preview, New tab/window
Open item in another program | ❌
Open item disk location | ❌
Item organization | Customizable pagination
Icons | ❌
Thumbnails | ✔
Resizing | ✔
Full-screen mode | ✔
Title/name | ✔
Description | ✔
Item path | ✔
Item Details | Width, Height, Type
Hiding items | ❌
Moving items | ❌
Sorting items | ❌
Duplicate checking | ❌
Items backup | ✔ and ❌ [^4]

## Notes
Recreation of booru projects written from scratch with no frameworks used. Started development because of Windows 7 image viewer not handling .webp files and because of migration to Linux OS needing a familiar set of tools. Is planned to be rewritten for general file explorer with tagging support for every file, not only those browser compatible.

# Contributors list
Qronikarz(GitHub), 

[^1]: Only tested EXT4, NTFS and FAT32. Should work on every file system since the whole program doesn't depend on any file system features and stores tags in custom JSON code.
[^2]: Tags stay unchanged but QMV needs to have current location and file name to display the files so if one of those changes you need to manually correct it in QMV for a correct ones.
[^3]: You can paste JSON code into the .js file to have it auto load it on the start
[^4]: QMV doesn't need to copy files into any special folders or require importing them so actual image/video files backup is up for the user. The JSON code only stores the tags of the files and it can be backed up.
