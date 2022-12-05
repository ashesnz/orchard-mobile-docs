# Goals

* Improvement of startup time  (Android) and other features with an upgrade of Gradle (https://gradle.org/whats-new/gradle-7/)
* Consider moving to the new Architecture  https://reactnative.dev/blog/2022/03/15/an-update-on-the-new-architecture-rollout
  * Currently sitting on version React Native version (`0.61.5`) Can be upgraded to (`0.70`) https://reactnative.dev/blog/2022/09/05/version-070
  * Last version upgrade release date - [`Nov 24, 2019`](https://github.com/facebook/react-native/releases/tag/v0.61.5)
  * Using **React Native update helper** (https://react-native-community.github.io/upgrade-helper/?from=0.61.5&to=0.71.0-rc.3)
* Consistent Typescript Support (moving away from js/jsx files to ts/tsx)
* Verify your app is working as expected on a device (or a simulator/emulator) from the user perspective (Consider using https://github.com/wix/detox/, https://blog.logrocket.com/react-native-end-to-end-testing-detox/)
* A fairly **consistent 60 FPS** across the supported devices



# Documentation (Amend README.md)

### Supported Android/iOS devices

- **Supported iOS versions**: 11+ (update to appropriate version)
- **Supported Android versions**: 5.0+ (update to appropriate version)
### Prerequisites

- [Node.js](https://nodejs.org/en/download/)
- [Watchman](https://facebook.github.io/watchman/docs/install.html)
- [Yarn](https://yarnpkg.com/en/docs/install)
- [JDK (Java development kit)](https://www.oracle.com/java/technologies/downloads/)
- [Android Studio](https://developer.android.com/studio?gclid=CjwKCAiAp7GcBhA0EiwA9U0mtrwIcZt277HkrNFiVD7b3QJr6FPulIaiiU6ZUb1TnHrONzsTgiQpwhoCp3EQAvD_BwE&gclsrc=aw.ds)
- React Native CLI - Use `$ yarn global add react-native-cli` to install the CLI.

More information on getting started can be found [here](https://reactnative.dev/docs/environment-setup)

#### Setup Issues  

Q. I'm unable to connect to my device physically when running application is built?

A. Running ``adb reverse tcp:8081 tcp:8081`` [seems to do the trick](https://github.com/facebook/react-native/issues/8309)

# DX (Developer) Improvements
* https://github.com/infinitered/reactotron

# **Questions**
* Do we track application log errors?
* Some tests are still failing? Get tests to pass and integrate into CI pipeline
