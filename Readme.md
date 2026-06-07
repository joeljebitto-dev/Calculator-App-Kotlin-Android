# Calculator App - Kotlin Android

A basic Android calculator app built with Kotlin and XML layouts. The app provides a simple calculator interface with number buttons, arithmetic operators, decimal input, clear functionality, and result evaluation.

## Features

* Native Android app built with Kotlin
* XML-based calculator UI
* Numeric input buttons from 0 to 9
* Addition operation
* Subtraction operation
* Multiplication operation
* Division operation
* Decimal point input
* Clear button
* Equals button for evaluating expressions
* Single-screen calculator layout
* AppCompat-based Android activity

## Tech Stack

* Kotlin
* Android SDK
* Android Gradle Plugin
* AppCompat
* Material Components
* ConstraintLayout
* XML layouts
* Gradle

## Project Structure

```text
Calculator-App-Kotlin-Android/
├── app/
│   ├── src/
│   │   └── main/
│   │       ├── java/com/joeljebitto/calculatorapp/
│   │       │   └── MainActivity.kt
│   │       ├── res/
│   │       │   ├── layout/
│   │       │   │   └── activity_main.xml
│   │       │   ├── values/
│   │       │   └── mipmap-*/
│   │       └── AndroidManifest.xml
│   └── build.gradle
├── build.gradle
├── settings.gradle
└── README.md
```

## How It Works

The calculator uses a `TextView` as the display and button click handlers in `MainActivity.kt`.

Main actions:

```text
Digit button      -> appends number to display
Operator button   -> appends arithmetic operator
Decimal button    -> appends decimal point when valid
Clear button      -> resets display
Equals button     -> evaluates the expression
```

Supported operators:

```text
+
-
*
/
```

The current implementation supports simple two-value arithmetic expressions such as:

```text
8+2
9-4
6*7
8/2
```

## Requirements

* Android Studio
* Android SDK
* JDK 8 or compatible Java toolchain
* Gradle / Android Gradle Plugin support

Project configuration:

```text
compileSdkVersion 30
minSdkVersion 16
targetSdkVersion 30
applicationId com.joeljebitto.calculatorapp
```

## Getting Started

Clone the repository:

```bash
git clone https://github.com/joeljebitto-dev/Calculator-App-Kotlin-Android.git
cd Calculator-App-Kotlin-Android
```

Open the project in Android Studio.

Then:

1. Let Android Studio sync Gradle.
2. Select an emulator or connected Android device.
3. Click **Run**.

## Running from Command Line

Build the debug APK:

```bash
./gradlew assembleDebug
```

On Windows:

```bash
gradlew.bat assembleDebug
```

Install on a connected device:

```bash
./gradlew installDebug
```

## App Flow

```text
Launch App
  ↓
Enter first number
  ↓
Choose operator
  ↓
Enter second number
  ↓
Tap equals
  ↓
View result
```

## Notes

* This is a beginner-friendly Android calculator project.
* The UI is implemented with classic Android XML views.
* The calculation logic is handled directly inside `MainActivity.kt`.
* The current evaluator is intentionally simple and is best suited for basic two-number arithmetic expressions.
* For production use, expression parsing and input validation should be improved.

## Future Improvements

* Add proper floating-point calculation support
* Add support for chained expressions
* Add percentage operation
* Add negative number handling improvements
* Add backspace/delete button
* Add division-by-zero user feedback
* Add better error handling for invalid input
* Replace deprecated Kotlin Android Extensions with View Binding
* Replace deprecated `jcenter()` repository usage
* Update Android Gradle Plugin and Kotlin versions
* Add unit tests for calculator logic
* Improve UI styling and responsiveness
* Add dark mode support

## Author

Built by [Joel Jebitto](https://github.com/joeljebitto-dev).
