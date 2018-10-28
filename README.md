StatusBarToast
==============

Displaying text on your StatusBar!(Telegram-X like)


![demo](demo/demo.gif)


## Usage
* Unlimited Duration Toast:
```java
// create a toast and show it
StatusBarToast toast = new StatusBarToast.Builder(this)
        .setText("Connecting")
        .setShowProgressBar(true)
        .setDuration(StatusBarToast.DURATION_UNLIMITED)
        .setBackgroundColorResource(R.color.colorPrimaryDark);
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
