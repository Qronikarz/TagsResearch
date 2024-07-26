# Tags research
Knowledge base originally made for improving QuoMediaView, rewritten for public access. New goals are to provide useful information for developers able to implement tags and establish a new standard/specification that allows for file tagging on every major platform (or at least unify the Linux ones).

> [!NOTE]
> Looking for someone to pass this project to. It was used as listed above and I want it to become a general documentation that somebody more talented oversees. I'm happy just to provide info and this was currently the best form possible to do. Someone else may make it into GitBook documentation or a website that shares the same goal, but is presented visually better along with program screenshots and translations.

# Resources
[Tags Overview](components/tagsoverview.md) - markdown file with an explanation of tagging systems in comparison with traditional folder based approach. Best for beginners.

[Tags Research](components/tagsresearch.md) - markdown file with a collection of links and notes about general file tagging and all specification attempts from the past. More tailored for developers or users that are already using file tags.

# Explanations

[Glossary](components/glossary.md) - markdown file with descriptions of features featured on single program pages. Due to some of them being harder to explain and being used in every page it needed to be made into separate file for easy access and deduplication.

**OS default file browsers** are listed even if they do not support tagging files. They have less features in their table because each of them is nearly identical with each other - type, free price/included, constant updates, lack of cross-platform, UI type.

Software listed in "**other software**" table needs to have some sort of tagging feature. It must allow user to choose a name for the tag and search for items using it. Viewing an item should show the tags that it has. 

Every added and listed program must have a link to more detailed description in their own .md file in components folder. The markdown table only has place for few most important features, but the programs have various tagging capabilities.

**Supported OS** - Operating System that specific software works on. Software may have a version for other platform, but only versions with tags are to be listed (in case of Steam, you can't view collections on Android). Web in OS means you can put the software on some server and access it through a website with a browser.

**updates** - updated at least once a year with either new features or bugfixes (documentation/readmes do not count)

**cross-platform** - It must work between three big platforms - Windows, Linux and macOS. 

**portable** - Ability to run software from other disks or USB devices. Does not need cross-platform support.

**UI type** - The interface that tagging uses - either GUI, CLI or in some cases both.

# OS Default file browsers

⌄name\features> | OS/DE/Brand | tags/key words | open-source | tag specification | cross-platform
---|---|---|---|---|---
[File Explorer](components/file-explorer.md) | Windows | ✔ not every file type
[Finder](components/finder.md) | macOS | ✔
[Dolphin](components/dolphin.md) | Linux/KDE Plasma | ✔ | ✔ GPL 2 | ✔ user.xdg.tags
[Caja](components/caja.md) | Linux/MATE | ✔ | ✔ GPL 2 | ✔ user.xdg.tags
[Index](components/index.md) | Linux/MauiKit | ✔ | ✔ LGPL 3
[Files](components/ios-files.md) | iOS | ✔
[Files](components/ipados-files.md) | iPadOS | ✔
[Nemo](components/nemo.md) | Linux/Cinnamon | | ✔ GPL 2
[cosmic-files](components/cosmic-files.md) | Linux/COSMIC | | ✔ GPL 3
[Thunar](components/thunar.md) | Linux/Xfce | | ✔ GPL 2
[Nautilus](components/nautilus.md) | Linux/GNOME | | ✔ GPL 3
[Files](components/chromeos-files.md) | ChromeOS
[Files by Google](components/files-by-google.md) | Android/Google
[Files](components/lineageos-files.md) | Android/LineageOS | | ✔ Apache 2.0
[Samsung My Files](components/samsung-my-files.md) | Android/Samsung
[Mi File Manager](components/mi-file-manager.md) | Android/Xiaomi

# Other software

⌄name\features> | Type | Supported OS |  price | open-source | updates | cross-platform | portable | UI type
---|---|---|---|---|---|---|---|---
[QuoMediaView](components/quomediaview.md) | Media board | Windows, Linux, macOS, Android, Web | free | ✔ AGPL 3 | ✔ | ✔ | ✔ | GUI | ✔
[Danbooru](components/danbooru.md) | Media board | Web | free | ✔ FreeBSD License | ✔ | | | GUI
[TMSU](components/tmsu.md) | CLI utility | Linux | free | ✔ GPL 3  | | | ✔ | CLI
[szurubooru](components/szurubooru.md) | Media board | Web | free | ✔ GPL 3 | | | | GUI
[Hydrus](components/hydrus.md) | Media board | Windows, Linux, macOS | free | ✔ WTFPL | ✔ | ✔ | | GUI
[Firefox](components/firefox.md) | Browser + bookmark manager | Windows, Linux, macOS | free | ✔ MPL 2.0 | ✔ | ✔ | ✔ | GUI
[Discourse](components/discourse.md) | Forum | Web | free + paid | ✔ GPL 2 | ✔ | | | GUI
[Steam](components/steam.md) | Gaming store + launcher | Windows, Linux, macOS | free | | ✔ | ✔ | | GUI
[TagSpaces](components/tagspaces.md) | File manager | Windows, Linux, macOS, Android, Web | free + paid | ✔ AGPL 3 | ✔ | ✔ | ✔ | GUI
[Pix](components/pix.md) | Image manager | Linux | free | ✔ GPL 2 | ✔ | | | GUI
[HomeGallery](components/homegallery.md) | Media gallery | Windows, Linux, macOS, Web | free | ✔ MIT | ✔ | ✔ | | GUI
[Playnite](components/playnite.md) | Gaming library + launcher | Windows | free | ✔ MIT | ✔ | | ✔ | GUI
[Heroic Games Launcher](components/heroicgameslauncher.md) | Gaming launcher | Windows, Linux, macOS | free | ✔ GPL 3 | ✔ | ✔ | | GUI
[Obsidian](components/obsidian.md) | Text writing manager | Windows, Linux, macOS, Android, iOS | free + paid | | ✔ | ✔ | ✔ | GUI
[digiKam](components/digikam.md) | Image manager | Windows, Linux, macOS | free | ✔ GPL 2 | ✔ | ✔ | | GUI
[Shimmie 2](components/shimmie.md) | Media board | Windows, Web | free | ✔ GPL 2 | ✔ | | | GUI
[Eagle](components/eagle.md) | File manager | Windows, macOS | paid + free trial | | ✔ | | | GUI
[TagStudio](components/tagstudio.md) | File manager | Windows, Linux, macOS | free | ✔ GPL 3 | ✔ | ✔ | ✔ | GUI
[Spacedrive](components/spacedrive.md) | File browser | Windows, Linux, macOS | free | ✔ AGPL 3 | ✔ | ✔ | | GUI
[Logseq](components/logseq.md) | Text writing manager | Windows, Linux, macOS, Android, iOS | free | ✔ AGPL 3 | ✔ | ✔ | | GUI
[Omnivore](components/omnivore.md) | Read-it-later manager | Web, Android, iOS | free | ✔ AGPL 3 | ✔ | | | GUI
[nb](components/nb.md) | Text writing and bookmark manager | Windows, Linux, macOS | free | ✔ AGPL 3 | ✔ | ✔ | ✔ | CLI
[filetags](components/filetags.md) | File name modification management | Windows, Linux, macOS | free | ✔ GPL 3 | ✔ | ✔ | ✔ | CLI
[Hoarder](components/hoarder.md) | Bookmark manager | Web, Android, iOS | free | ✔ AGPL 3 | ✔ | | | GUI
[Grimoire](components/grimoire.md) | Bookmark manager | Web? | free | ✔ MIT | ✔ | | | GUI
[Linkwarden](components/linkwarden.md) | Bookmark manager | Web | free + paid | ✔ AGPL 3 | ✔ | | | GUI
[Raindrop.io](components/raindrop-io.md) | Bookmark manager | Windows, Linux, macOS, Web, Android, iOS | free + paid | ? | ✔ | ✔ | | GUI
[bibliothecula](components/bibliothecula.md) | Document organizer | Windows, Linux, macOS | free | ✔ GPL 3 | | ✔ | | GUI, CLI
[Hyperplane](components/hyperplane.md) | File browser | Linux | free | ✔ GPL 3 | ✔ | | | GUI
[friends](components/friends.md) | people relationship calendar/diary? | Linux? | free | ✔ MIT | | | | CLI
[Planify](components/friends.md) | To-do list | Linux | free | ✔ GPL 3 | ✔ | | | GUI
[QOwnNotes](components/qownnotes.md) | Text writing manager | Windows, Linux, macOS | free | ✔ GPL 2 | ✔ | ✔ | ✔ | GUI
[Files](components/files-community.md) | File browser | Windows | free | ✔ MIT | ✔ | | | GUI
[GitHub](components/github.md) | Git development platform | Web | free + paid | | ✔ | | | GUI
[GitLab](components/gitlab.md) | Git development platform | Web | free + paid | ✔ MIT | ✔ | | | GUI

# Contributors list
Qronikarz(GitHub), 

# Fully completed files:
Research: [Tags Overview](components/tagsoverview.md), [Tags Research](components/tagsresearch.md), [Glossary](components/glossary.md), [Program Template](components/programtemplate.md)

Programs: [QuoMediaView](components/quomediaview.md),

# License
CC-BY-SA-4.0

If there's a better license feel free to suggest it. Main goal was to have it available for copying and using it in other projects - like for example if somebody wants to convert it into something like Gitbook documentation then there should be no problems.

# File info
Last updated | 2024-07-26

Number of programs in database | 51
