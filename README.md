1. Create custom launch screen in Xcode (File > New > File and choose Launch Screen)
2. Add it to .NET MAUI project Resources folder
3. Make sure that it has the build action `InterfaceDefinition`
4. Exclude `MauiSplashScreen` for iOS (in csproj)
5. Include custom launchscreen only for iOS (in csproj)
6. Specify launch screen in `info.plist`

> ![NOTE]
> As of iOS 16.4 your app has to be code signed in order for the splash screen to show up. If you do not sign your app, the splash screen will always show black.
