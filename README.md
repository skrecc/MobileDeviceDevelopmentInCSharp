# MobileDeviceDevelopmentInCSharp
Recherche for the mobile device development in C#

## Tools & technologies to write cross-platform applications in C# 
limitations / benefits are listed

### Xamarin
* Open source cross-platform development framework allowing to build native mobile applications for iOS and Android using the C#
* Abstraction layer manages communication of shared code with underlying platform code
* Shared code is bound into underlying platform SDKs - by iOS (Xamarin.iOS) and Android (Xamarin.Android)
* Xamarin application can use .NET BCL which is known by C# developers
* Existing C# code can be recompiled and used in Xamarin application
* Apps are compiled in native code - .apk file on Android, or an .ipa file on iOS
* Native platform Interop - possiblity of invoking native platform libraries
* Provides Xamarin.Essentials API to access resources across all platforms

Pros:
* Code reusability
* Performance - compilation into native code
* Single language knowledge needed - C# - for application code
* Open source
* Community suppport

Cons:
* UI has to be written using native libraries
* Delay in support of platform specific features
* Xamarin app is larger than native app (Mono runtime and BCL assemblies)

### Xamarin.Forms
* Open source UI framework - part of Xamarin platform - for building user interfaces across multiple platforms
* User interfaces are created in XAML or C#, MVVM supported
* UI is rendered as native platform controls by target platform renderers
* Application typically consist of shared .NET (bussiness logic, UI) and platform specifics projects
* Xamarin.Forms platform-specifics allows utilization of specific feature available only on specific platform
* Development can be even simplified by usage Xamaring.Forms Shell providing common navigation, search, app structure and layout basis

Pros:
* Single code base application development - C# and XAML
* Saves development time and effort
* Native app performance and look - due compilation in native code
* Prebuild controls and layouts
* Access to target platform specific features
* Support to build custom reusable UI components

Cons:
* Customization limitations - provided pre-build controls may not cover app requrements
* Performance overhead compared to native apps - shared controls mapping can add additional processing and redering steps
* Not all platform specifics are available
* Larger Xamarin.Forms app size than native app
* Platform specific availability delay
* Shared Xamarin.Forms UI controls may restrict certain design choices or require additional customization


### MAUI
* Multi-platform App UI is the evolution of Xamarin.Forms, a open source, cross-platform UI framework for building native apps
* Can build native mobile, desktop and web applications using a shared codebase and UI
* Can run on multiple platforms including iOS, Android, macOS and Windows
* Uses a series of platform-specific frameworks for creating apps: .NET Android, .NET iOS, .NET macOS, and Windows UI 3 (WinUI 3) library provided by .NET6 or greater
* These frameworks have access to the same .NET BCL and this libraries abstracts the details of the underlying platform
* MAUI provides also a single framework for building the UIs, but platform specifics UI's can be also defined separately using .NET Android, .NET iOS, .NET macOS or WinUI 3
* As evolution of Xamarin.Forms are also provided cross platform API's for accessing device features, collection of prebuild controls, layouts and databinding support
* Is compatibile with existing Xamarin.Forms projects, allowing developers to migrate their existing apps

Pros (over Xamarin.Forms):
* Single project structure with multitargeting - combining the shared code and resources for multiple platforms into a single project file
* Performance enhancements - new rendering architecture, optimized layouts and improved startup time
* Extended target platforms support - macOS, Linux planned but not released yet
* Improved controls, layouts and styling options
* Hot Reload introduced - code and UI changes while the app is running. Also available in latter Xamarin.Forms

Benefits over Xmarin.Forms?

Before decision to use Xamarin/MAUI is allways needed to consider purpose of the app.
As the biggest benefit is code sharing between platforms then developing platform specific apps decreasing such benefit.

Is there any other?

## Roadmap of hard skills to develop mobile device apps in C#

## List skills / knowledge outside .Net platform to develope feature-rich mobile apps

### Native Development with Platform-specific Tools
Native development offers the most direct access to platform-specific features and performance but requires specific knowledge for each platform.
Generally saying each platform has it's own specific of: application infrastructure, data persistence, networking, background processing, testing and debugging, CI/CD.

#### iOS
* Swift or Objective-C knowledge - as they are the primary languages used for iOS app development
* iOS Software Development Kit (SDK) knowledge
* Xcode is official IDE for iOS app development
* Understanding the principles of UI design for iOS apps
* App Store app deployment
* Testing tools: XCTest
* CI/CD: Bitrise or Jenkins
  
#### Android
* Java or Kotlin knowledge - as they are the primary languages used for Android app development
* Android Software Development Kit (SDK) knowledge
* Android Studio official IDE
* Understanding the principles of UI design for Android apps, Android UI layouts using XML files.
* Google Play Store app deployment
* Testing tools: JUnit, Espresso or Mockito
* CI/CD: Jenkins

There is also several possibilities to use C# with other frameworks.

### Flutter with C#
Flutter is a popular open-source framework developed by Google that allows you to build cross-platform mobile apps using the Dart programming language.
Flutter primarily uses Dart, there are community-driven projects like Flutter for Xamarin that enable you to write Flutter code in C#.
https://docs.flutter.dev/get-started/flutter-for/xamarin-forms-devs
https://www.flutnet.com/

### Unity with C#
Unity is primarily used for game development, it can also be used to create interactive mobile applications.
https://unity.com/how-to/learning-c-sharp-unity-beginners#what-languages-can-you-use-unity--2

### React Native with C#
React Native is a framework developed by Facebook for building cross-platform mobile applications using JavaScript.
React Native can be used with C# through projects like React Native for Xamarin
https://microsoft.github.io/react-native-windows/docs/native-code-language-choice
