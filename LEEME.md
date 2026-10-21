# Refrigeración Pro — proyecto Android inicial

Aplicación Android nativa en Java, con interfaz oscura azul/negro y almacenamiento local SQLite. No requiere permisos de Internet ni crea cuentas.

## Incluye
- Inicio con resumen de registros y utilidad.
- Registro de diagnósticos, síntomas y mediciones.
- Registro local de clientes/equipos.
- Cotizaciones con cálculo de costos y utilidad estimada.
- Historial con opción de eliminar registros.

## Generar el APK usando solo tu celular (GitHub Actions)
Este proyecto incluye un flujo de compilación en la nube. No necesitas instalar Android Studio ni compilar en el teléfono.

1. Descarga el ZIP y extráelo con un administrador de archivos.
2. En el navegador, entra a https://github.com y crea una cuenta o inicia sesión.
3. Crea un repositorio nuevo. Puedes llamarlo `RefrigeracionPro`; para una primera prueba, elige **Public** y no agregues README, licencia ni `.gitignore` (así la carga es más sencilla).
4. Sube el contenido de la carpeta `RefrigeracionPro` al repositorio, incluyendo la carpeta oculta `.github/workflows/android.yml`. Si la web móvil no permite subir carpetas, abre la vista de escritorio del navegador o crea los archivos/carpetas desde la web.
5. En el repositorio, abre **Actions** y selecciona **Build Refrigeracion Pro APK**. Pulsa **Run workflow**.
6. Espera a que termine correctamente. En la ejecución, baja hasta **Artifacts** y descarga `RefrigeracionPro-debug-apk`.
7. Extrae ese ZIP en tu teléfono y abre `app-debug.apk`. Android puede pedir permiso para instalar desde ese navegador/administrador de archivos; habilítalo solo si verificaste que descargaste tu propio artefacto de GitHub Actions.

La compilación usa GitHub Actions, Java 17 y Gradle 8.9. El APK de depuración es para pruebas, no está firmado para publicar en Play Store.
