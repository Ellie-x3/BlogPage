+++
title = 'Pixel Platformer Part 1'
date = 2024-03-14T21:59:13-03:00
draft = false
description = "We will go through and install monogame and create our first window!"
image = "/images/MG.webp"
imageBig = ""
categories = ["MonoGame", "CSharp", "PixelPlatformer"]
authors = ["Ellie"]
+++


# MonoGame Setup

First we will need to go through the installation steps for [**MonoGame**](https://monogame.net/) Steps: [Here](https://monogame.net/articles/getting_started/index.html)

This Guide will be for MonoGame on Windows but there is steps in the documentation for other platforms.
I will quickly go through the steps but I highly encourage going through the documentation yourself aswell.

First we will install [Visual Studio](https://visualstudio.microsoft.com/vs/) - This will help speed up the install process

When installing make sure to select the correct .NET options


![alt text](https://monogame.net/articles/getting_started/images/1_installer_vs_components.png "Install selections")

Once Visual Studio is installed we will install the monogame templates.

1. Launch VS 2022
2. Select the "Continue Without Code" option
3. At the top of your screen select "extensions" tab and then "Manage Extensions"
4. In the search box search for "MonoGame" and install the c# project templates

You may be prompted to install it and close VS 2022 to proceed.

This will allow us to now use Visual Studio to create our game by selecting the template

![alt text](https://monogame.net/articles/getting_started/images/vswin_mg_new_2.png "Template")

## **OTHER DEV ENVIRONMENTS**

If you prefer using Jetbrains Rider or Visual Studio Code (Like Myself) we will need to install the .NET SDK
[Here](https://dotnet.microsoft.com/en-us/download/dotnet/8.0)

Download the latest SDK for your operating system to continue

Once installed you should now have a new command tool. Run the following commands in your command prompt: 

```cs
    dotnet --version
```

Note you may need to close and re-open command prompt if previously opened.

Now that you have dotnet installed. You can create a project with the following:

```cs
    dotnet new --install MonoGame.Templates.CSharp
    dotnet new mgdesktopgl -o PixelPlatformer
```

Where -o is the project directory it will create.

# Project has beed made
Now that you successfully created your project with either VS 2022 Tempplates or via dotnet we will check out the code.

Firstly the files it created: Most of these we can ignore for now

![alt text](filesystem)
[filesystem]: D:/blog/quickstart/static/images/pp1/filesystem.png "fs"