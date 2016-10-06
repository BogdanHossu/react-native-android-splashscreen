# react-native-android-splashscreen

I found a lot of tutorials on how to replace the default white splash screen with a custom one, but most of them they were not complete or they were not used on a react-native project. So I decided to make this repo with my simple solution for future projects.

## Result

<img src="http://i66.tinypic.com/2vs3hpe.gif" width="300"/>

## Documentation

My solution was to create all of the drawable folders and create a splash screen with the logo for each device size. All of the splash images are ```/android/app/src/res```.

* I used [this sketch resource](http://www.sketchappsources.com/free-source/1631-android-screen-size-artboards-sketch-freebie-resource.html) to create my splash screen for all required sizes.
* For this example I used the [Yellow lazy bird logo](http://www.sketchappsources.com/free-source/731-yellow-lazy-bird-sketch-freebie-resource.html)

To change the splash screen image with another one you simply need to edit the ```android:src="@drawable/splash"``` in the ```/android/app/src/res/drawable/splash_screen.xml``` with your own image.

To change the splash screen background color with your own you need to define your color in the ```/android/app/src/res/values/colors.xml``` and than to set ```<item android:drawable="@color/<your color>/>``` it in the ```/android/app/src/res/drawable/splash_screen.xml```
