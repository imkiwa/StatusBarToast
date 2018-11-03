StatusBarToast
==============
[![GitHub top language](https://img.shields.io/github/languages/top/imkiva/StatusBarToast.svg)](https://github.com/imkiva/StatusBarToast)
[![license](https://img.shields.io/github/license/imkiva/StatusBarToast.svg?colorB=000000)](https://github.com/imkiva/StatusBarToast)
[![Download](https://api.bintray.com/packages/imkiva/maven/statusbar-toast/images/download.svg) ](https://bintray.com/imkiva/maven/statusbar-toast/_latestVersion)

Displaying text on your StatusBar!(Telegram-X like)


## Features
* Display Progress Bar
* Change Text Dynamically
* Toggle Progress Bar States


![demo](demo/demo.gif)


## Usage
* Add following code to your `build.gradle`:
```groovy
compile 'com.imkiva.statusbar.toast:library:1.0-1'
```
* Unlimited Duration Toast:
```java
// create a toast and show it
StatusBarToast toast = new StatusBarToast.Builder(this)
        .setText("Connecting")
        .setShowProgressBar(true)
        .setDuration(StatusBarToast.DURATION_UNLIMITED)
        .setBackgroundColorResource(R.color.colorPrimaryDark)
        .build();
toast.show();

// somewhere else
toast.dismiss();
```

* Auto Hide Toast
```java
new StatusBarToast.Builder(this)
        .setText("Connecting")
        .setShowProgressBar(true)
        .setDuration(StatusBarToast.DURATION_LONG)
        .setBackgroundColorResource(R.color.colorPrimaryDark)
        .show();
```
