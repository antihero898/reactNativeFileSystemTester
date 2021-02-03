# reactNativeFileSystemTester
Simple application that tests the efficiency of file reading packages using various sizes json files.

Note: this project currently targets only iOS. Android will be a following feature.

While recently working on a project for a client, I noticed differing loading times between native file system packages when reading in various sized json files. react-native-fs was taking about 1500 ms on average to read in a json file that only took 500ms (on average) while using rn-fetch-blob. While one second may seem unnoticeable, it becomes quite a visible hiccup when occurring in a fuild application process. 

Although the big difference between these packages is the layer that is used (rn-fetch-blob using the native layer while react-native-fs is javascript), I want to see how consistent (or inconsistent) the usage of layers are between file-system packages that are available for react-native via npm. 

This project overall aims to test all of these dependencies while taking into consisteration package size and features.

Packages that this repo aims to test:
- [react-native-fs](https://www.npmjs.com/package/react-native-fs/v/1.2.0)
- [rn-fetch-blob](https://www.npmjs.com/package/rn-fetch-blob)
- [react-native-filesystem](https://www.npmjs.com/package/react-native-filesystem)
- [expo-file-system](https://www.npmjs.com/package/expo-file-system)
- [react-native-fetch-blob](https://www.npmjs.com/package/react-native-fetch-blob)
- [react-native-file-access](https://www.npmjs.com/package/react-native-file-access)

