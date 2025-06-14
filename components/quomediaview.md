# QuoMediaView
[Glossary](glossary.md) - explanation of below features

## File info
. | . |
---|---
File considered complete | ✔
Fact checked by the developer | ✔ Qronikarz(GitHub)-(v0.3)-(2025-06-14)
Last updated | 2025-06-14
Last checked for updates | 2025-06-14

## General info
. | . |
---|---
Name | QuoMediaView
Newest version | 0.3
Type | Media board
Website | ❌
Tag/key words support | ✔
Tag specification | ❌
Supported OS | Windows 7 and above, Linux, macOS, Android, Website, iOS
OSs default | ❌
Supported file systems | all [^1]
Required dependencies | Internet browser with JavaScript support
Price | free
Account required | ❌
Open-source | ✔ AGPL 3
Repository | https://github.com/Qronikarz/QuoMediaView
Roadmap | https://github.com/Qronikarz/QuoMediaView/issues
Documentation | ❌
Written in | HTML 5, CSS 3, JavaScript
Architectures | 32 bit, 64 bit, ARM 32 bit, ARM 64 bit
Updates | ❌
Last update date | 2024-05-30
Works offline | ✔
Language support | English
UI type | GUI
Interface toolkit | ❌
Dark mode | ✔
Accessibility support | ❌
Cross-platform | All, Website
Portable | ✔
Install methods | portable version in archive
Theming support | ✔
Tag support links | ❌

## Tagging specific features
. | . |
---|---
Type of tagging | JSON code
Supported files | jpg, png, gif, mp4, webm, webp, custom item
Modifies files | ❌
Can modify files | ❌
Modifies file metadata | ❌
Tags prevail item modification | ✔ and ❌ [^2]
Custom tags | ✔
Tag groups | ✔
All available tags view | ✔
Multiple files tagging | ❌
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
Single file tags view | ✔
Tag statistics | ✔
Hidden tags | ✔
Tagging with AI | ❌
Auto saving | ❌
Auto loading | ✔ [^3]
Cloud saving | ❌

## Tagged files features
. | . |
---|---
Search view types | Grid view, List
View file inside program | ✔
File view types | Lightbox, Side panel preview, New tab/window
Open file in another program | ❌
Open file disk location | ❌
File organization | Customizable pagination
Icons | ❌
Thumbnails | ✔
Resizing | ✔
Full-screen mode | ✔
Title/name | ✔
Description | ✔
File path | ✔
File Details | Width, Height, Type
Hiding files | ❌
Moving files | ❌
Sorting files | ❌
Duplicate checking | ❌
Files backup | ✔ and ❌ [^4]
Copying files | ❌
Deleting files | ✔ and ❌ [^5]
Renaming files | ❌

## Notes
Recreation of booru projects written from scratch with no frameworks used. Started development because of Windows 7 image viewer not handling .webp files and because of migration to Linux OS needing a familiar set of tools.

No updates planned because of being rewritten into a more general tagging program that does not only focus on media files.

# Contributors list
Qronikarz(GitHub), 

[^1]: Only tested EXT4, NTFS and FAT32. Should work on every file system since the whole program doesn't depend on any file system features and stores tags in custom JSON code.
[^2]: Tags stay unchanged but QMV needs to have current location and file name to display the files so if one of those changes you need to manually correct it in QMV for a correct ones.
[^3]: You can paste JSON code into the .js file to have it auto load it on the start
[^4]: QMV doesn't need to copy files into any special folders or require importing them so actual image/video files backup is up for the user. The JSON code only stores the tags of the files and it can be backed up.
[^5]: QMV doesn't have access to actual files so they can't be deleted from the disk, but they can be deleted inside QMV which removes all the tags from their entry and you can add them again later manually.
