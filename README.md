# NotesApp - A Secure Note-Taking Android Application

A simple, secure, and intuitive note-taking application for Android, built with Java and Firebase.

## 🚀 Project Objective

The main goal of this project is to provide a secure and reliable mobile application where users can create, manage, and store their personal notes. The application uses Google's Firebase for user authentication and cloud storage, ensuring that user data is safe and synced in real-time.

## ✨ Key Features

-   **Secure User Authentication**: Users can create an account and log in securely using Firebase Authentication (Email & Password).
-   **Create & Manage Notes**: Once logged in, users can easily create, view, edit, and update their notes.
-   **Cloud Storage**: All notes are stored securely in the cloud using **Firebase Firestore**. This means your notes are safe even if you lose your device.
-   **Real-time Sync**: Notes are updated instantly across your sessions.
-   **Clean & Simple UI**: The user interface is built following Material Design principles, making it easy and intuitive to use.

## 🛠️ Technology Stack

-   **Language**: **Java**
-   **Platform**: **Android**
-   **Database**: **Firebase Firestore** (for storing notes)
-   **Authentication**: **Firebase Authentication** (for user login/signup)
-   **IDE**: Android Studio
-   **UI**: XML with Material Design Components
-   **Core Libraries**:
    -   AndroidX Libraries (AppCompat, RecyclerView)
    -   Firebase UI for Firestore (to easily display data in lists)

## ⚙️ Application Workflow

1.  **Launch**: When the app starts, it checks if a user is already logged in.
2.  **Authentication**:
    -   If the user is **not logged in**, they are shown a **Login Screen**. They can either log in or navigate to the **Sign-Up Screen** to create a new account.
    -   If the user is **already logged in**, they are taken directly to the main notes screen.
3.  **Main Screen (All Notes)**:
    -   After a successful login, the user sees a list of all their previously created notes.
    -   A **Floating Action Button (+)** allows the user to create a new note.
4.  **Create/Edit Note**:
    -   Users can write a title and content for their note and save it.
    -   Tapping on an existing note allows the user to view its details and edit it.
5.  **Data Persistence**:
    -   All notes are saved to Firebase Firestore under the current user's unique ID, ensuring privacy and security.
6.  **Logout**:
    -   Users can log out from the options menu, which will take them back to the Login Screen.

## 📂 Project Structure

-   `MainActivity.java`: Handles user login.
-   `signup.java`: Handles new user registration.
-   `notesactivity.java`: The main screen that displays a list of all notes using a `RecyclerView`.
-   `createnote.java`: The screen for creating a new note.
-   `editnoteactivity.java`: The screen for editing an existing note.
-   `notedetails.java`: The screen to view the full details of a single note.
-   `firebasemodel.java`: A simple model class to represent a note (title and content).
-   `NoteViewHolder`: A `ViewHolder` for the `RecyclerView` adapter to display each note item.

## 🚀 How to Run the Project

1.  **Clone the repository**:
    
