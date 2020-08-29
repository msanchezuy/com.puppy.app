# com.puppy.app


Subo archivos relevantes para el desarrollo y para entender lo realizado, la configuracion de colores y otros valores seteados en la app
iconos usados y el codigo java de una actividad que despliega la imagen y se puede ver la seleccion de colores 


Configuracion de colores a utilizar

    "colorPrimary"      #0fe4ff
   
    "colorPrimaryDark"  #008f9e
   
    "colorAccent"      #FF5722
    
Tema utilizado para dar soporte a versiones anteriores  Material Design

    name="AppTheme" parent="Theme.AppCompat.Light.DarkActionBar"    
    

Captura de ide Android Studio 
    https://github.com/msanchezuy/com.puppy.app/blob/master/captura%20ide%20Android.png

Captura de la aplicacion ejecutando
    https://github.com/msanchezuy/com.puppy.app/blob/master/capturaPuppy.png

------------------------------------------------------------ res/values.xml

------------------------------------------------------------ res/strings.xml

------------------------------------------------------------ res/strings.xml

------------------------------------------------------------ res/layout


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
