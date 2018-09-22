# Testing and debugging
A number of testing and debugging tools have been designed specifically for Dart and Flutter. Some of them run in background, like the **Dart Analyzer** tool (analyzing your code, the IDE points out possible mistakes, so you do not need to run the ``flutter analyze`` command). Other new tools include **Flutter Inspector** and **Observatory**. You can use them to test, analyze, and debug your application.

## Run the application in the debug mode
To run your application in the **Debug Mode**, click the <img src="https://github.com/jetpack-pizza/demo/blob/master/img/6_debug_icon.png" alt="Debug" width="16"/> icon in the upper-right corner of the main IDE window. This mode includes all debugging information, enables **Observatory** and service extensions. Now you can use the **Debugger** to view the data on frames and variables.
<p align="center">
<img src="https://github.com/jetpack-pizza/demo/blob/master/img/6_debugger.png" alt="Debugger" width="700"/>
</p>

## Analyze issues
This tool allows you to monitor issues, such as potential problems and inconsistencies, that might arise during the project development. In the the **Dart Analysis** tool window you can:
  * Sort the errors by severity or location.
  * Group errors by severity.
<p align="center"><img src="https://github.com/jetpack-pizza/demo/blob/master/img/6_dart_analysis_1.gif" alt="" width="590"/></p>
 
 * Use the **Dart Problems Filter** to filter out some error messages.
 <p align="center"><img src="https://github.com/jetpack-pizza/demo/blob/master/img/6_dart_analysis_2.gif" alt="" width="590"/></p>
 
  * Determine the precise location of the issue and navigate to it.
  * Identify the type of the issue (there can be errors, warnings, or hints).
  * Enable the **Autoscroll to Source** feature that helps get to the issue quickly.
  * Restart the Dart Analysis Server.

## Use the Flutter Inspector
Widgets are the core building blocks in Flutter applications, and IntelliJ IDEA has got a tool for visualizing and exploring widget trees and debugging UIs. The **Flutter Inspector** helps to manage bidirectional mapping between the active Flutter UI and the corresponding visualization of the **Widgets** tree and the **Render** tree. Thus, you can follow this mapping into the source and see where in the code (whether it is your code or the the framework code) a widget is being created or configured. The **Flutter Inspector** displays widgets that were created directly in your application in Bold, making it easier to distinguish between widgets created in the app and in the framework.

To inspect your application, check the layouts, widgets, and performance, open the tool by clicking **Flutter Inspector** on the right side of the main IDE window (alternatively, choose **View | Tool Windows | Flutter Inspector** or find the icon in the **Run** tool window). Use the toolbar to interact with the elements of the app and to switch between the Inspector tabs:
<p align="center">
<img src="https://github.com/jetpack-pizza/demo/blob/master/img/6_inspector_toolbar.png" width="600" alt="Inspector Toolbar"/>
</p>

### Enable the Select widget mode
To activate this mode, click the <img src="https://github.com/jetpack-pizza/demo/blob/master/img/6_select_widget_mode.png" alt="Select Widget Mode" width="16"/> icon. Now you can:
- Select a widget that you need, so while interacting with your device you can see which widget is responsible for a specific position on the screen. 
- See the tree of widgets, the widget's position, and its properties.
- Get to the source code of a particular widget: select a widget, right-click it, and choose **Jump to Source** from the menu. Then the **Editor** will show you the code section where this widget is created.
>**Tip:** Hover over a property value to see the list of allowed values. When you perform a hot reload, the **Flutter Inspector** will update the widget properties accordingly.

|<img src="https://github.com/jetpack-pizza/demo/blob/master/img/6_allowed_values.png" alt="Allowed values" width=""/>|<img src="https://github.com/jetpack-pizza/demo/blob/master/img/6_allowed_values_2.png" alt="Allowed values" width="590"/>|
--- | ---

### Refresh widget info
Click the <img src="https://github.com/jetpack-pizza/demo/blob/master/img/6_refresh.png" alt="Refresh Widget Info" width="16"/> icon to update the widget information that is displayed in the **Flutter Inspector**. The widget tree will show the selected widget in case you have scrolled the list to another position.

### Enable the Debug paint mode
The **Debug Paint** mode helps to understand how your widgets are laid out on the screen. Click the <img src="https://github.com/jetpack-pizza/demo/blob/master/img/6_debug_paint.png" alt="Debug Paint" width="16"/> icon to activate this mode.
<p align="center">
<img src="https://github.com/jetpack-pizza/demo/blob/master/img/6_debug_paint_mode.png" alt="Debug Paint" width="300"/>
</p>

### Enable the Toggle platform mode
Click the <img src="https://github.com/jetpack-pizza/demo/blob/master/img/6_platform.png" alt="Platform Mode" width="16"/> icon to activate this mode and switch between Android and iOS platform rendering to test platform-specific rendering without having to use two devices.

### Enable the Performance Overlay
The **Performance Overlay** displays the GPU & CPU threads performance graphs and helps you to analyze and improve the performance. Click the <img src="https://github.com/jetpack-pizza/demo/blob/master/img/6_performance_overlay.png" alt="Performance Overlay" width="16"/> icon to enable this feature. Now you can test your application and check the performance statistics on the screen.
<p align="center">
<img src="https://github.com/jetpack-pizza/demo/blob/master/img/6_performance_mode.png" alt="Performance Overlay" width="300"/>
</p>

## Debug performance issues
### Use the Timeline
The **Timeline** is a tool for debugging performance issues: it allows you to capture the stack snapshot. This feature works in conjunction with the **Observatory**.

## Use the Observatory
The **Observatory** is a debugging and profiling tool for profiling, examining the heap, and displaying code coverage. To open the **Observatory**, you must run your application and click the <img src="https://github.com/jetpack-pizza/demo/blob/master/img/6_observatory_button.png" alt="Observatory" width="16"/> icon (it is available in the **Run** or **Flutter Inspector** tool windows). You can use the **Observatory** to analyze the Dart virtual machine performance, to obtain the current data on memory leaks, check which lines of code have been executed, etc.
<p align="center">
<img src="https://github.com/jetpack-pizza/demo/blob/master/img/6_observatory.png" width="900"/>
</p>

---
To see the rest of features provided by the **Flutter Inspector**, click the gear-wheel icon in the upper-right corner of the tool window.

### Enable baseline painting
Enable this feature to see the baseline paintings in your Flutter application: each RenderBox will paint a line at its baseline.
<p align="center">
<img src="https://github.com/jetpack-pizza/demo/blob/master/img/6_baseline.png" width="500"/>
</p>

### Enable repaint rainbow
This feature shows the rotating colors on layers when the repainting or rebuilding is performed. The **Repaint rainbow** helps to understand which areas of the screen are being repainted, and which are not.

### Enable slow animations
Slow your animations down and perform a visual inspection in case something is not animating properly.

### Hide debug banner
Hide the **Debug** banner that is displayed in the upper-right corner of your application by default. This feature allows you to do it without rebuilding the application.

### Enable auto horizontal scroll
Enable this feature to make the IDE perform the horizontal scroll automatically when you navigate in the widget structure tree.

### Highlight nodes
When this feature is enabled, the nodes that are displayed in two panes of the **Flutter Inspector** are highlighted.
<p align="center">
<img src="https://github.com/jetpack-pizza/demo/blob/master/img/6_highlight_nodes.png" width="500"/>
</p>

## Manage rendering
You can switch to the **Render Tree** tab in case there are problems with UI elements rendering. Note that the **Widgets** and **Render Tree** tabs are connected, so if you select a widget and switch between tabs, you get the data about the same widget. 
>**Tip:** If you have animations in your application, the **Render Tree** displays the values being changed on-the-fly. 

|<img src="https://github.com/jetpack-pizza/demo/blob/master/img/6_widgets-render_tree_1.png" alt="Allowed values" width="590"/>|<img src="https://github.com/jetpack-pizza/demo/blob/master/img/6_widgets-render_tree_2.png" alt="Allowed values" width="590"/>|
--- | ---

## Apply quick-fixes
If the **Dart Analysis** tool window shows you a number of errors, you can use suggested quick-fixes. Place the cursor to the code fragment and press the ``Alt+Enter`` (Win, Linux) or ``⌘↩`` (Mac OS) (or use the intention action icon).

## Run unit tests
You can create and run unit tests for your Flutter applications:
1. Find the **Run** icons in the gutter of your test file.
<p align="center">
<img src="https://github.com/jetpack-pizza/demo/blob/master/img/6_test_file_gutter.png" alt="" width="400"/>
</p>

2. Click the icon and choose whether you want to **run** or **debug** your test (alternatively, right-click in the **Editor** and select the required option). 
<p align="center">
<img src="https://github.com/jetpack-pizza/demo/blob/master/img/6_test_run_debug.png" alt="" width="300"/>
</p>

3. The IDE displays the data on tests in the **Run** or **Debug** tool windows respectively.

<p align="center">
<img src="https://github.com/jetpack-pizza/demo/blob/master/img/6_test_passed.png" alt="" width="800"/>
</p>

<p align="center">
<img src="https://github.com/jetpack-pizza/demo/blob/master/img/6_test_breakpoints.png" alt="" width="800"/>
</p>
