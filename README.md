# Android Multiple Activities Example

This is a simple Android application demonstrating how to work with multiple activities and pass data between them. The app consists of two activities, where the user inputs data in the first activity, and the second activity displays the passed data.

## Features
- Two separate activities for input and display.
- Passing data between activities using **Intent** and **Extras**.
- Basic UI handling with **EdgeToEdge** and **WindowInsetsCompat** for immersive system bars management.

## Technologies Used
- **Android Studio**
- **Java** 
- **Intent** for activity transitions and data transfer.
- **EdgeToEdge** and **WindowInsetsCompat** for immersive UI.

## Code Overview

### Main Components
1. **MainActivity**:
   - Contains an **EditText** field where the user can input a username.
   - When the user presses the button, the entered username is passed to the second activity (**MainActivity2**) using an **Intent**.
   - Method **changeActivity(View view)** is responsible for handling this transition.

2. **MainActivity2**:
   - Receives the username passed from **MainActivity** using **Intent** extras.
   - Displays the passed username in a **TextView**.
   - Includes a button to navigate back to **MainActivity** using **Intent**.
   - Method **changeScreen(View view)** is used to return to the first activity.

### Layout
- The first activity has an **EditText** for user input and a button to move to the second activity.
- The second activity has a **TextView** to display the passed data and a button to return to the first activity.

## Getting Started

### Prerequisites
To run this project, you need:
- Android Studio installed on your computer.
- Basic knowledge of Kotlin/Java and Android development.

### Installation

1. Clone the repository:
    ```bash
    git clone https://github.com/blueyes0101/MultipleActivitiesAndroid
    ```

2. Open the project in Android Studio.

3. Build and run the project on an emulator or physical device.

## Usage

1. In **MainActivity**, enter a username in the input field.
2. Press the button to move to **MainActivity2**. The entered username will be displayed.
3. Press the back button or the provided button in **MainActivity2** to return to **MainActivity**.

## Contributing
Feel free to contribute by opening issues or submitting pull requests.

## License
This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.
