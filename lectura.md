# Sendeiro · PMDM-UD2 · actividad 1 · leer y tocar

> Cada pregunta con vuestras palabras, de dos a cinco líneas. Las dos líneas del cambio van al final.

## Pregunta 1
**Dónde mirar:** `MainActivity.kt` · líneas 30 y 44 a 49

En todo el fichero no hay ninguna línea nuestra que llame a `onCreate`, ni a `onStart`, ni a ninguna de las siete. ¿Quién las llama, entonces? ¿Y qué quiere decir la palabra `override` delante de cada una?

**Respuesta:**

## Pregunta 2
**Dónde mirar:** `MainActivity.kt` · líneas 32 y 36 · `activity_main.xml`

`setContentView(R.layout.activity_main)` y `findViewById(R.id.campoNombre)`: ¿de qué fichero sale `activity_main`, y de qué línea de ese fichero sale `campoNombre`? ¿Qué pasaría si las tres líneas de `findViewById` estuvieran antes de `setContentView`?

**Respuesta:**

## Pregunta 3
**Dónde mirar:** `MainActivity.kt` · líneas 30 y 33

`Bundle?` lleva un interrogante. ¿Qué quiere decir? Según la línea que prepara la traza, ¿cuándo es nulo `savedInstanceState` y cuándo no?

**Respuesta:**

## Pregunta 4
**Dónde mirar:** `MainActivity.kt` · líneas 24 a 27

¿Por qué `campoNombre` es `lateinit` y no se le da valor en la misma línea en que se declara, como a `creaciones`?

**Respuesta:**

## Pregunta 5
**Dónde mirar:** Logcat, con el filtro `tag:CICLO`

Con el registro limpio, abrid la aplicación: ¿qué tres trazas salen, y en qué orden? Pulsad «inicio» (el círculo): ¿cuáles salen? Volved a la aplicación: ¿cuáles? ¿Ha vuelto a salir `onCreate`?

**Respuesta:**

## Pregunta 6
**Dónde mirar:** Logcat

Escribid algo en los dos campos. **Antes de girar**, anotad qué trazas esperáis. Girad el emulador. ¿Qué ha salido? ¿Qué dice ahora la traza de `onCreate`?

**Respuesta:**

## Pregunta 7
**Dónde mirar:** `MainActivity.kt` · línea 53 · los `android:id` del XML

Después del giro, lo que escribisteis en los dos campos sigue ahí, y en el código no hay ni una línea que lo guarde ni que lo recupere. ¿Quién lo ha hecho?

**Respuesta:**

## Pregunta 8
**Dónde mirar:** `MainActivity.kt` · líneas 27 y 40

Girad tres veces. El texto de abajo sigue diciendo «se ha creado 1 veces», y el registro demuestra que se ha creado cuatro. ¿Por qué no sube? Mirad dónde vive `creaciones`.

**Respuesta:**

## Pregunta 9
**Dónde mirar:** Terminal y Logcat

Con la aplicación delante, ejecutad `adb shell cmd uimode night yes` (modo oscuro) y después `adb shell settings put system font_scale 1.3` (letra más grande). ¿Qué trazas salen en cada caso? ¿A qué caso anterior se parecen?

**Respuesta:**

## Pregunta 10
**Dónde mirar:** Terminal y Logcat

Pulsad «inicio» y, con la aplicación en el fondo, ejecutad `adb shell am kill gal.sendeiro.rutas`. ¿Sale alguna traza? Volved a abrirla: ¿`onCreate` dice nulo o restaurado?, ¿siguen los campos escritos? Repetidlo con `adb shell am force-stop gal.sendeiro.rutas`. ¿Qué cambia? ¿Qué situación real representa cada orden?

**Respuesta:**

## Cambio de dos líneas (TOCAR)
**Línea 40** (`MainActivity.kt`):

**Línea 55** (`MainActivity.kt`):

**Capturas antes y después de girar:** (enlaces o nombres de fichero)
