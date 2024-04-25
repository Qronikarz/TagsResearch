# Windows and the meh file tagging
There should be no surprise that even though Windows supported tags for quite some time on the NTFS, most users don't actually use them or even heard about the possibility to use file tagging. Not only file tagging is not visible enough it is also restricted to unknown number of file types so you can't use tags for each of your files.

To make the matters even worse, file tags are considered to not be persistent during the transfer or other operations on files. File tags in NTFS are stored on Alternate Data Streams and not every file handling method respects those. Copying the tagged files to another file system generally gets rid of the tags. So if you for example have USB memory stick with FAT32 and you copy tagged file from NTFS the tags are gone.

The new Work-In-Progress file system of Microsoft Windows (ReFS) does not implement Extended Attributes, but it later got Alternate Data Streams support so there is no certainty if has support for file tagging or not.

Other note worthy thing is that changing the file tags actually changes the file hash sums. It may break some things due to that behavior.

# Golden apples ecosystem
[Need fact checking and some more details from actual users of macOS and iOS - paragraph written based on few articles]

According to many articles the file tags on Apple ecosystem are a superior form. Interoperability between computer and mobile, easily discoverable tags with coloring support and widely used by programs.

Tags in macOS are supposedly stored both in separate place on HFS+ file system in .DS_Store file and as Extended Attributes in the actual files.

Problems start when you do start leaving the ecosystem in any way - transferring the files to your non-Apple devices will most certainly get rid of the tags and you won't have the same features anyway. Sharing files with your friends/peers who don't have any Apple devices will get them a lacking experience.

# Linux specifications
Linux world is vast with many often clashing visions and a lot of distributions, but at the core it's still the same OS and often the file systems are the same. Despite the problems, there are actually few things that majority of developers agree on.

Freedesktop is a project focused on providing specifications which Linux distributions can follow for better cross platformness. The most famous example probably being XDG user directories. Freedesktop actually had some work on file tagging, but it never got finished and it seems forgotten nowadays.

One thing that currently works are Common Extended Attributes - https://www.freedesktop.org/wiki/CommonExtendedAttributes/
It's a specification that many distributions adhere to, but it currently misses tags.
Extended Attributes work on all major Linux file systems sp there should be no obstacles at that front.

https://www.freedesktop.org/wiki/Specifications/shared-filemetadata-spec/ - The specification that was in works and had keywords support for generic files, audio, documents and images. There was no activity since 2013 looking at the last edited date. Some Linux Desktop Environments actually started using the user.xdg.tags for storing the file tags. KDE's Dolphin and MATE's Caja both share the same way so theoretically there should be no problems transferring files between them and still having the access to the tags in the files. However there are cases when Extended Attributes are lost during transfer or other operations on the files.

There are few Linux commands that don't preserve Extended Attributes, some that do and some that also do, but require special flags for it to keep them. Highly recommended checking the ArchWiki further below for more info about commands and their flags, and interoperability between file systems even including the Windows NTFS.

https://github.com/welbornprod/filetags - Linux command for editing the extended attributes - "user.xdg.tags" and "user.xdg.comment" on files.

# Cross platformness
Now having the 3 major OS platforms looked at, there is one problem. Even if we have one OS that does the file tagging with no complaints what if you decide to migrate to another OS, or what if you own few devices and want to copy the files and keep using the tags for easier search/work.

There are 2 possible solutions for that.

1st: use a cross-platform software to manage the files. This however locks you to use only one vendor on all your devices. Good example of that is Photoshop still being recommended as the only program for photo editing even though there are now wonderful alternatives. Even if the software is available for other device then you still are at mercy of the developer to not break your workflow in future updates.

2nd: Settle on one common format to embed tags in files. Massively hard to accomplish task. Probably even impossible when it comes to actually implementing it in all major Operating Systems. Though there is one example where the collaboration actually succeeded. 

# mp3 Utopia
World of mp3 files and the software for tagging them is truly wonderful example of how using a one way to do things can lead to great results. It may not be considered modern or the best practice by few, but mp3 files and it's tags are usually considered a solved issue.

There is a rich ecosystem of software that is centered around playing the music with tags support, programs that allow you to easily edit the tags yourself or automatically tag them with appropriate tags based either on the file name alone or song detection through something like Shazam. 

Mp3 perfect world is vast and would require it's own case study to actually provide useful info for generic file tagging which would exceed the scope of tag research. What matters is that mp3 with their few ways to store tags is great for cross platformness and is a great goal even though it may be hard to recreate.

The most popular tag formats in mp3 are ID3 and APE.

# Auto tagging in other areas
As before said, mp3 auto tagging is already in great shape. It can connect to music databases and automatically apply all relevant tags like the author, band, title, year, CD track and many more. You can't do that with generic files since there is no database for all files that were ever created. But thanks to object detection and text processing we can use generic tags to describe photos, videos or text and apply them to the files.

It's not a new concept. Image detection was researched and developed since as early as 1960s. It wasn't very easy though and required performance that not many computers were capable of yet.

Picasa was one of the first programs that allowed facial recognition for normal users. It was offered since 2008 and allowed to apply tags based on what was detected.

Another big example of image recognition offered to normal users is Facebook and it's use of automatic alt text on uploaded images (based on article date since 2016). It was not able to run it locally and offline, but it allowed for great results back then. Images were applied with a description such as "Image may contain: two people, smiling, sunglasses, outdoor". It was a big win for accessibility such as with visually impaired people, but it was also useful for users with slower connections or browsers with no image support, but as already said to use it you had to upload every image to Facebook and there was no easy way to later use it on your actual files. Years later the automatic alt text got supercharged with AI capabilities.

After the AI boom of 2022 we're currently in era where whole images can be created with text prompts which also use keywords to describe the photos. Various text processing models are capable of reading through thousands of lines and provide a quick summary which could also be used to automatically create tags to describe local text files and later easily search them. If there was one standard or even few of them which majority of file managers and other programs supported there would be no need to manage the files by your own in folders. Just throw all files into one folder, run auto tagging software and wait for it to complete to have it sorted and available for use.

# "Virtual" tag systems
Some tagging solutions require you to make a copy of the files in their preferred location to use the program sometimes even in a matter of uploading it and converting to supported file format. On the one hand it's great because they can also implement image duplication code to check if you already have the file in your folder, but on the other hand it increases the size that data on your disk occupies due to making a duplicate on its own, but also in some cases restricting you to only use that program to access the file from now on.

Other case is with TagSpaces - it stores tags inside the file name. Which has the advantage of not making a duplicate file, but has the restrictions of file system which means there are some characters that can't be used and you're limited with filename length which can be an issue if you start applying 50+ tags to one file. But it does offer an alternative solution to this approach.

Sidecar files allow to store information about the file without changing anything about the actual file. TagSpaces also offers this approach for people who don't want to rename their files. Sidecar files can be either created for all files or there can be one big side car file in some location that keeps track of every file.

Another solution that is kind of similar to sidecar files, but deserves it's own category are virtual file systems. If the file system that you use doesn't support tags or does it in horrible way, just add a new file system on top of it and enjoy the features. TMSU is such a virtual file system that doesn't alter any of your files and allows you to create a database that can be used on top of your own file system. Or it can be used to create few databases on top of your own file system. It's virtual and doesn't depend on the files so the only size limit are the tags itself and they can only be simple texts. Another program that allows the same approach is QuoMediaView. This time however it's GUI based and requires you to add files manually as there is no support for scanning the files with browser's JavaScript. But you can create few instances of this database and backup the tags themselves so they are not lost even if something happens to them. Naturally this means that if you do change the actual file the tags are lost in some way - they still exist but are now unmatched from file and you need to edit the file location so the program can see the file again.

# Backing up tags
With files the backup is straightforward. Make a copy of the file on some other disk and you're done. However when it comes to tags the situation is complicated once again. Even on one platform that supports tags some backup methods may discard file tags - just like on Linux when you don't use certain flags while copying or on Windows where for some reason some programs don't backup the file Alternate Data Streams and in the result get rid of your tags.

That's why it's important that the program or file browser is aware of how tags are stored and offers some way to backup the tags themselves which could later be imported or even applied to files manually.

On macOS it's supposedly possible to do script export of tags to some spreadsheet format according to this question: https://discussions.apple.com/thread/253998483?sortBy=best

On Linux the file browsers that support "xdg.user.space" store tags as a CSV format which means they can be easily backuped to text files using terminal and redirection operators.

Other programs may offer their own solution to backing the tags themselves. Like before said with QuoMediaView there is a button that exports the whole database for you in JSON format for you to store wherever you want as a backup.

# Tags management
Once you get used to tags all the tags you use may start to grow. And grow. And keep growing. Let's consider 1000 tags as a common result which may grow even larger. If there's at least a place/window where all tags are listed you can take a look at what tags have you been using, but there are still problems with organizing this new database that you've created.

What if you made a typo in the tag? What if due to slightly different spelling you have essentially 2 the same tags but applied to different files? What if you want to use synonyms for some words? What if you want to search for "water" but your file is only tagged with "lake"?

Tags come with their own fair share of problems. It can be challenging to manage all the tags you've started to create. That's why it would be good if the programs offered some deduplication based on naming or spelling correction so there are no typos. If the tags are stored only in your files then you would need to manually rename them whenever such situation arises. Tags should also be able to have relations to other tags - exactly like in languages we can have different ways to name the same thing we should be able to do the same with tags. If some tag belongs to wider tag just like with water/lake example you shouldn't need to tag files with all your tags but the ones that match the most. More talented developers may implement a mind map of tags and how they relate to each other so you can instantly see visually which tags are the most popular in your collection.

# Worth checking for more
https://karl-voit.at/2019/11/26/Tagging-Files-With-Windows-10/ - A detailed guide describing how to use tags in Windows 10. Which file extensions are restricted from it and overall problems with Windows implementation.

https://www.reddit.com/r/linuxquestions/comments/sl7xfd/is_there_a_tag_based_file_manager/ - Reddit post looking for tag based linux file manager. Explanations in comments and few program suggestions.

https://www.reddit.com/r/datacurator/comments/nm4gax/looking_for_file_manager_with_tags/ - Another Reddit post, this time for windows file manager with tags.

https://en.wikipedia.org/wiki/Image_organizer - List of programs for managing images. Not all of them support tagging.

https://en.wikipedia.org/wiki/Tag_editor - List of tag programs with tagging support for managing audio, images or videos.

https://wiki.archlinux.org/title/Extended_attributes - ArchWiki article for Extended Attributes. Lists programs with and without support, short overview, file system support for extended attributes and a mention of user.xdg.tags for storing tags

https://musicbrainz.org/doc/About - Community-maintained open source encyclopedia of music information.

https://picard-docs.musicbrainz.org/en/about_picard/introduction.html - Documentation of MusicBrainz Picard with various tagging methods listed for easy overview.

https://engineering.fb.com/2016/04/04/ios/under-the-hood-building-accessibility-tools-for-the-visually-impaired-on-facebook/ - Facebook article about their automatic image alt text

https://community.kde.org/GSoc/2023/StatusReports/QuocHungTran - 2023 report of GSoc project about adding object detection based tagging support to digiKam 8.3.0

https://hydrusnetwork.github.io/hydrus/advanced_siblings.html - Documentation for Hydrus program about tag relations and what happens when your tag database grows to massive sizes.

https://github.com/microsoft/VoTT - Visual Object Tagging Tool: An electron app for building end to end Object Detection Models from Images and Videos.

https://www.youtube.com/watch?v=wTQeMkYRMcw - Tags explanation and a concept of advanced tagging feature

https://news.ycombinator.com/item?id=33248391 - 250+ comments detailed discussion about tagging systems, problems and avantages

https://recognize-anything.github.io/ - open-source image recognition models that can be included into programs
