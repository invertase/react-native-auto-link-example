# React Native Auto Link Example

The changes in this template will eventually be part of the main RN template (`react-native init`) - for now this is an example template that can be experimented with and be used to try out auto-linking.

> **Warning**: this uses a pre-release version of the cli (which has auto-linking support), as such; some things may not work as expected - please provide feedback and report any bugs/issues

## Init a React Native project with Auto Linking:

Run the below command to init a new React Native project that supports auto-linking. 

```
npx @react-native-community/cli@next init --template=@invertase/template <myProjectName>
```

**Note**: Some React Native modules may be using an old configuration format and will be excluded from auto-linking but will print warnings similar to the following when running `react-native start`:

![image](https://user-images.githubusercontent.com/5347038/56456147-1ad9c380-6360-11e9-85a0-c2d85c1a6580.png)

Please report these issues to the individual module repos

## Adding React Native modules to your project

 - `yarn add` or `npm install` your react-native module
 - Rebuild your app:
   - **Android**: `react-native run-android`
   - **iOS**: `cd ios/ && pod install`, `react-native run-ios`
   
## Additional Resources

 - [Android PR](https://github.com/react-native-community/cli/pull/258)
 - [iOS PR](https://github.com/react-native-community/cli/pull/256)
 - [React Native PR to apply template changes](https://github.com/facebook/react-native/pull/24506)
 - [CLI Issue: 'Umbrella: Autolinking'](https://github.com/react-native-community/cli/issues/288)
