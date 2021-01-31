# Feeling Sports SDK for Android

The Feeling Sports SDK enables people to play their favorites Feeling Sports games into your app.

## 1. Integrate the Feeling Sports SDK

Add the following to your `app/build.gradle` file.
```gradle
dependencies {
    // Feeling Sports Games
    implementation 'com.feelingsports.android:fs-android-sdk:1.0.0'
}
```

Add the following to your `project/build.gradle` file.
```gradle
allprojects {
    repositories {
        maven {
            url  "https://dl.bintray.com/fs/maven"
        }
    }
}
```

## 2. Edit Your Resources and Manifest


Add the following to your `app/src/main/res/values/string.xml` file.

```xml
<string name="facebook_app_id">PASTE_YOUR_FB_APP_ID_HERE</string>
<string name="fb_login_protocol_scheme">PASTE_YOUR_FB_SCHEME_HERE</string>
<string name="fs_api_key">PASTE_YOUR_FS_API_KEY_HERE</string>
```

Add the following to your `app/manifest/AndroidManifest.xml` file.

```xml
<uses-permission android:name="android.permission.INTERNET"/>
```

## 3. Add the Feeling Sports Full Game

Add the following to your layout XML file.

```xml
<com.feelingsports.android.FSFullGame
    android:id="@+id/fsFullGame"
    android:layout_width="match_parent"
    android:layout_height="match_parent" />
```
Congrats, you've added Feeling Sports games to your app! 
