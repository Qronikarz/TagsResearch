# Tags vs folders
## Problem: Organization of your digital collection.
Nowadays there is abundance of digital files of every possible type. Even after using various duplicate removing software there is too much to handle. So you look into possible solutions. 

How about sorting the files into folders? Time proven method, always was there and probably always will be there no matter how much time passes. So begins your adventure to sort your photographs into organized folders.

You decide to start with scenery. It goes easy, your photos from the trip to forest into the "forest" folder, clouds into the "sky" folder because they can only be in the sky and don't require their own folder. Problems start to appear when you notice the photos from your forest trip also have clouds on the sky. Not a big deal since they are not the main focus of the photos, but just with this you lose a possible search in the future. You can consider making a shortcut in the "sky" folder but then you have more files than you started with and you would need to create a new shortcut copy for every folder that you could categorize the photo with.

That's where tags come handy. If some photo has elements that would categorize it into few folders then you just apply the keywords to it and don't create any new files and folders therefore not adding to the problem of too much stuff on your memory. Say for example a photo of lake in the mountains next to some trees and a cloudy sky. Just with that description you could add 5 keywords that you could later use to search with.

## Problem: Folder support vs tags support
You can skip this section if you are macOS user.

Folders are used in every possible device available. No matter the OS, no matter the architecture you can expect the system to use folders. Not counting the problem of computer users just throwing everything into the desktop folder and still growing problem of smartphone users not even understanding that photos are actually stored in folders, the folders are always going to be available for you to use them.

Situation is sadly way, way worse when it comes to tags. On Windows, tags are hidden so much that casual users probably don't even know that it is possible to tag the files. And even if they do, the tags are fragile and don't survive copying to other file systems like for example to USB memories. macOS has allegedly the best implementation of tags when it comes to default file browsers. Unfortunately it is only available in Apple ecosystem so many people can't even check it themselves. When it comes to last major OS - Linux the support for tags is scarce. Only KDE and MATE desktops have file browsers that support file tags. All the other desktops no matter how big, don't use tags for files. 

That's one of the reasons this tag research was created. To list the file browsers and convince people of usefulnes of tagging files or other stuff. If more people get familiar with it, it may result in possibly some of them improving the file browsers with tag support. They can either develop it themselves or sponsor existing developers to add tags into the file browsers. When it comes to closed-source software it's also possible to give feedback to developers if a large enough group of people share their opinions.

## Problem: Custom solutions and lack of standards + AI rise
On nearly every device and system you are not confined to only using the default file browsers. You can mostly without problems install other programs that you can organize your files with. Then just use that program to manage your collection. Problems solved you can have your sweet tags and your digital storage is organized...

But problems appear again when for example:

1) the developer stops updating the program version for your OS of use and it has some bugs or security vulnerabilities for worse,

2) the developer doesn't make the program for newer version of your OS leaving you with nothing to use after upgrade, 

3) You want to share photos with your friends and they have vastly different operating systems,

4) You rename the file and it loses the tags? which means they were stored in some weird place, 

5) You move the files into another drive and all files lose the tags

6) You leave Windows for macOS and you must tag your files again

There are possibly even more problems that may arise, but it certainly shows that tags are very fragile system to use. One thing that may help here is some standardization of tags or even a shared developers effort without a given standard.

Let's take a look at the world of mp3 songs. Despite not having a standard most programs and developers settled on the same way to tag music files - ID3. This allowed for outstanding situation where even right now there are multitudes of programs that either show music tags in the player or allow you to tag music files either manually or automatically using some public database like for example MusicBrainz.

Of course, we can't have a public database for general files that users create themselves, but object detection in photos and AI based text summarizing are becoming increasingly popular so it is important to settle on some form of doing tags the same way across all modern programs. It would allow you to just run the auto tagging programs in the background and once they finish use the tags in every other program that supports them. It would also allow you to easily share files with tags between your own devices or to your friends.

# Worth checking for more

https://zapier.com/blog/how-to-use-tags-and-labels/ - Explanation about tags, tips for using them and a short collection of programs with tagging capability.

https://karl-voit.at/2019/11/26/Tagging-Files-With-Windows-10/ - A detailed guide describing how to use tags in Windows 10. Which file extensions are restricted from it and overall problems with Windows implementation.

https://barrowclift.me/post/tags-explained - Short and precise article about tags on macOS

https://community.kde.org/GSoc/2023/StatusReports/QuocHungTran - 2023 report of GSoc project about adding object detection based tagging support to digiKam 8.3.0

https://www.youtube.com/watch?v=wTQeMkYRMcw - Short tag explanation in video format and a report on Work-In-Progress file manager with advanced tag capabilities