This is a Kotlin Multiplatform project targeting Android, iOS.

* `/composeApp` is for code that will be shared across your Compose Multiplatform applications.
  It contains several subfolders:
  - `commonMain` is for code that’s common for all targets.
  - Other folders are for Kotlin code that will be compiled for only the platform indicated in the folder name.
    For example, if you want to use Apple’s CoreCrypto for the iOS part of your Kotlin app,
    `iosMain` would be the right folder for such calls.

* `/iosApp` contains iOS applications. Even if you’re sharing your UI with Compose Multiplatform, 
  you need this entry point for your iOS app. This is also where you should add SwiftUI code for your project.

How to use

Switch between the branches 1 to 7 to checkout from a more initial to a more advanced state of the application.

Architectural diagram

The UI/Framework layers reside in the native apps, while everything from the View Model up to Data layer is in the common KMP module.

![287762783-a1a465db-1484-4eb8-ab3c-1d43b457d7c2](https://github.com/yigitkarakurt/DailyPulse/assets/73107549/82887cf8-41ff-4283-a0d1-d192641a6f2c)

Architectural Layers

<img width="531" alt="287763244-620fb7ca-68cb-428c-b134-4a012a8836eb" src="https://github.com/yigitkarakurt/DailyPulse/assets/73107549/2106c88a-f63a-49bb-9c69-def943cb4871">

Learn more about [Kotlin Multiplatform](https://www.jetbrains.com/help/kotlin-multiplatform-dev/get-started.html)…
