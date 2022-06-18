# Install, Configure and Integrate Firebase Emulator Suite
## **How to install**
#### Before installing the Emulator Suite you will need:-

- Node.js version 8.0 or higher.

- Java JDK version 11 or higher.

#### To install the Emulator Suite:
- Install the Firebase CLI. If you don't already have the Firebase CLI installed, install it (https://firebase.google.com/docs/cli#install-cli-windows). 
  You will need CLI version 8.14.0 or higher to use the Emulator Suite.
- You can install the Firebase CLI using npm (the Node Package Manager). Note that you will need to install Node.js and npm. Installing Node.js should install npm as well.

```
npm install -g firebase-tools
```
  
- You can check which version you have installed using the following command in theterminal.
  
```
firebase --version
```
    
- After Installation Initialize the firebase Using
  
```
firebase init
```

-  Now Set up the Emulator Suite. The Below Command Provides you some emultors Like, Authentication,Firestore, Realtime Database,Storage DataBase etc.
   Select the emulatorsyou needed
    
```
firebase init emulators
``` 
## **How to Configure** 

#### Configure Emulator Suite:-

- You can optionally configure the emulators' network ports and path to Security Rules definitions in the firebase.json file:
    - Change emulator ports by running `firebase init emulators` or by editing `firebase.json` manually.
    
Note:-(***Recommended***)If you don't configure these settings, the emulators will listen on their default ports, and the Cloud Firestore, Realtime Database and Cloud Storage 
        emulators will run with open data security.
#### Port Configuration - These are the Default Ports Provided you can change them while initializing(if needed)

| Emulator             | Ports|
| ---                  | ---  |
| Authentication       | 9099 |
| Emulator Suite UI    | 9099 |
| Cloud Functions      | 9099 |
| Realtime Database    | 9099 |
| Cloud Firestore      | 8080 |
| Cloud Storage        | 8080 |
| Firebase Hosting     | 5000 |
| Pub/Sub              | 8085 |

- The emulators will take Security Rules configuration from the database, firestore and storage configuration keys in `firebase.json`.

## Integrate With your CI System.

- Installation and configuration of the Emulator Suite with containers in a typical CI setup is straightforward.

- To Start the Emulators:-

```
firebase emulators:start
```
- You can check/open Emulator suite at `localhost:4000` nby default
- You need to run `firebase emulators:start` irst and then run `npm start` inorder to run the codelabz webpage  

