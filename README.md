1. Create custom launch screen in Xcode (File > New > File and choose Launch Screen), see [here](https://github.com/jfversluis/MauiStoryboardSample/blob/main/MauiStoryboardSample/Resources/LaunchScreen.storyboard).
2. Add it to .NET MAUI project Resources folder, see [here](https://github.com/jfversluis/MauiStoryboardSample/blob/main/MauiStoryboardSample/Resources).
3. Make sure that it has the build action `InterfaceDefinition`, see [here](https://github.com/jfversluis/MauiStoryboardSample/blob/main/MauiStoryboardSample/MauiStoryboardSample.csproj#L58).
4. Include custom launchscreen only for iOS (in csproj), see [here](https://github.com/jfversluis/MauiStoryboardSample/blob/main/MauiStoryboardSample/MauiStoryboardSample.csproj#L57).
5. Exclude `MauiSplashScreen` for iOS (in csproj), see [here](https://github.com/jfversluis/MauiStoryboardSample/blob/main/MauiStoryboardSample/MauiStoryboardSample.csproj#L41).
6. Specify launch screen in `info.plist`, see [here](https://github.com/jfversluis/MauiStoryboardSample/blob/main/MauiStoryboardSample/Platforms/iOS/Info.plist#L31-L32).

> [!NOTE]
> As of iOS 16.4 your app has to be code signed in order for the splash screen to show up. If you do not sign your app, the splash screen will always show black.
