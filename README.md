# Live UTM Bus Tracking System 🚍

## Description
A real-time bus tracking system designed for **Universiti Teknologi Malaysia (UTM)**, utilizing two Android apps—one for drivers and one for students—to enhance transportation efficiency and user convenience.

---

## Technologies Used
- **Programming Language**: Java
- **Development Platform**: Android Studio
- **Database**: Firebase Firestore

---

## Key Features

### 🚐 **Driver App**
- **Sign Up & Log In**: Drivers can create accounts and log in to access the app.
- **Real-Time Location Sync**: Drivers can share their live location with the database with a single button press.
- **Data Storage**: Driver locations (latitude and longitude) are stored in the **Driver Collection** in Firestore, organized by bus number.

### 🎓 **Student App**
- **Sign Up & Log In**: Students can create accounts and log in to access the app.
- **Live Bus Locations**: Displays live bus locations on a map based on active drivers sharing their locations.
- **Lightweight Design**: The app contains only three pages for a clean, efficient user experience.

---

## Firestore Collections

- **Driver Collection**: Stores driver locations with bus numbers as subcollections, each containing documents with longitude and latitude data.
- **Driver Info Collection**: Contains driver details such as email, name, and password, with bus numbers as subcollections.
- **User Info Collection**: Holds student details including email, matric number, name, and password, with matric numbers as subcollections.

---

## Installation

1. Clone this repository to your local machine.
    ```bash
    git clone https://github.com/NightShade86/Live-UTM-Bus-Tracking-System.git
    ```
2. Open the project in **Android Studio**.
3. Set up **Firebase**:
    - Create a Firebase project on the [Firebase Console](https://console.firebase.google.com/).
    - Download the `google-services.json` file and add it to the `app/` directory.
    - Enable Firestore in the Firebase Console.

4. Sync the project with Gradle files.

---

## Setup

### Firebase Firestore Configuration:
- Create the following collections in Firebase:
  - **Driver Collection**: To store driver location data.
  - **Driver Info Collection**: To store driver information (email, name, etc.).
  - **User Info Collection**: To store student details (email, matric number, etc.).

### Firebase Authentication:
- Set up Firebase Authentication for both driver and student sign-ins.
- Use Firebase Authentication for managing user sessions (sign-up, sign-in).

---

## Usage

### 🚐 **Driver App**:
- **Sign In**: Drivers sign in to the app using their credentials.
- **Share Location**: Once logged in, drivers can press a button to sync their real-time location with the Firestore database, associated with their bus number.

### 🎓 **Student App**:
- **Sign In**: Students log in using their credentials.
- **View Bus Locations**: The student app shows a map with live bus locations, updated in real-time as drivers share their location.

---

## Contributing

1. **Fork** the repository.
2. Create a **new branch** for your feature.
    ```bash
    git checkout -b feature-name
    ```
3. **Commit** your changes.
    ```bash
    git commit -m "Add new feature"
    ```
4. **Push** to your branch.
    ```bash
    git push origin feature-name
    ```
5. Submit a **pull request** for review.

---

## Acknowledgements
- **Firebase**: For real-time database services.
- **Android Studio**: For development environment.

---

## Contact
- **Project Owner**: [Narres Khumar Jayakumaran](https://github.com/NightShade86)

---
