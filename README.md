# Manually Install Diuit API in Your Project



* Version: 1.2.0
* ​:heavy_check_mark: Compatible with Swift 2.3
* ​:x:​ Do not work with Swift 3 now



## How to Install Diuit API



1. Open your existed project or create a new project.
2. Download this repo
3. Choose the framework based on your configuration of bitcode. (You may fail to upload onto App store due to inconsistent configuration)
   ![bitcode](http://i.imgur.com/jyMQWbl.png)
4. Drag both **DUMessaging.framework** and **SocketIO.framework** to your project navigator in Xcode. Make sure that "Copy items if needed" is checked when Xcode asks you about the options for adding files.
   ![copyfiles](http://i.imgur.com/zlgLeWG.png)
5. Now you should see both frameworks in your project navigator.
   ![projectNavigator](http://i.imgur.com/Kpnqdy6.png)
6. In your target -> General tab, click "+" in **Embedded Binaries** section. Add both **DUMessaging.framework** and **SocketIO.framework**.
   ![embededBinaries](http://i.imgur.com/JpgL26c.png)
7. That's it! Now you can go on your project with the power of Diuit.



## You May Want to Know

1. SocketIO forgets to close detail log in this version. However this is the stable version to work with Swift 2.3 and they may not maintain this version anymore. You probably need to add some tags or identifier for your log.
2. Even though Swift 3 is officially released, Diuit API will still maintain versions for Swift 2.3( v. 1.2.0 +). Since pod file spec does not support dependency of a specific branch, we have to distribute the framework by this method. Thus, you can ONLY install Diuit API for Swift 2.3 **manually**.
3. Diuit API for Swift 3 (v. 2.0+) can be installed via Cocoapods or manually, stay tuned.

