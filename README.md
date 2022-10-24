# Seforim Finder ![Logo](https://raw.github.com/shmueldabomb441/SeforimCatalog/master/SeforimFinderWhiteAndAlpha.jpeg)


This is a fast, powerful, and beautiful (see screenshots below) program for searching a catalog of Hebrew books (seforim). It can search by exact match, malei/chaseir (plene/defective) insensitivity, and Shoresh (root word) search (good for finding a sefer with an approximate title, among other things). I would love to spread it to other yeshivos and libraries for free. if you would like to use it, please let me know so I can keep tabs on the user base. Feel free to create an issue [here](https://github.com/shmueldabomb441/YGW-Seforim-Catalog/issues/new/choose) if you need help setting it up. The code is available [here](https://github.com/shmueldabomb441/SeforimCatalog)

# Installation 
This repository contains files for setting up the seforim finder on a Windows computer. Instructions for setting it up on a macOS or Linux computer are virtually the same, but require me to create an additional file. Create an issue [here](https://github.com/shmueldabomb441/YGW-Seforim-Catalog/issues/new/choose) if you would like instructions for setting the program up on those platforms.

### Basic installation 
 1. Download the contents of this repository into a zip file by clicking [here](https://github.com/shmueldabomb441/YGW-Seforim-Catalog/archive/refs/heads/main.zip) (download will start automatically), and unzip/extract the zip file.
 2. Download the official Java program interpreter (which allows the program to run) by clicking [here](https://download.java.net/java/GA/jdk11/13/GPL/openjdk-11.0.1_windows-x64_bin.zip) (download will start automatically) and extract the zip file to the folder you extracted in the previous step, so that the folder with the name "jdk..." is in the same folder as the file "SeforimFinder.jar".
 3. Double-click the file named "SeforimFinder***Runner***.bat" (the file with a gear icon - the ".bat" part may not be visible) and the program should start up!

### Adding a taskbar shortcut

If you would like to add a shortcut to the taskbar at the bottom of the screen that can be clicked to run the program, follow the steps below. If you don't care about the icon in the taskbar displaying the seforim finder logo, skip step 4.

 1. Right-click on SeforimFinder***Runner***.bat (the file with a gear icon) and click "Create shortcut".
 2. Right-click the newly created file named "SeforimFinderRunner - Shortcut", and click on "Properties".
 3. In the text field with the label "Target:", replace the text with `%windir%\system32\cmd.exe /c start "" "%CD%\SeforimFinderRunner.bat"`. Click "Apply" to save the changes.
 4. Click "Change icon". In the popup, click "Browse..." and navigate to where you extracted this repository (the file you downloaded in step 1 of Basic Installation above). There is an icon in that folder with a magnifying glass on a book. Double-click that image to select it. Click "OK" to exit the icon picker popup window. Click "Apply" in the Properties windo to save the changes, and click "OK" to close the Properties window.
 5. Drag the shortcut file to the taskbar and the shortcut should appear. Click on the new shortcut and the program should start up!

## Why not just use an .exe file?
You may wonder why I don't package this as an exe file. There are several reasons:
    
 - Some antiviruses falsely flag Java programs packaged in an .exe file as a virus, so to make this as seamless of a process as possible, it is not packaged as an exe.
 - If an error occurs, the contents of the log need to be sent to me for me to fix the error, and using an exe would not allow seeing the logs.
 - Java programs get very big when packaged into an .exe, and GitHub does not allow hosting files bigger than 100 MB.
 - The program takes 10-15 seconds to start up, and I wouldn't want a user thinking that nothing happened while it was loading, so displaying the logs lets you know what is happening and how soon the program will finish setting up.
 - Packaging a Java program as an .exe can be quite complicated, and increases the number of moving parts that can be the cause of an issue should one come up. Leaving the program as a .jar file reduces these complications.

In short, it is to give you, the user, a better experience using the program - both when getting it up and running, as well as when reporting an issue (should one arise).

# License 
This software uses [HebMorph](https://github.com/synhershko/HebMorph) for the Shoresh search, which is licensed under the GNU Affero General Public License version 3.

# Screenshots

![Alt Text](https://raw.github.com/shmueldabomb441/SeforimCatalog/master/ScreenshotProgramFrontPage.png)
![Alt Text](https://raw.github.com/shmueldabomb441/SeforimCatalog/master/ScreenshotRootWordSearchOptions.png)
![Alt Text](https://raw.github.com/shmueldabomb441/SeforimCatalog/master/ScreenshotRootWordSearchExample.png)
![Alt Text](https://raw.github.com/shmueldabomb441/SeforimCatalog/master/ScreenshotMaleiChaseirInsensitive.png)
![Alt Text](https://raw.github.com/shmueldabomb441/SeforimCatalog/master/ScreenshotSeforimByCriteria.png)
![Alt Text](https://raw.github.com/shmueldabomb441/SeforimCatalog/master/ScreenshotAuthors.png)
![Alt Text](https://raw.github.com/shmueldabomb441/SeforimCatalog/master/ScreenshotCategories.png)
![Alt Text](https://raw.github.com/shmueldabomb441/SeforimCatalog/master/ScreenshotShelves.png)
![Alt Text](https://raw.github.com/shmueldabomb441/SeforimCatalog/master/ScreenshotTips.png)
![Alt Text](https://raw.github.com/shmueldabomb441/SeforimCatalog/master/ScreenshotHelp.png)
