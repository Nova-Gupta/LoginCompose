# Login Form using Jetpack Compose (Kotlin)

This project demonstrates a **Login Form built using Jetpack Compose in Kotlin** without using any XML layout files.  
The entire UI is implemented using **Composable functions** inside a single `MainActivity.kt` file.

---

## Features

- Username validation (minimum **4 characters**)
- Password validation (**more than 6 characters**)
- **Remember Me** checkbox
- **Additional Information** switch
- **Login button**
- Displays a **Toast message** on successful login
- Uses **Explicit Intent**
- UI screen switching handled using **Composable functions**
- No XML layouts used (Jetpack Compose only)

---

## Technologies Used

- **Kotlin**
- **Jetpack Compose**
- **Android Studio**
- **Material 3 Components**

---

## Project Structure


All UI screens (`LoginScreen` and `HomeScreen`) are created as **Composable functions** inside `MainActivity.kt`.

---

## How It Works

1. User enters username and password.
2. Input validation is performed:
   - Username ≥ 4 characters
   - Password > 6 characters
3. User can select:
   - Remember Me (Checkbox)
   - Additional Information (Switch)
4. On clicking the **Login** button:
   - If validation passes:
     - A **Toast message** is shown: `Login Successful`
     - An **Explicit Intent** is triggered
     - User is navigated to the Home screen
   - If validation fails:
     - An error Toast message is displayed

---

## Navigation Logic

- Explicit Intent is used to restart the same activity.
- Intent data is checked in `onCreate()` to decide which Composable screen to display:
  - `LoginScreen`
  - `HomeScreen`

---

## 📖 Learning Outcome

- Understanding Jetpack Compose UI
- Using state management with `remember` and `mutableStateOf`
- Handling input validation
- Using Toast messages in Compose
- Implementing Explicit Intent without multiple activities
- Creating multi-screen UI using Composables only
