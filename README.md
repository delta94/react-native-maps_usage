react-native-maps usage
===================

## Execution screen 
> <img src="./images/RN_map.png" />
  
-----------------------

## How to use
> ### Source, more details
> [react-native-maps](https://github.com/react-native-community/react-native-maps)

> ### **For ios**
> - First, install react-native-maps
> ```bash
>   npm install --save react-native-maps
> ```
> - Second, Move dir to ~project/ios and run pod install
> ```bash
>   # in project dir
> 
>   cd ios
>   pod install
>   cd ..
> ```
> - Third, use MapView
> ```javascript
>   import MapView from 'react-native-maps';
>   ...
>   <MapView />
>   ...
> ```
> It'll use an apple map

> ### **For android**
> - First, get google api key.
> - Second, open ~project/android/app/src/main/AndroidManifest.xml file. <br/> And add these lines in application element
> ```xml
>   <application
>   ...>
>     ...
>     <meta-data
>     android:name="com.google.android.geo.API_KEY"
>     android:value="API_KEY" />
>     ...
>   </application>
> ```
> - Third, open ~project/android/build.gradle file. <br/> And add these lines in ext
> ```gradle
>   buildscript {
>     ext {
>       ,,,
>       supportLibVersion = "28.0.0"
>       googlePlayServicesVersion = "17.0.0"
>       androidMapsUtilsVersion = "0.6.2"
>     }
>     ,,,
>   }
> ```
> - Fourth, use MapView
> ```javascript
>   import MapView from 'react-native-maps';
>   ...
>   <MapView />
>   ...
> ```
> It'll use a google map
