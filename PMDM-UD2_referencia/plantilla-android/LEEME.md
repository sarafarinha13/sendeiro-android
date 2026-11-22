# Sendeiro · PMDM-UD2 · actividad 1

Aquí hay **dos ficheros**, no un proyecto Android entero. El proyecto lo crea el asistente de Android
Studio, que lo deja compilando con las versiones de hoy, y encima se ponen estos dos. Diez minutos:

1. Android Studio → *File → New → New Project → Empty Views Activity*.
   Nombre `Sendeiro`, paquete `gal.sendeiro.rutas`, lenguaje Kotlin, `minSdk` el del perfil de
   dispositivos de la unidad 1.
2. Ejecutar una vez en el emulador: tiene que abrirse una pantalla casi vacía. Ya hay proyecto.
3. Sustituir `app/src/main/java/gal/sendeiro/rutas/MainActivity.kt` por el de esta carpeta.
4. Sustituir `app/src/main/res/layout/activity_main.xml` por el de esta carpeta.
5. Ejecutar otra vez: dos campos y el texto «Esta pantalla se ha creado 1 veces».
6. Ver las trazas. En Android Studio, ventana *Logcat*, con el filtro `tag:CICLO`. O en una terminal:

       adb logcat -c && adb logcat -s CICLO:D

Qué trae `MainActivity.kt`: una traza en cada una de las siete llamadas del ciclo de vida, dos campos
y un contador de las veces que se ha creado la pantalla. Los dos campos sobreviven al giro sin que el
código haga nada. El contador no: ese es el cambio de la actividad (los dos sitios marcados `TOCAR`).

Si se sube a un repositorio, el `.gitignore` que genera el asistente ya deja fuera `local.properties`
y `build/`.
