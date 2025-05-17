# firebase-raspi
This project demonstrates how to connect an Adafruit DHT11 temperature and humidity sensor to Firebase using Python.

## Installation

1.  **Install necessary Python libraries:**
    Open your terminal and run the following commands:
    pip install Adafruit_DHT
    pip install firebase_admin

## Firebase Setup

1.  **Go to Firebase Console:** Navigate to the [Firebase Console](https://console.firebase.google.com/).
2.  **Create a new project:** Follow the steps to create a new Firebase project.
3.  **Click on your project name.**
4.  **Build -> Realtime Database -> Create database.**
5.  **Choose a location for your Realtime Database.**
6.  **Set up security rules:** For initial testing, you can start in locked mode, but for production, configure appropriate security rules.
7.  **Generate new private key:**
    * Go to **Project overview** (gear icon next to "Project Overview" in the left sidebar) -> **Service accounts**.
    * Click on **Generate new private key**. This will download a JSON file containing your service account credentials. **Keep this file secure.**

## Project Configuration

1.  **Go to your terminal.**
2.  **Navigate to the project directory:**
   
    ls /home/pi/Downloads/
   
3.  **Copy the downloaded JSON file** (your Firebase service account key) into your project directory.
4.  **Save your Python code** (likely with a `.py` extension) in the same directory.

## Running the Code

1.  **Go to your terminal.**
2.  **Navigate to your project directory.**
3.  **Run the Python script:**
   
    python your_script_name.py
   
    (Replace `your_script_name.py` with the actual name of your Python file).

## Notes

* Ensure your Raspberry Pi (or the device running the code) has internet connectivity to communicate with Firebase.
* The Python script will likely read data from the DHT11 sensor and send it to your Firebase Realtime Database.
* Refer to the Firebase Realtime Database in the Firebase Console to see the data being updated.
* Remember to configure appropriate security rules for your Firebase Realtime Database for production environments.




