FaceAware for Android Studio
========
[![License](https://img.shields.io/badge/License-Apache%202.0-blue.svg)](https://opensource.org/licenses/Apache-2.0)
<br>
FaceAware is zoom library to face for Android.<br>

<img src="https://github.com/memishood/FaceAware-Android/blob/master/avatarExample.png" width=50%>

Let me show how to use this library:

## Setup
```
allprojects {
    repositories {
        ...
        maven { url 'https://jitpack.io' }
    }
}
```
```
dependencies {
    implementation 'com.github.memishood:FaceAware-Android:1.2'
}
```

## XML

```xml
<tr.com.emrememis.library.FaceAware
    android:id="@+id/faceAware"
    android:layout_width="wrap_content"
    android:layout_height="wrap_content"
    app:face_elevation="25"/>
```
## Params

| Params | Value |
| :------: | :------: |
| app:face_elevation | int |
-------------------

## Kotlin

```kotlin  
        faceAware.setImageResource(R.drawable.test)
        //or
        faceAware.setImageDrawable(ActivityCompat.getDrawable(this,R.drawable.test))
        //or
        faceAware.setImageBitmap(BitmapFactory.decodeResource(resources,R.drawable.test))
        //or
        Glide.with(this).load(R.drawable.test).into(faceAware)
```

do not use android:src="image", use on your code.

-------------------
## For better understanding
<img src="https://github.com/memishood/FaceAware-Android/blob/master/largeExample.jpg" width=50%>