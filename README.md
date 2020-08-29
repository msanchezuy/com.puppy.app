# com.puppy.app


Subo archivos relevantes para el desarrollo y para entender lo realizado, la configuracion de colores y otros valores seteados en la app
iconos usados y el codigo java de una actividad que despliega la imagen y se puede ver la seleccion de colores 


Configuracion de colores a utilizar

   "colorPrimary"      #0fe4ff
   "colorPrimaryDark"  #008f9e
    "colorAccent"      #FF5722


------------------------------------------------------------ res/values.xml
<?xml version="1.0" encoding="utf-8"?>
<resources>
    <color name="colorPrimary">#0fe4ff</color>
    <color name="colorPrimaryDark">#008f9e</color>
    <color name="colorAccent">#FF5722</color>
</resources>
------------------------------------------------------------ res/strings.xml
<resources>
    <string name="app_name">Puppy.App</string>
    <string name="puppylogo">puppylogo</string>
</resources>
------------------------------------------------------------ res/strings.xml
<resources>
    <!-- Base application theme. -->
    <style name="AppTheme" parent="Theme.AppCompat.Light.DarkActionBar">
        <!-- Customize your theme here. -->
        <item name="colorPrimary">@color/colorPrimary</item>
        <item name="colorPrimaryDark">@color/colorPrimaryDark</item>
        <item name="colorAccent">@color/colorAccent</item>
    </style>
</resources>
------------------------------------------------------------ res/layout
<?xml version="1.0" encoding="utf-8"?>
<androidx.constraintlayout.widget.ConstraintLayout xmlns:android="http://schemas.android.com/apk/res/android"
    xmlns:app="http://schemas.android.com/apk/res-auto"
    xmlns:tools="http://schemas.android.com/tools"
    android:layout_width="match_parent"
    android:layout_height="match_parent"
    android:background="#6BC9F4"
    tools:context=".MainActivity">
    <RelativeLayout
        android:id="@+id/relativeLayout1"
        android:layout_width="match_parent"
        android:layout_height="match_parent" >
        <ImageView
            android:id="@+id/picture"
            app:srcCompat="@drawable/puppybig"
            android:layout_width="wrap_content"
            android:layout_height="wrap_content"
            android:layout_alignParentBottom="true"
            android:contentDescription="@string/puppylogo"  />

    </RelativeLayout>
</androidx.constraintlayout.widget.ConstraintLayout>
---------------------------------------------------------- MainActivity.java
package com.puppy.app;

import androidx.appcompat.app.AppCompatActivity;

import android.os.Bundle;

public class MainActivity extends AppCompatActivity {

    @Override
    protected void onCreate(Bundle savedInstanceState) {
        super.onCreate(savedInstanceState);
        setContentView(R.layout.activity_main);
    }
}
