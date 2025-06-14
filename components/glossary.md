# ProgramName
Explanations for used terminology in program specific markdown files.

## File info
. | . |
---|---
File considered complete | If every category is filled and possibly checked by actual long standing users of the program it may get marked with ✔ otherwise ❌. 
Fact checked by the developer | It may be possible that even the users don't know all the features a program offers, so this category is the same as above but only marked ✔ if the actual program developer reads the entry and has no objections. Otherwise marked as ❌. Include the name of the developer, version that was checked and date of approval. Link to the post where the developer approved it if possible.
Last updated | Date of last update of the file in YYYY-MM-DD format
Last checked for updates | Date of when the software was checked for updates in YYYY-MM-DD

## General info
. | . |
---|---
Name | Program name. Multiple programs can have the same name, but they must be different in their markdown files to differentiate them.
Newest version | Newest version that is available to download. Development versions don't count.
Type | Type of the program. There is no actual categorization so there may be differences. Generally used classifications like "file explorer/browser", "media/image board", "gallery" etc.
Website | Link to the program website. Only link to actual website, no repositories or docs.
Tag/key words support | The only exceptions that don't have this are the default file browsers that don't have tag support which is the purpose of this tag research collection. Default file browsers may get added, but other programs that users install on their own must have tag support to be included.
Tag specification | If the program has tag support, specify if it adheres to some known tag specification like user.xdg.tags or different.
Supported OS | Operating System that specific software works on. Software may have a version for other platform, but only versions with tags are to be listed (in case of Steam, you can't view collections on Android). Website in OS means you can put the software on some server and access it through a website with a browser. In case of Windows specify the earliest version that the newest program version works on - like for example Windows 7
OSs default | Operating Systems that it is included by default. Different linux distributions count but only the flagship ones to not make it too big - for example Nemo file browser is used both in Mint and Solus.
Supported file systems | File systems that it works with - NTFS, FAT32, EXT4, BTRFS etc.
Required dependencies | What does it need installed to work correctly.
Price | Program price. Can be either free or paid or both. In case of Steam it allows purchasing games, but the main program is the same no matter if you pay or not.
Account required | If the software needs an ONLINE account to use it. Price doesn't matter here. Local accounts don't count here. 
Open-source | If it is open-source specify the license that it uses
Repository | Link to the code repository of the program
Roadmap | Link to the roadmap of the program
Documentation | Link to the documentation of the program
Written in | Programming/scripting languages that were used to create the program.
Architectures | For example - 64 bit, ARM 32 bit. It can be just general architecture or something more specific it it needs to be
Updates | updated at least once a year with either new features or bugfixes (documentation/readmes do not count)
Last update date | date of last publicly available update
Works offline | Program can be run and started without internet connection and tags can still be used if they are supported. 
Language support | User Interface language - English, Polish, German etc. In case more than 10 languages are supported it's preferable to link a documentation where the languages are listed. Try to list only completed or mostly completed languages.
UI type | The interface of the program - either GUI, CLI or in some cases both.
Interface toolkit | If it uses some toolkits specify them - for example GTK, QT, MAUI
Dark mode | Support of dark mode. If the program only has one mode and it happens to be dark mode it also counts.
Accessibility support | Support of various accessibility technologies. List all of them - for example image alt texts, screen reader, voice input etc.
Cross-platform | Desktop - Desktop only (data works between Windows, Linux and macOS), Mobile - Mobile only (data works between Android and iOS), All - All (data works between all OSs - Windows, Linux, macOS, Android and iOS), Website - Website (can be accessed on a website using a browser on any of the OS).
Portable | Ability to run software from other disks or USB devices. Does not need cross-platform support.
Install methods | List all available install methods, portable versions should be specified to download in archive
Theming support | Program supports theming of UI or some other part. It must be specified by developers.
Tag support links | In case of default file browsers list every link that mentioned working on tag support - may be some forum, some repository issue request or anything that had developers acknowledge or refuse tag support in any shape or form.

## Tagging specific features
. | . |
---|---
Type of tagging | Method of tagging that is used - for example it may be a file rename or some other file/code or a custom unknown solution.
Supported files/items | files and possibly their extensions that the program supports tagging of. Only files that the developers officially list. May be a custom item like bookmarks or others.
Modifies files | Program modifies actual file to store tags - either inside the file in case of text files or in the file name.
Can modify files | Program has the ability to modify the actual files. Some of the programs can't even scan files on their own so this needed separation.
Modifies file metadata | Program modifies metadata of the file.
Tags prevail file/item modification | Tags stay when you rename or move the file/item. May be both, may be partially.
Custom tags | Tags aren't only predefined and can be named by a user
Tag groups | Tags can be grouped or are in groups
All available tags view | Program has some way to show/list all available/created tags to see how many they are
Multiple files/items tagging | A way to tag multiple items with same tag
Search combining | Files/items can be searched using multiple tags. May be a AND, OR or any other join methods.
Tag autocomplete | User doesn't need to type the whole tag to use it, it shows in some form near the search box.
Tag colors | Tags can be colored with either predefined colors or custom.
Exclude tags from search | Disallow items/files that match the searched tag from showing 
Tag blocking | Some way to to specify that files/items with certain tags should not be shown, permanently
Tag deleting | Tags can be deleted - either from the whole or just single file/item
Tag renaming | Tags can be renamed in all files/items. Some programs may have it both ways.
Tag aliases | Tags may combined together. For example some synonyms or the different order of names - first name or last name has different place in Japanese and English, but is referring to the same person.
Tag implications | Some tags can be nested or have certain relations to other tags - for example "sea" in most cases indicates that "water" is used so users searching for "water" should also be shown every "sea" tagged item/file even if it doesn't have "water" tag. There are no ideal synonyms though because even that example may be wrong, imagine sea of lava in fantasy worlds - there's no water there.
Other tag relations | In case there are other tag relations that don't fall into aliases or implications category, list them here
Tag descriptions | Program allows to describe the tags with some short text or maybe even a whole page with examples
Not allowed naming symbols | Symbols that are not allowed to use in tag names - in case of tags stored in file name it probably is certain that no file system specific name characters may be used. Other may have some rules like no "-" at the beginning or no whitespaces at all.
Tag sorting | Ways to sort the tags. List all available
Tags backup | Tags can be backed up in some form to not lose them.
Single file/item tags view | Tags are listed or can be listed while viewing a single item/file.
Tag statistics | Some page or tab where there are statistics for tags - how many are in total, number of their groups or others
Hidden tags | Tags can searched for, but are hidden either from the tag list or single item/file view
Tagging with AI | AI can be used to automatically assign the tags. Some form of object detection or something like that.
Auto saving | Tags are saved automatically and don't need any manual action
Auto loading | Tags can be loaded automatically and don't need any manual action
Cloud saving | Tags are saved into the cloud

## Tagged items features
. | . |
---|---
Search view types | How the items/files are presented when you actually browse them or search the tags. For example grid view, list view or other applicable
View file/item inside program | File/item can be viewed inside the program. For example images may be easily viewed in the program but documents may require external programs.
File/Items view types | How the actual file is viewed - new window, sidebar, same window but fullscreen or any other applicable. It's different from all files/items view - for example Firefox bookmarks may be viewed in sidebar, but they can't be opened in the sidebar and require a new window or tab.
Open file in another program | Some shortcut to open the item in another program - like file browsers opening image viewer 
Open file disk location | Some shortcut to open the file in system file browser
File/Item organization | How the files/items are presented - it may be pagination, infinite scroll, folders or any other form available. List all of them.
Icons | Files/items show icons
Thumbnails | Files/items show thumbnails
Resizing | Files/items can be resized. Generally referred to some form of icons or thumbnails but text can also be resized.
Full-screen mode | It's possible to view items in full screen.
Title/name | Items/files show their names
Description | Files/items have a special place where you can make a short description of the file/item
File path | Location of item/file on the disk is shown
File/Item Details | Various details of the file/item, for example width, height, size etc
Hiding files/items | File/item may be hidden, but not actually removed
Moving files/items | It is possible to move items/files to another folder
Sorting files/items | Items/files can be sorted. List all sorting methods
Duplicate checking | Items/files can be checked for duplicates in some form. For programs it may be during the upload and for file browsers it may require some duplicate checking extension/program
Files/Items backup | Files/items can get backed up. In case of programs that require importing the files to some special folder or converting into the format that they can use you may lose the files with no way of backing them up. Files with their tags should have some form of backup available to avoid that. Some programs may only offer tags without requiring the actual files to be present.
Copying files/items | It's possible to copy files/items .
Deleting files/items | It's possible to delete files/items.
Renaming files/items | It's possible to rename files/items.

## Notes
Some short description about the creation of program or anything worth mentioning about the tags that doesn't match the categories above

# Contributors list
List all people that contributed some info to the file
