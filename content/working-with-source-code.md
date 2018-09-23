# Working with source code
You can use standard features of IntelliJ IDEA while working on Flutter projects. In addition, the Dart and Flutter plugins work in conjunction to perform language and SDK-specific tasks, from code completion to hot reload. IntelliJ IDEA offers tools that have been designed specifically for working on Dart and Flutter code.

## Use the Flutter Outline
Widgets are the core building blocks in Flutter applications (everything-is-a-widget concept), so a tool for managing widgets and ensuring the structure correctness has been created. Click **Flutter Outline** on the right side of the main IDE window (alternatively, choose **View | Tool Windows | Flutter Outline** on the main menu) to open the **Flutter Outline** and manage your widgets. The **Flutter Outline** allows you to center widgets, add padding, wrap widgets with columns and rows, extract methods, move widgets up and down, and remove them. To perform the required action, click the corresponding button on the toolbar:
<p align="center">
<img src="https://github.com/jetpack-pizza/demo/blob/master/img/4_flutter_outline_toolbar.png" alt="Flutter Outline Toolbar" 
width="590"/>
</p>

**Flutter Outline** permits to view the structure of your application and modify it. When you use this tool, the IDE makes sure that the structure is correct, so you can avoid typos or omitted symbols. For instance, you can center a widget by using the **Flutter Outline** tool: 
1. Select a widget.
2. Click the **Center widget** button on the toolbar. Note that if an action cannot be executed, the corresponding button is greyed out.
3. Perform **Hot Reload** to see the changes.

<img src="https://github.com/jetpack-pizza/demo/blob/master/img/4_center_widget.gif" alt="" width=""/>|
<img src="https://github.com/jetpack-pizza/demo/blob/master/img/4_center_widget_demo.gif" alt="" width="340"/>|
--- | --- |

>**Note:** Click the <img src="https://github.com/jetpack-pizza/demo/blob/master/img/4_filter.png" alt="Filter" width="16"/> 
icon in the upper-right corner of the **Flutter Outline** tool window to enable filtering and display only widgets.

## Use the Structure tool window
Another way to look at the structure of your project is to use the **Structure** tool window. To open it, click **Structure** on the left side of the main IDE window (alternatively, choose **View | Tool Windows | Structure** on the main menu). When you select a widget in the **Structure View**, the **Editor** jumps to the corresponding line in your code.
<p align="center">
<img src="https://github.com/jetpack-pizza/demo/blob/master/img/4_structure_view.png" alt="Structure View" width="850"/>
</p>

## Manage widgets
IntelliJ IDEA offers alternative widgets management functionalities: you can add padding, remove a widget, swap it with its parent, wrap it with a new widget by using the ``Alt+Enter`` (Win, Linux) or ``⌘↩`` (Mac OS) shortcuts in the **Editor**. This method helps to save time and makes sure that the project structure remains valid. For instance, you can center a widget by using the **Center widget** option:
<p align="center">
<img src="https://github.com/jetpack-pizza/demo/blob/master/img/4_center_widget_2.png" alt="Center Widget" width="400"/>
</p>

Alternatively, you can select the **Wrap with new widget** option, which allows you to implement any valid widget. In this example, it is possible to use the same ``Center`` widget:
<p align="center">
<img src="https://github.com/jetpack-pizza/demo/blob/master/img/4_wrap_widget.gif" alt="Wrap With New Widget" width="500"/>
</p>

## Convert components
If you need to convert ``child`` to ``children``, use the ``Alt+Enter`` (Win, Linux) or ``⌘↩`` (Mac OS) shortcuts to open the menu and choose the **Convert to children** option.
<p align="center">
<img src="https://github.com/jetpack-pizza/demo/blob/master/img/4_convert.png" alt="Convert" width="500"/>
</p>

## Use live templates 
IntelliJ offers several Flutter live templates that simplify adding new widgets to your project. For instance, it speeds up creating **Stateless** (``stless``), **Stateful** (``stful``), **Stateful with AnimationController** (``stanim``), and **Inherited** (``inh``) widgets. To view the templates available out of the box, open the **Settings/Preferences** dialog and go to **Editor | Live Templates**. Expand the **Flutter** or **Dart** sections to see the samples and modify them.
<p align="center">
<img src="https://github.com/jetpack-pizza/demo/blob/master/img/4_live_template.gif" alt="Flutter Live Template" width="400"/>
</p>

## Hot reload an app
**Hot reload** is a feature that injects updated source code files into the running VM (or a connected device). To initiate hot reload click the <img src="https://github.com/jetpack-pizza/demo/blob/master/img/4_hot_reload.png" alt="Hot Reload" width="16"/> icon (or use the ``Ctrl+Back Slash`` (Win, Linux) or ``⌘\`` (Mac OS) shortcut) in the upper-right corner of the main IDE window (you can also find this icon in the **Run** tool window). Alternatively, press ``Ctrl+S`` (``⌘S``) to **Save All** changes, which results in displaying the latest changes as well. 
> Note: The first loading on a physical device can take some time.

## Reformat the code
You can reformat the code to make sure that the proper Dart style is used. To do so, use the **dartfmt** command: use the **Find Action dialog** (use the ``Ctrl+Shift+A`` (Win, Linux) or ``⌘⇧A`` (Mac OS) shortcut) or choose the **Reformat Code with dartfmt** option from the right-click menu.
<p align="center">
<img src="https://github.com/jetpack-pizza/demo/blob/master/img/4_dartfmt.png" alt="Reformat Code with dartfmt" width="500"/>
</p>

## Add trailing commas
If your code includes multiple tree-shaped blocks, you can use trailing commas to help the formatter implement the proper number of line breaks for the Flutter code. To keep the format, add trailing commas at the end of parameter lists.

## Open a module in another IDE
It is possible to open a module and modify its code in another IDE. To do so, find the ``android`` folder in your **Project** tool window, right-click it, and choose **Flutter | Open Android module in Android Studio** (the similar feature is available for the Xcode SDK as well).

## System comments
Curly brackets can be divided by many lines of code in your app. IntelliJ IDEA displays special comments denoting classes and widgets which facilitate determining the beginning and ending of a specific invocation.
<p align="center">
<img src="https://github.com/jetpack-pizza/demo/blob/master/img/4_comments.png" alt="System Comments" width="500"/>
</p>

## Run Flutter commands
To invoke Flutter commands, click the required action at the top of the ``pubspec.yaml`` window. You can install referenced packages (the ``Packages get`` command), upgrade them to the latest version (the ``Packages upgrade`` command), upgrade the Flutter framework itself (the ``Flutter upgrade`` command), or validate the installed tools and check their versions (the ``Flutter doctor`` command).
<p align="center">
<img src="https://github.com/jetpack-pizza/demo/blob/master/img/4_packages_get.png" alt="Packages get" width="800"/>
</p>

## Add packages
You can use open-source packages in your projects. When you add a package name into the dependencies list (``pubspec.yaml``), click **Packages get** at the top of the window to pull the package into the project. The console should display the output of the following kind:
```
Running "flutter packages get" in demo_project... 
Process finished with exit code 0
```

## Import libraries
In case the Dart library required in your project has not been imported, press ``Alt+Enter`` (Win, Linux) or ``⌘↩`` (Mac OS) and select the library you need.
<p align="center">
<img src="https://github.com/jetpack-pizza/demo/blob/master/img/4_import_library.png" alt="Import Library" width="500"/>
</p>

## Use postfix completion templates
The Dart plugin comes with a number of postfix completion templates. To see them, open the **Settings/Preferences** dialog and go to **Editor | General | Postfix Completion**.  
<p align="center">
<img src="https://github.com/jetpack-pizza/demo/blob/master/img/4_postfix_completion.png" alt="Postfix Completion" width="700"/>
</p>

---

**Next:** IntelliJ IDEA offers several modes for [running applications](https://github.com/jetpack-pizza/demo/blob/master/content/running-applications.md).
