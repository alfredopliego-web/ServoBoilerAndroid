SERVO BOILER WIFI - ANDROID
Proyecto base para Android Studio (Kotlin).

IMPORTANTE
- Este ZIP contiene el proyecto Android. No es una APK compilada.
- El archivo .ino se carga por separado al ESP32.
- Firmware esperado: AP WiFi ServoBoiler, clave Boiler123, dirección usual 192.168.4.1.
- La app manda GET /set?angle=0..180.
- Se requiere Android Studio y conexión a internet para descargar dependencias.

CREAR APK
1. Descomprime ServoBoilerAndroid.zip en una computadora.
2. Abre Android Studio > Open y selecciona la carpeta ServoBoilerAndroid.
3. Espera que termine Gradle Sync.
4. Menú Build > Build Bundle(s) / APK(s) > Build APK(s).
5. Android Studio mostrará la ubicación de app-debug.apk.
6. Pasa la APK al celular e instálala. Si Android pregunta, permite instalar desde esa fuente.

USO
1. Programa el ESP32 con ServoBoilerWiFi.ino.
2. Alimenta el SG90 con una fuente regulada de 5 V adecuada; conecta GND de la fuente y GND del ESP32 juntos.
3. En el celular, conéctate a WiFi ServoBoiler (clave Boiler123).
4. Si Android dice que no hay internet, elige mantener la conexión.
5. Abre la app, usa Probar conexión y mueve el deslizador.

Seguridad:
No uses este prototipo para reemplazar controles o dispositivos de seguridad del boiler.
Prueba el movimiento del servo sin acoplarlo primero. Confirma que los topes mecánicos
y el sentido de giro son correctos antes de conectar a la perilla.
