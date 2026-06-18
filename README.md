# Aplicación de Calculadora

Una aplicación de calculadora sencilla y funcional desarrollada utilizando el framework Flutter. Permite realizar operaciones matemáticas básicas con una interfaz de usuario moderna y oscura.

## Tabla de Contenidos
- [Tecnologías Utilizadas](#tecnologías-utilizadas)
- [Características](#características)
- [Requisitos](#requisitos)
- [Instalación](#instalación)
- [Configuración](#configuración)
- [Cómo Ejecutar el Proyecto](#cómo-ejecutar-el-proyecto)
- [Ejemplos de Uso](#ejemplos-de-uso)
- [Estructura de Carpetas](#estructura-de-carpetas)
- [Explicación de Módulos](#explicación-de-módulos)
- [Solución de Problemas](#solución-de-problemas)
- [Notas Adicionales](#notas-adicionales)

## Tecnologías Utilizadas
- **Flutter**: Framework para el desarrollo de aplicaciones multiplataforma.
- **Dart**: Lenguaje de programación utilizado por Flutter.
- **Google Fonts**: Paquete para la implementación de tipografías personalizadas (Rubik).
- **Math Expressions**: Librería para el parseo y evaluación de expresiones matemáticas.

## Características
- **Operaciones Básicas**: Suma, resta, multiplicación y división.
- **Cálculo de Porcentajes**: Soporte para la operación de porcentaje.
- **Gestión de Pantalla**:
    - Visualización de la expresión actual.
    - Historial inmediato de la última operación realizada.
- **Interfaz Moderna**: Diseño con modo oscuro y botones personalizados.
- **Multiplataforma**: Compatible con Android, iOS, Web, Windows, macOS y Linux.

## Requisitos
Para ejecutar este proyecto, necesitas tener instalado:
- [Flutter SDK](https://docs.flutter.dev/get-started/install) (Versión >= 2.18.2 < 3.0.0)
- [Dart SDK](https://dart.dev/get-started/sdk)
- Un editor de código (recomendado: Visual Studio Code o Android Studio)
- Un emulador o dispositivo físico configurado para pruebas.

## Instalación
1. Clona el repositorio:
   ```bash
   git clone https://github.com/tenshi98/calculadora_app.git
   ```
2. Navega al directorio del proyecto:
   ```bash
   cd calculadora_app
   ```
3. Instala las dependencias:
   ```bash
   flutter pub get
   ```

## Configuración
El proyecto no requiere configuraciones adicionales de variables de entorno. Asegúrate de que tu entorno de Flutter esté correctamente configurado ejecutando:
```bash
flutter doctor
```

## Cómo Ejecutar el Proyecto
Para iniciar la aplicación en el dispositivo o emulador seleccionado:
```bash
flutter run
```

## Ejemplos de Uso
1. **Suma Simple**: Presiona `5` $\rightarrow$ `+` $\rightarrow$ `3` $\rightarrow$ `=`. El resultado `8` se mostrará en pantalla.
2. **Limpiar Pantalla**:
    - Presiona `C` para borrar la expresión actual.
    - Presiona `AC` para borrar tanto la expresión como el historial.
3. **Operaciones Complejas**: Ingresa una expresión como `10 * 5 / 2` y presiona `=` para obtener el resultado.

## Estructura de Carpetas
```text
calculadora_app-main/
├── android/               # Archivos de configuración para Android
├── ios/                   # Archivos de configuración para iOS
├── linux/                 # Archivos de configuración para Linux
├── macos/                 # Archivos de configuración para macOS
├── web/                   # Archivos de configuración para Web
├── windows/               # Archivos de configuración para Windows
├── lib/                   # Código fuente de la aplicación
│   ├── main.dart          # Punto de entrada y lógica principal
│   └── widgets/           # Componentes de UI reutilizables
│       └── CalcButton.dart # Definición del botón de la calculadora
├── test/                  # Pruebas automatizadas
├── analysis_options.yaml  # Reglas de análisis de código
└── pubspec.yaml           # Dependencias y metadatos del proyecto
```

## Explicación de Módulos
- **`main.dart`**: Contiene la clase `CalcApp`, que gestiona el estado de la calculadora (expresión e historial) y define la estructura visual mediante un `Scaffold` con una columna de botones.
- **`CalcButton.dart`**: Un widget personalizado (`StatelessWidget`) que estandariza el diseño de los botones, permitiendo configurar el color de fondo, el texto y la función de callback al hacer clic.
- **`pubspec.yaml`**: Gestiona las dependencias externas como `google_fonts` y `math_expressions`, esenciales para la estética y el funcionamiento matemático de la app.

## Solución de Problemas
- **Error de dependencias**: Si encuentras errores al ejecutar, prueba limpiar el proyecto:
  ```bash
  flutter clean
  flutter pub get
  ```
- **Dispositivo no detectado**: Verifica la conexión del dispositivo o el estado del emulador con:
  ```bash
  flutter devices
  ```

## Notas Adicionales
Esta aplicación fue creada como un ejercicio educativo para implementar el manejo de estados básicos en Flutter y la integración de librerías de evaluación matemática.
