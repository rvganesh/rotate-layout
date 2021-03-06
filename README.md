Rotate Layout
=============

Custom layout that can rotate it's view

[![Example](https://github.com/rongi/rotate-layout/raw/master/docs/screenshot2.png)](#Example)

Usage
=====

In your layout file add

```xml 
<com.github.rongi.rotate_layout.layout.RotateLayout
	app="http://schemas.android.com/apk/res-auto"
	android:layout_width="wrap_content"
	android:layout_height="wrap_content" >

	<YourLayoutHere
		android:layout_width="wrap_content"
		android:layout_height="wrap_content"
		app:layout_angle="90">	<!-- Specify rotate angle here -->
	</YourLayoutHere>
</com.github.rongi.rotate_layout.layout.RotateLayout>
```

Voila! Your layout will be rotated 90 degrees.

Download
========

```groovy
repositories {
    jcenter()
}

dependencies {
    compile 'rongi.rotate-layout:rotate-layout:1.0.1'
}
```

Features
========

1. Handles all touch events in correct way. You press the same button you touch!
2. Layout measures itself in a correct way. This means that if original view is 50x100, then 90 degree rotated it will measure itself as 100x50 and can fit in another layouts with this dimensions.
3. Supports only multiple of 90 angles atm. Still can be easily modifyed to support any angle.
