# Running applications

## Prerequisites
To run and test your application, you must have either a connected device or a configured virtual device. You can check the status in the **Flutter Device Selection** field in the upper-right corner of the main IDE window. In case you have not added a device, you can do it with the help of the **Android Virtual Device (AVD) Manager**. 

1. Choose **Tools | Android | AVD Manager** on the main tool bar.
2. Click **Create Virtual Device** in the bottom left corner.
3. Configure hardware settings and click **Next**.
4. Select a system image and click **Next**. Note that if the required release is missing, you can download it in this dialog.
5. Verify the configuration and click **Finish**.  

> **Note:** If you need to use the iOS simulator, make sure that your Xcode SDK is installed and configured properly. 

Alternatively, you can use a physical device. To check the connection either use the ``flutter doctor`` command in the console or click **Flutter Doctor** at the top of the ``pubspec.yaml`` window: it will provide you with the data on your environment.

## Run the application
Action | Description
--- | --- 
**Use the toolbar** | Use the buttons in the upper-right corner of the main IDE window to run your application and check its look-and-feel and performance. <p align="center"><img src="https://github.com/jetpack-pizza/demo/blob/master/img/5_run_app_toolbar.png" alt="Toolbar" width="590"/></p>
**Build project** | Build your project either by clicking the hammer icon or by using the ``Ctrl+F9`` (Win, Linux) or ``⌘F9`` (Mac OS) shortcuts.
**Select Flutter device** | Select the device that you want to use for running your application.
**Configure running/debugging** | Configure your Run/Debug options. You can perform the fine tuning: set the entry point for your application, set additional command-line arguments, manage build flavor, and add the tasks that should run before the launch.<p align="center"><img src="https://github.com/jetpack-pizza/demo/blob/master/img/5_run_debug_configuration.png" alt="Run/Debug Configuration" width="600"/></p>
**Run the app** | Run your project (use the ``Shift+F10`` (Win, Linux) or ``^R`` (Mac OS) shortcuts).
**Debug the app** | Run the project in the **Debug mode** and study the console output to make adjustments, if necessary (use the ``Shift+F9`` (Win, Linux) or ``^D`` (Mac OS) shortcuts).
**Run with coverage** | Run your application with coverage to study the coverage measurement results. To check the current coverage configuration, open the **Settings/Preferences** dialog and go to **Build, Execution, Deployment &#9134; Debugger &#9134; Coverage**.
**Profile the app** | Launch your application in the **Profile** mode. You need to use this mode if you are using **Observatory** (a debugging and profiling tool shipped with the Dart SDK) for profiling your application. **Note:** The **Profile** mode is not available on simulators and emulators because this kind of profiling does not not represent the real performance.
**Hot reload the app** | Apply the latest code changes. Press ``Ctrl+Back Slash`` (Win, Linux) or ``⌘\`` (Mac OS) to view the changes implemented in the app immediately.
**Attach a debugger** | Attach a debugger to your application process.
**Stop the app** | Stop the application running.
**Run the application in Terminal** | Use **Terminal** in IntelliJ to run Flutter code using the ``flutter run``, ``flutter run --release``, ``flutter run --profile``, and ``flutter test`` commands. <p align="center"><img src="https://github.com/jetpack-pizza/demo/blob/master/img/5_terminal.png" alt="Allowed values" width="900"/></p>
**Run the app in Profile and Release modes** | Run your application in the **Profile** or **Release** mode. To do so, choose the required mode from the **Run** menu.<p align="center"><img src="https://github.com/jetpack-pizza/demo/blob/master/img/5_run_modes.png" alt="Run modes" width="400"/></p>


---

**Next:** Flutter and Dart plugins offer a number of tools for [testing and debugging](https://github.com/jetpack-pizza/demo/blob/master/content/testing-and-debugging.md).  
