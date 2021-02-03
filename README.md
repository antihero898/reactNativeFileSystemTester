# reactNativeFileSystemTester
Simple application that tests the efficiency of file reading packages using various sizes json files.

While recently working on a project for a client, I noticed differing loading times between native file system packages when reading various sized json files. react-native-fs was taking about 1500 ms to read in a json file that only took 500ms while using rn-fetch-blob. 

Although the big difference between these packages is the layer that is used (rn-fetch-blob using the native layer while react-native-fs is javascript), I want to see how consistent (or inconsistent) the usage of layers are between file-system packages that are available for react-native via npm. 

This project overall aims to test all of these dependencies while taking into consisteration package size and features.

Packages that this repo aims to test:
- react-native-fs
- rn-fetch-blob
- react-native-filesystem
- expo-file-system
- react-native-fetch-blob
- react-native-file-access

