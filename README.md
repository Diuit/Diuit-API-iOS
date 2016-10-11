# Manually Install Diuit API in Your Project



## Choose the Right Version

* For Swift 3: User version 2.0.1

* For Swift 2.3: Use version 1.2.0

  ​



## How to Install Diuit API Manually



1. Open your existed project or create a new project.
2. Download this repo
3. Choose the framework based on your Swift version and configuration of bitcode. (You will fail to upload onto App store due to inconsistent configuration)
   ![bitcode](http://i.imgur.com/jyMQWbl.png)
4. Drag both **DUMessaging.framework** and **SocketIO.framework** to your project navigator in Xcode. Make sure that "Copy items if needed" is checked when Xcode asks you about the options for adding files.
   ![copyfiles](http://i.imgur.com/zlgLeWG.png)
5. Now you should see both frameworks in your project navigator.
   ![projectNavigator](http://i.imgur.com/Kpnqdy6.png)
6. In your target -> General tab, click "+" in **Embedded Binaries** section. Add both **DUMessaging.framework** and **SocketIO.framework**.
   ![embededBinaries](http://i.imgur.com/JpgL26c.png)
7. That's it! Now you can go on your project with the power of Diuit.



## You Need to Know

1. Even though Swift 3 is officially released, Diuit API will still maintain versions for Swift 2.3( v. 1.2.0 +). Since pod file spec does not support dependency of a specific branch, we have to distribute the framework by this method. Thus, you can ONLY install Diuit API for Swift 2.3 **manually**.
2. Diuit API for Swift 3 (v. 2.0+) can be installed via Cocoapods or manually.
3. To hide unwanted strange log in Xcode 8, you have to add an environment variable `OS_ACTIVITY_MODE` and set its value to `disable` in your scheme.
   ![env](http://i.imgur.com/EhrJ3kC.png)

