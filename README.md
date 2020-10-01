#Android Webkit

[![Build Status](https://travis-ci.org/vinkas0/webkit-android.svg?branch=master)](https://travis-ci.org/vinkas0/webkit-android)
[![](https://jitpack.io/v/com.vinkas/webkit-android.svg)](https://jitpack.io/#com.vinkas/webkit-android)
[![License: MIT](https://img.shields.io/badge/License-MIT-orange.svg)](https://opensource.org/licenses/MIT)
<hr />
Easy to use android module to create apps for responsive or mobile websites using custom WebView. Build your website's own android app in minutes!!!
####[Download Sample APK](https://github.com/Vinkas-com/Webkit/releases/download/1.0.1/sample.apk)
##Add as dependency module
Add this on your project's root 'build.gradle' file
```
  repositories { 
        jcenter()
        maven { url "https://jitpack.io" }
   }
```
Add this on your app folder's 'build.gradle' file
```
   dependencies {
         compile 'com.vinkas:webkit-android:1.0.1'
  }
```
#How we can use this 
###Java code
```
    @Override
    protected void onCreate(Bundle savedInstanceState) {
        super.onCreate(savedInstanceState);
        setContentView(R.layout.activity_main);
        BrowserLayout browserLayout = (BrowserLayout) findViewById(R.id.browser);
        browserLayout.loadUrl("https://github.com/Vinkas-com");
    }
```
###Xml layout
```
<?xml version="1.0" encoding="utf-8"?>
<com.vinkas.webkit.BrowserLayout xmlns:android="http://schemas.android.com/apk/res/android"
    android:id="@+id/browser"
    android:layout_width="match_parent" android:layout_height="match_parent">
</com.vinkas.webkit.BrowserLayout>
```
