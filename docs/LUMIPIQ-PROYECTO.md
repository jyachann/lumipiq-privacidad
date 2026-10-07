# Lumipiq — información del proyecto

Actualizado: 7 de octubre de 2026.

## Identidad
- Nombre: Lumipiq.
- Identificador Android de publicación: `com.labschann.lumipiq`.
- Identificador debug: `com.labschann.lumipiq.debug`.
- Namespace interno Kotlin: `com.example.lumipiq`; es independiente del identificador de instalación.
- Política pública: https://jyachann.github.io/lumipiq-privacidad/
- Contacto de privacidad: LABSCHANN@GMAIL.COM.

## Aplicación
Aplicación Android nativa en Kotlin y Jetpack Compose para organizar y buscar imágenes y capturas elegidas por el usuario.
Incluye importación selectiva, copia privada, deduplicación, OCR local, etiquetas visuales automáticas, búsqueda en español e inglés, favoritos, archivo, colecciones, notas y correcciones manuales.
El reconocimiento visual usa un catálogo finito; no garantiza detectar cualquier objeto.
La estimación opcional de edad aparente propone bebé, niño, joven, adulto o resultados inciertos. No identifica personas ni verifica edades. Los recortes de rostros se procesan en memoria.
El botón Importar capturas está arriba en Biblioteca, antes del buscador.

## Privacidad
La privacidad del usuario es la prioridad del proyecto.
Las imágenes, texto OCR, búsquedas, notas y grupos de edad se procesan localmente y no se envían para análisis ni publicidad.
Incluye bloqueo, protección de capturas de pantalla, respaldo cifrado y restauración, y migraciones de base de datos sin borrado destructivo.
ML Kit y Google Mobile Ads pueden tratar datos técnicos según la política.
Ajustes → Privacidad abre la política pública; hay resumen sin conexión y contacto por correo.
La página de privacidad no incluye el nombre personal del propietario ni identificadores técnicos de la aplicación.

## Monetización implementada
- Banner de Google AdMob y consentimiento UMP.
- Premium de compra única sin anuncios; producto esperado: `lumipiq_premium_lifetime`.
- Debug usa anuncios de prueba y compras simuladas, sin cobros ni ingresos.
- Compras y anuncios reales requieren configuración y validación del propietario.

## Validación
El 3 de octubre de 2026 pasaron 25 pruebas unitarias; lintDebug tuvo cero errores y 43 advertencias.
El APK de esa fecha se instaló y arrancó en Redmi Note 14 sin cierre inmediato.
Las pruebas instrumentadas completas y parte de la interacción automatizada no se ejecutaron por restricciones del teléfono. Quedan pruebas de aceptación, accesibilidad, bibliotecas grandes, respaldo/restauración desde la interfaz y precisión con imágenes variadas.
El 7 de octubre se verificaron correctamente processDebugMainManifest y processReleaseMainManifest con los nuevos identificadores y sus FileProvider.
Los resultados del APK anterior corresponden al identificador anterior; no equivalen a una validación completa de la nueva instalación.
Cambiar el identificador crea una instalación separada. Para transferir la biblioteca anterior se debe exportar un respaldo cifrado y restaurarlo en la nueva.

## Entrega y límites autorizados
El entregable es el proyecto Android Studio y el ZIP llamado `lumipiq version 1-android studio.zip`.
El propietario genera el AAB, configura Google Play Console y AdMob y realiza las subidas y publicaciones.
El asistente debe limitarse a desarrollar, corregir, verificar y entregar el proyecto. No debe generar el AAB ni realizar acciones en las consolas.
Las claves de firma, contraseñas y datos personales de usuarios deben permanecer fuera del repositorio y del ZIP.
Esta ficha guarda información del proyecto; no constituye un respaldo del código fuente completo ni de los modelos.

## Tecnología
Kotlin, Jetpack Compose, Room, ML Kit, modelo local de edad FairFace modificado y ONNX, Google Mobile Ads, UMP y Play Billing.
Entorno de compilación verificado: JDK 21.0.11, Gradle 8.14.3, SDK 36, Build Tools 35.0.0.
