# Start up Emulators
#### The Emulators can be start You can start emulators to run until manually terminated based on the user preferences:-
**NOTE**:- To Run the webpage First you need to start Emulators to load the Database You  start the emulators in different mode.
### **Initial Start** 
- To Start all the emulators at a time we can use the command `firebase emulators:start` 
### **Start Particular Emulator** 
- By including `--only` flag will  Limit which emulators to start. Supply a comma-separated list of emulator names, specifying one or more of 'auth', 'database', 'firestore', 'functions', 'hosting', or 'pubsub'. 
- Example:-`firebase emulators:start --only firestore` will start the firestore emulator only.

# Import Data to Emulators
- To import data to emulators there should be a pre-exisiting data file which contains data about respective Emulators.
- we can get the data file by exporting it fron the database emualators(if your are using for first time the must be created).
- To import data we can use the command in terminal while starting the emulators `firebase emulators:start --import file_name`, the file name can be any thing if the file exist in the project folder then the data from it is imported to the firebase local emulators.
-  
