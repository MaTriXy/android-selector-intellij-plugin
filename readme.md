[![Android Arsenal](https://img.shields.io/badge/Android%20Arsenal-android--selector--intellij--plugin-green.svg?style=flat)](https://android-arsenal.com/details/1/2342)


# android-selector-intellij-plugin ![icon](src/icons/icon@2x.png)
:art: Generate selectors for background drawable.

You can use `colorButtonNormal` simply,  
but make easily touch feedback of normal `View`s as well as `Button`s with this plugin.


## Usage
- Set your colors(in `res/values/colors.xml`).
```xml
<color name="colorPrimary">#519FE5</color>
<color name="colorPrimaryDark">#388AC6</color>
<color name="colorAccent">#FFFFFF</color>
```

- Select `New -> Android Selector(or Ctrl/Cmd + N)` on your `res` directory.  

![screenshot1](images/screenshot1.png)

- Select filename, color, pressed and pressed-v21 respectively.

![screenshot2](images/screenshot2.png)

> ripple drawable is generated in drawable-v21 directory.  
> normal drawable is generated in drawable directory.

- Use the drawable.
```xml
    <android.support.v7.widget.AppCompatButton
        android:layout_width="wrap_content"
        android:layout_height="wrap_content"
        android:layout_margin="16dp"
        android:background="@drawable/<GENERATED_DRAWABLE>"
        android:gravity="center"
        android:minWidth="100dp"
        android:text="pressed" />
```


## Demo

| Lollipop &gt; | Lollipop &lt;= |
|---------------|----------------|
| ![demo1][d1]  | ![demo2][d2]   |


## Dependency
- com.android.support:appcompat-v7:22.+


## License
MIT © [Jaewe Heo][importre]












[importre]: http://import.re
[d1]: images/demo1.png
[d2]: images/demo2.png
