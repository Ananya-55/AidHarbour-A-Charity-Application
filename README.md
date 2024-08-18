# AidHarbour - A Charity Application

## Overview

AidHarbour is a charity application designed to streamline charitable activities and enhance donation processes. Developed using Kotlin, Android Studio, and Firebase, AidHarbour connects donors with homeless shelters and NGOs, facilitating seamless and impactful contributions. By integrating Google Maps API and Firebase, AidHarbour offers a user-friendly platform with real-time updates, transparent donation tracking, and intuitive map-based navigation.

## Features

- User Dashboard: View real-time updates, donation history, and personalized recommendations.
- History Activity: Access detailed records of past donations, including photos and donated goods.
- Map Integration: Locate nearby shelters and donation points using Google Maps API.
- Firebase Integration: Manage user profiles, donation history, and real-time updates securely.


## Setup Instructions

### Prerequisites

- **Android Studio**: Ensure you have Android Studio installed. Download it from [here](https://developer.android.com/studio).
- **Firebase Account**: Create a Firebase project at [Firebase Console](https://console.firebase.google.com/).

### Clone the Repository

### Setup the Firebase

#### Create a Firebase Project:

1. Go to [Firebase Console](https://console.firebase.google.com/).
2. Click on "Add project" and follow the prompts to create a new project.

#### Add Your Android App to Firebase:

1. In the Firebase Console, select your project.
2. Click on the Android icon to add a new Android app.
3. Register your app with the package name `com.example.aidharbour`.
4. Download the `google-services.json` file and place it in the `app` directory of your project.

#### Enable Firebase Services:

1. Go to the Firebase Console and select your project.
2. Navigate to the "Authentication" section and enable the necessary sign-in methods.
3. Navigate to the "Realtime Database" section and create a new database.

## Configure the Project

### Update `build.gradle` Files:

In the **root-level** `build.gradle` file, add the Google services classpath:

```gradle
buildscript {
    dependencies {
        classpath 'com.google.gms:google-services:4.3.14'
    }
}

In the app-level build.gradle file, apply the Google services plugin and add Firebase dependencies:

```gradle
apply plugin: 'com.google.gms.google-services'
dependencies {
    implementation 'com.google.firebase:firebase-auth:23.5.0'
    implementation 'com.google.firebase:firebase-database:20.2.0'
    implementation 'com.google.android.gms:play-services-maps:18.1.0'
}

### Sync the project:

Click "Sync Now" in Android Studio to synchronize your project with Gradle files.

## Build and Run the Application




