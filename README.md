## Android Studio
### como mostrar un hola mundo
- Crear un nuevo proyecto con la plantilla **"empty activity"**
- Dale un nombre al proyecto. Ej: *"Holamundo"* y despues apreta *finish*
- Cuando el  proyecto se creo vas a la carpeta **activity_main.xml**
- Copia y pega:
~~~
  <?xml version="1.0" encoding="utf-8"?>
<RelativeLayout xmlns:android="http://schemas.android.com/apk/res/android"
    xmlns:tools="http://schemas.android.com/tools"
    android:layout_width="match_parent"
    android:layout_height="match_parent"
    tools:context=".MainActivity">

    <TextView
        android:id="@+id/textView"
        android:layout_width="wrap_content"
        android:layout_height="wrap_content"
        android:text="Hola Mundo!"
        android:layout_centerInParent="true"
        android:textSize="24sp"
        android:textColor="@android:color/black"/>
</RelativeLayout>
~~~
- Abris el archivo **"MainActivity.kt"** que esta en **"app/src/main/java/tu_paquete/MainActivity.kt."**
- Tiene que estar asi:
~~~
package tu_paquete

import androidx.appcompat.app.AppCompatActivity
import android.os.Bundle

class MainActivity : AppCompatActivity() {
    override fun onCreate(savedInstanceState: Bundle?) {
        super.onCreate(savedInstanceState)
        setContentView(R.layout.activity_main)
    }
}
~~~
- Conecta un dispositivo o emulador y apreta *run* (triangulo verde)
- selecciona tu dispositivo y clickea **OK**
## Listo!
