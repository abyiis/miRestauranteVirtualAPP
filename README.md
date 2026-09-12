# MyRestauranteVirtual

[![Android SDK](https://img.shields.io/badge/Platform-Android-green?style=for-the-badge&logo=android)](https://developer.android.com/)
[![Language](https://img.shields.io/badge/Language-Java-orange?style=for-the-badge&logo=java)](https://www.java.com/)
[![Gradle Kotlin DSL](https://img.shields.io/badge/Gradle-Kotlin_DSL-purple?style=for-the-badge&logo=gradle)](https://gradle.org/)

**MyRestauranteVirtual** es una aplicación móvil nativa para Android diseñada para brindar una experiencia digital completa a los clientes de un restaurante. Desarrollada por estudiantes e investigadores de la Universidad Pontificia Bolivariana (UPB), la aplicación permite consultar el menú interactivo por categorías, visualizar detalles de productos, explorar promociones, realizar reservas de mesa y localizar las sedes del restaurante.

---

## Características Principales

- **Menú Virtual Interactivo:** Explora las opciones gastronómicas divididas por categorías:
  - **Entradas**
  - **Platos Fuertes**
  - **Bebidas**
  - **Licores**
  - **Postres**
- **Promociones Especiales:** Sección dedicada para ver los descuentos y ofertas vigentes.
- **Detalle del Producto:** Visualización detallada de los elementos del menú.
- **Gestión de Reservas:** Formulario interactivo para agendar mesas en el restaurante.
- **Localización de Sedes:** Consulta la ubicación y detalles de las sedes disponibles.

---

## Tecnologías Utilizadas

- **Lenguaje:** Java 
- **SDK Objetivo:** Android SDK
- **Gestor de Dependencias y Compilación:** Gradle con Kotlin DSL (`build.gradle.kts`)
- **Arquitectura e Interfaz:** Android Views (XML Layouts, Activities)
- **ID de Paquete:** `com.upb.myrestaurantevirtual`
- **Institución:** Universidad Pontificia Bolivariana (UPB)

---

## Estructura del Proyecto

```text
Aplicacion-master/
├── app/
│   ├── build.gradle.kts           # Configuración de compilación del módulo (Kotlin DSL)
│   ├── proguard-rules.pro         # Reglas de ofuscación y optimización
│   └── src/
│       ├── main/
│       │   ├── AndroidManifest.xml # Declaración de componentes y permisos
│       │   ├── java/com/upb/myrestaurantevirtual/
│       │   │   ├── MainActivity.java           # Pantalla principal / bienvenida
│       │   │   ├── MenuActivity.java           # Categorías del menú
│       │   │   ├── EntradasActivity.java       # Menú de entradas
│       │   │   ├── PlatosFuertesActivity.java  # Menú de platos fuertes
│       │   │   ├── BebidasActivity.java        # Menú de bebidas
│       │   │   ├── LicoresActivity.java        # Menú de licores
│       │   │   ├── PostresActivity.java        # Menú de postres
│       │   │   ├── ProductoActivity.java       # Detalle de un producto individual
│       │   │   ├── PromocionActivity.java      # Sección de promociones
│       │   │   ├── ReservaActivity.java        # Formulario de reservas
│       │   │   └── SedeActivity.java           # Información de sedes
│       │   └── res/
│       │       ├── drawable/       # Imágenes, iconos y recursos gráficos
│       │       ├── layout/         # Diseños de pantallas en XML
│       │       ├── mipmap-*/       # Iconos de la aplicación
│       │       └── values/         # Colores, cadenas de texto (strings) y temas
├── gradle/
│   ├── libs.versions.toml          # Catálogo de versiones de dependencias
│   └── wrapper/                    # Envoltorio de Gradle
├── build.gradle.kts                # Configuración de Gradle a nivel de proyecto
├── settings.gradle.kts             # Ajustes e inclusión de módulos
└── gradlew / gradlew.bat           # Scripts de ejecución de Gradle
```

---

## Requisitos e Instalación

### Prerrequisitos

- **Android Studio** (versión Iguana | 2023.2.1 o superior recomendada).
- **JDK 17** o superior.
- Dispositivo físico Android con depuración USB habilitada o un emulador (Android 7.0 / API 24 o superior).

### Pasos para ejecutar localmente

1. **Clonar el repositorio:**
   ```bash
   git clone https://github.com/tu-usuario/Aplicacion.git
   cd Aplicacion-master
   ```

2. **Abrir en Android Studio:**
   - Abre Android Studio.
   - Selecciona **Open** y navega hasta la carpeta `Aplicacion-master`.
   - Espera a que Gradle ejecute la sincronización (`Gradle Sync`).

3. **Compilar y Ejecutar:**
   - Selecciona tu dispositivo de destino (Emulador o Dispositivo Físico).
   - Presiona el botón **Run** (ó `Shift + F10`).

4. **Compilar APK mediante consola:**
   ```bash
   # En Linux / macOS
   ./gradlew assembleDebug

   # En Windows
   gradlew.bat assembleDebug
   ```
   *El APK generado se ubicará en `app/build/outputs/apk/debug/`.*

---

## Licencia y Créditos

Proyecto desarrollado con fines académicos e institucionales en la **Universidad Pontificia Bolivariana (UPB)**. Todos los derechos reservados.
