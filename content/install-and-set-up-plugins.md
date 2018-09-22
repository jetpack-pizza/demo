# Installing and configuring plugins
To start building your application with Flutter using IntelliJ IDEA, you must install both Flutter and Dart plugins. The Flutter plugin is responsible for hot reload, running, debugging, and other developer workflows, while the Dart plugin carries out code analysis features like code completion and validation. These plugins work in conjunction.

## Install plugins
1. Press ``Ctrl+Alt+S`` (Win, Linux) or ``⌘,`` (Mac OS) to open the **Settings/Preferences** dialog and go to **Plugins**.
2. Click the **Browse repositories** button at the bottom of the window to view the list of available plugins.
3. Find the Flutter plugin using the search field and click **Install** on the right side of the window.
4. Click **Yes** when/if IntelliJ IDEA suggests installing the Dart plugin.
5. Close the **Settings/Preferences** dialog by clicking **OK**.
6. Restart IntelliJ IDEA for the changes to take effect.

## Configure plugins
Once you have installed the plugins, you must specify proper SDK paths.

### Specify the Flutter SDK path
1. Open the **Settings/Preferences** dialog and go to **Languages & Frameworks | Flutter**.
2. Specify the Flutter SDK path in the field at the top of the window. Once it is done, the current version is displayed.
<p align="center">
<img src="https://github.com/jetpack-pizza/demo/blob/master/img/1_flutter_sdk_path.png" alt="Flutter SDK" width="700"/>
</p>

3. Click **OK**.

### Specify the Dart SDK path
1. Open the **Settings/Preferences** dialog and go to **Languages & Frameworks | Dart**.
2. Specify the Dart SDK path in the field at the top of the window. Note that this path is actually inside of your Flutter SDK directory. For instance, if the Flutter SDK location is ``\src\flutter-sdk\flutter``, the Dart SDK location will be ``\src\flutter-sdk\flutter\bin\cache\dart-sdk``. Once the path is specified, the current version is displayed.
<p align="center">
<img src="https://github.com/jetpack-pizza/demo/blob/master/img/1_dart_sdk_path.png" alt="Dart SDK" width="700"/>
</p>

3. Click **OK**.

## Additional configuration
Now you can start working on your Flutter projects in IntelliJ IDEA. To configure additional Flutter- and Dart-specific settings, such as color schemes or live templates, open and explore the **Settings/Preferences** dialog.
<p align="center">
<img src="https://github.com/jetpack-pizza/demo/blob/master/img/1_settings.png" alt="Settings" width="700"/>
</p>

### Set up the Flutter plugin
IntelliJ IDEA allows you to customize your Flutter environment. For example, you can enable the **Hot Reload** performing or formatting code (running the ``dartfmt`` command) on save, enable verbose logging, etc. To view these settings, open the **Settings/Preferences** dialog and go to **Languages & Frameworks | Flutter**.
<p align="center">
<img src="https://github.com/jetpack-pizza/demo/blob/master/img/1_settings_flutter.png" alt="Flutter Settings" width="700"/>
</p>

### Set up the Dart plugin
To modify the Dart code style according to your needs, open the **Settings/Preferences** dialog and go to **Editor | Code Style | Dart**.
<p align="center">
<img src="https://github.com/jetpack-pizza/demo/blob/master/img/1_settings_dart.png" alt="Dart Settings" width="700"/>
</p>

### Shortcuts
Shortcuts allow to save time, so explore the **Keymap** (**Settings/Preferences dialog | Keymap**) once you have installed the new plugins. 

### Color schemes
You can modify color schemes if needed (**Settings/Preferences dialog | Editor | Color Scheme**).

---

**Next:** While working on your Flutter application you will interact with [tool windows](https://github.com/jetpack-pizza/demo/blob/master/content/tool-windows.md). Some of them are standard for IntelliJ IDEA, but there are new tool windows that have been designed specifically for the Flutter and Dart plugins.
