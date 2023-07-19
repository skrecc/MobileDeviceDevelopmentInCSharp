# MobileDeviceDevelopmentInCSharp
Recherche for the mobile device development in C#

## Tools & technologies to write cross-platform applications in C# 
limitations / benefits are listed

Xamarin
* Is abstraction layer that manages communication of shared code with underlying platform code.
* Shared code is bound into underlying platform SDKs - iOS (Xamarin.iOS) and Android (Xamarin.Android)
* Xamarin application can use .NET BCL which is known by C# developers
* Existing C# code can be recompiled and used in Xamarin application
* Apps are compiled in native code - .apk file on Android, or an .ipa file on iOS
* Native platform Interop - possiblity of invoking native platform libraries
* Provides Xamarin.Essentials API to access resources across all platforms

Pros:
* Code reusability
* Performance - compilation into native code
* Single language knowledge needed - C# - for application code
* Community suppport

Cons:
* UI has to be written using native libraries
* Delay in support of platform specific features

Xamarin.Forms

MAUI
* Benefits over Xmarin.Forms

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
