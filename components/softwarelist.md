# Contents:
1) [OS Default file browsers](#os-default-file-browsers)
2) [Files](#Files)
3) [Media](#Media)
4) [Text](#Text)
5) [Bookmarks](#Bookmarks)
6) [Games](#Games)
7) [Other](#Other)

# Explanations

Every program listed in here must have some sort of tagging feature which in addition to the ability to tag items, was minimally defined as:
1) Name of the tag must be chosen by user
2) Viewing the item that was tagged must show all the tags that were attached to this item
3) Searching with the tag should show all items that have the tag that was used in search.

**OS default file browsers** are listed even if they do not support tagging files. It's a special exception to showcase how file tagging concept is unknown. File browsing programs have less features in their table because each of them is nearly identical with each other - type, free price/included, constant updates, lack of cross-platform, UI type.

Every added and listed program must have a link to more detailed description in their own .md file in components folder. The markdown table only has place for few features, but the programs have various tagging capabilities.

Software may be listed in more than 1 table in some cases but generally if something is classified in files category then it doesn't need to be classified in media/documents or other categories.

Tables are sorted by the number of check marks first and software name second.

**Account not required** - Due to many programs needing account this category is placed next to the price to quickly see if you need ONLINE account to use the program. Worded with "not" to make the checkmark count for the above sorting rule. Local accounts don't count here.

**Supported OS** - Operating System that specific software works on. Software may have a version for other platform, but only versions with tags are to be listed (for example: Steam - you can't view collections on Android). Website in OS means you can put the software on some server and access it through a website with a browser.

**updates** - Updated at least once a year with either new features or bugfixes (documentation/readmes do not count)

**cross-platform** - D - Desktop only (data works between Windows, Linux and macOS), M - Mobile only (data works between Android and iOS), A - All (data works between all OSs - Windows, Linux, macOS, Android and iOS), W - Website (can be accessed on a website using a browser on any of the OS). Any of them count for the checkmark. A =/= W for clearer categorization.

**portable** - Ability to run software from other disks or USB devices. Does not need cross-platform support.

## Categories explanations
1) **OS Default file browsers** - file browsing programs included by default on various operating systems
2) **Files** - programs that deal with many different files - images, videos, documents, texts, archives etc.
3) **Media** - programs that deal with only media files - images, videos, audio etc. 
4) **Text** - programs that deal with text files. They may or may not offer the ability to edit those text files
5) **Bookmarks** - programs that deal with website bookmarks. This should be specifically mentioned somewhere in the documentation of the program.
6) **Games** - programs that deal with games and the game library organizing.
7) **Other** - programs that don't match any of the above categories

# OS Default file browsers

⌄Name\Features> | OS/DE/Brand | Tags/keywords | Open-Source | Tag specification | Cross-platform
---|---|---|---|---|---
[File Explorer](file-explorer.md) | Windows | ✔ not every file type
[Finder](finder.md) | macOS | ✔
[Dolphin](dolphin.md) | Linux/KDE Plasma | ✔ | ✔ GPL 2 | ✔ user.xdg.tags
[Caja](caja.md) | Linux/MATE | ✔ | ✔ GPL 2 | ✔ user.xdg.tags
[Index](index.md) | Linux/MauiKit | ✔ | ✔ LGPL 3
[Files](ios-files.md) | iOS | ✔
[Files](ipados-files.md) | iPadOS | ✔
[Nemo](nemo.md) | Linux/Cinnamon | | ✔ GPL 2
[cosmic-files](cosmic-files.md) | Linux/COSMIC | | ✔ GPL 3
[Thunar](thunar.md) | Linux/Xfce | | ✔ GPL 2
[Nautilus](nautilus.md) | Linux/GNOME | | ✔ GPL 3
[Files](chromeos-files.md) | ChromeOS
[Files by Google](files-by-google.md) | Android/Google
[Files](lineageos-files.md) | Android/LineageOS | | ✔ Apache 2.0
[Samsung My Files](samsung-my-files.md) | Android/Samsung
[Mi File Manager](mi-file-manager.md) | Android/Xiaomi

# Files

⌄Name\Features> | Type | Supported OS | Price | Account not required | Open-Source | Updates | Cross-platform | Portable
---|---|---|---|---|---|---|---|---
[filetags](filetags.md) | File name modification management | Windows, Linux, macOS | free | ✔ | ✔ GPL 3 | ✔ | D | ✔
[TagSpaces](tagspaces.md) | File manager | Windows, Linux, macOS, Android, Website | free + paid | ✔ | ✔ AGPL 3 | ✔ | D, W | ✔
[TagStudio](tagstudio.md) | File manager | Windows, Linux, macOS | free | ✔ | ✔ GPL 3 | ✔ | D | ✔
[Spacedrive](spacedrive.md) | File browser | Windows, Linux, macOS | free | ✔ | ✔ AGPL 3 | ✔ | D
[Files](files-community.md) | File browser | Windows | free | ✔ | ✔ MIT | ✔
[TMSU](tmsu.md) | CLI utility | Linux | free | ✔ | ✔ GPL 3 | | | ✔
[Hyperplane](hyperplane.md) | File browser | Linux | free | ✔ | ✔ GPL 3
[Eagle](eagle.md) | File manager | Windows, macOS | paid + free trial | | | ✔

# Media

⌄Name\Features> | Type | Supported OS | Price | Account not required | Open-Source | Updates | Cross-platform | Portable
---|---|---|---|---|---|---|---|---
[digiKam](digikam.md) | Image manager | Windows, Linux, macOS | free | ✔ | ✔ GPL 2 | ✔ | D | ✔
[Aves](aves.md) | Media gallery | Android | free | ✔ | ✔ BSD-3-Clause | ✔ | | ✔
[Danbooru](danbooru.md) | Media board | Website | free | ✔ | ✔ FreeBSD License | ✔ | W
[HomeGallery](homegallery.md) | Media gallery | Windows, Linux, macOS, Website | free | ✔ | ✔ MIT | ✔ | D, W
[Hydrus](hydrus.md) | Media board | Windows, Linux, macOS | free | ✔ | ✔ WTFPL | ✔ | D
[QuoMediaView](quomediaview.md) | Media board | Windows, Linux, macOS, Android, Website, iOS | free | ✔ | ✔ AGPL 3 | | A, W | ✔
[Shimmie 2](shimmie.md) | Media board | Windows, Website | free | ✔ | ✔ GPL 2 | ✔ | W
[Pix](pix.md) | Image manager | Linux | free | ✔ | ✔ GPL 2 | ✔
[szurubooru](szurubooru.md) | Media board | Website | free | | ✔ GPL 3 | | W

# Text

⌄Name\Features> | Type | Supported OS | Price | Account not required | Open-Source | Updates | Cross-platform | Portable
---|---|---|---|---|---|---|---|---
[nb](nb.md) | Text writing and bookmark manager | Windows, Linux, macOS | free | ✔ | ✔ AGPL 3 | ✔ | D | ✔
[QOwnNotes](qownnotes.md) | Text writing manager | Windows, Linux, macOS | free | ✔ | ✔ GPL 2 | ✔ | D | ✔
[Logseq](logseq.md) | Text writing manager | Windows, Linux, macOS, Android, iOS | free | ✔ | ✔ AGPL 3 | ✔ | A
[Obsidian](obsidian.md) | Text writing manager | Windows, Linux, macOS, Android, iOS | free + paid | ✔ | | ✔ | A | ✔
[bibliothecula](bibliothecula.md) | Document organizer | Windows, Linux, macOS | free | ✔ | ✔ GPL 3 | | D, W
[Material Notes](material-notes.md) | Notes app | Android | free | ✔ | ✔ AGPL 3 | ✔
[Quillpad](quillpad.md) | Notes app | Android | free | ✔ | ✔ GPL 3 | ✔


# Bookmarks

⌄Name\Features> | Type | Supported OS | Price | Account not required | Open-Source | Updates | Cross-platform | Portable
---|---|---|---|---|---|---|---|---
[Firefox](firefox.md) | Browser + bookmark manager | Windows, Linux, macOS | free | ✔ | ✔ MPL 2.0 | ✔ | D | ✔
[nb](nb.md) | Text writing and bookmark manager | Windows, Linux, macOS | free | ✔ | ✔ AGPL 3 | ✔ | D | ✔
[Grimoire](grimoire.md) | Bookmark manager | Website | free | ✔ | ✔ MIT | ✔ | W
[Karakeep](karakeep.md) | Bookmark manager | Website, Android, iOS | free | ✔ | ✔ AGPL 3 | ✔ | W
[Omnivore](omnivore.md) | Read-it-later manager | Android, iOS | free | ✔ | ✔ AGPL 3 | ✔ | M
[Linkwarden](linkwarden.md) | Bookmark manager | Website | free + paid | | ✔ AGPL 3 | ✔ | W
[Raindrop.io](raindrop-io.md) | Bookmark manager | Windows, Linux, macOS, Android, iOS | free + paid | | ? | ✔ | A

# Games

⌄Name\Features> | Type | Supported OS | Price | Account not required | Open-Source | Updates | Cross-platform | Portable
---|---|---|---|---|---|---|---|---
[Heroic Games Launcher](heroicgameslauncher.md) | Gaming launcher | Windows, Linux, macOS | free | ✔ | ✔ GPL 3 | ✔ | D | ✔
[Playnite](playnite.md) | Gaming library + launcher | Windows | free | ✔ | ✔ MIT | ✔ | | ✔
[Steam](steam.md) | Gaming store + launcher | Windows, Linux, macOS | free | | | ✔ | D

# Other

⌄Name\Features> | Type | Supported OS | Price | Account not required | Open-Source | Updates | Cross-platform | Portable
---|---|---|---|---|---|---|---|---
[Kanri](kanri.md) | Project management board | Windows, macOS, Linux | free | ✔ | ✔ GPL 3 | ✔ | D | ✔
[Discourse](discourse.md) | Forum | Website | free + paid | ✔ | ✔ GPL 2 | ✔ | W
[GitLab](gitlab.md) | Git development platform | Website | free + paid | ✔ | ✔ MIT | ✔ | W
[Nemo Tags](nemo-tags.md) | Plugin for file browser | Linux | free | ✔ | ✔ GPL 3 | ✔
[Planify](planify.md) | To-do list | Linux | free | ✔ | ✔ GPL 3 | ✔
[friends](friends.md) | people relationship calendar/diary? | Linux? | free | ✔ | ✔ MIT
[GitHub](github.md) | Git development platform | Website | free + paid | | | ✔ | W
