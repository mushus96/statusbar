# statusbar
A simple QML example app that sets the status bar color on Android.

![screenshot](https://github.com/jpnurmi/statusbar/raw/master/example/statusbar.png)

Registering the QML type in C++:

    qmlRegisterType<StatusBar>("StatusBar", 0, 1, "StatusBar");

Example usage in QML:

    import StatusBar 0.1

    StatusBar {
        theme: StatusBar.Dark // or Material.Dark
        color: Material.color(Material.Indigo, Material.Shade700)
    }

*NOTE: Requires Android 5.0 Lollipop (API level 21) or later.*
