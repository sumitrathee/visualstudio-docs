---
title: "Quickstart: Create a console app in Visual Studio with Visual Basic | Microsoft Docs"
ms.custom: ""
ms.date: "12/05/2017"
ms.reviewer: ""
ms.suite: ""
ms.technology:
  - "vs-acquisition"
ms.tgt_pltfrm: ""
ms.topic: "quickstart"
ms.devlang: "vb"
author: "TerryGLee"
ms.author: "tglee"
manager: ghogen
dev_langs:
  - vb
---
# Quickstart: Create a console app in Visual Studio with Visual Basic
In this 5-10 minute introduction to the Visual Studio integrated development environment (IDE), you'll create a simple Visual Basic application that runs on the console.

If you haven't already installed Visual Studio, go to the [Visual Studio Downloads](https://aka.ms/vsdownload?utm_source=mscom&utm_campaign=msdocs) page to install it for free.

## Create a project
First, you'll create a Visual Basic application project. The project type comes with all the template files you'll need, before you've even added anything!

1. Open Visual Studio 2017.

2. From the top menu bar, choose **File** > **New** > **Project...**.

3. In the **New Project** dialog box in the left pane, expand **Visual Basic**, and then choose **.NET Core**. In the middle pane, choose **Console App (.NET Core)**. Then name the project *HelloWorld*.

   ![.NET Core cross-platform development workload in the Visual Studio Installer](../ide/media/new-project-vb-dotnet-helloworld-console-app.png)

     If you don't see the **Console App (.NET Core)** project template, click the **Open Visual Studio Installer** link in the left pane of the **New Project** dialog box.

   ![Click the Open Visual Studio Installer link from the New Project dialog box](../ide/media/vb-open-visual-studio-installer.png)

     The Visual Studio Installer launches. Choose the **.NET Core cross-platform development** workload, and then choose **Modify**.

     ![.NET Core cross-platform development workload in the Visual Studio Installer](../ide/media/dot-net-core-xplat-dev-workload.png)

## Create the application
After you select your Visual Basic project template and name your project, Visual Studio creates a simple "Hello World" application for you. It calls the [Console.WriteLine(System.String)](https://docs.microsoft.com/en-us/dotnet/api/system.console.writeline?view=netframework-4.7.1#System_Console_WriteLine_System_String) method to display the literal string "Hello World!" in the console window.

![View the default Hello World code from the template](../ide/media/vb-console-helloworld-template.png)

If you click the **HelloWorld** button in the IDE, you can run the program in Debug mode.

  ![Click the Hello World button to run the program in Debug mode](../ide/media/vb-console-hello-world-button.png)

When you do this, the console window is visible for only a moment before it closes. This happens because the `Main` method terminates after its single statement executes, and so the application ends.

### Add some code
Let's add some code to pause the application and then ask for user input.

1. Add the following code immediately after the call to the [Console.WriteLine(System.String)](https://docs.microsoft.com/en-us/dotnet/api/system.console.writeline?view=netframework-4.7.1#System_Console_WriteLine_System_String) method:

   ```vb
   Console.Write("Press any key to continue...")
   Console.ReadKey(true)
   ```
   This pauses the program until you press a key.

2. On the menu bar, select **Build** > **Build Solution**.

   This compiles your program into an intermediate language (IL) that's converted into binary code by a just-in-time (JIT) compiler.

## Run the application
1. Click the **HelloWorld** button on the toolbar.

   ![Click the Hello World button to run the program from the toolbar](../ide/media/vb-console-hello-world-button.png)

2. Press any key to close the console window.

   ![Console window showing Hello World and Press any key to continue](../ide/media/vb-console-hello-world-press-any-key.png)

Congratulations on completing this quickstart! We hope you learned a little bit about Visual Basic and the Visual Studio IDE. If you'd like to delve deeper, please continue with a tutorial in the **Tutorials** section of the table of contents.

## See also
* [Quickstart: Create a "Hello World" Windows Forms app in Visual Studio with Visual Basic](quickstart-visual-basic-winforms.md)
* [Learn more about Visual Basic IntelliSense](visual-basic-specific-intellisense.md)
