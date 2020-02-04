# Deploying an Angular/React App to Firebase Hosting
### 1) Build a production-ready set of assets for your app in the dist folder
```
ng build --prod
```
### 2) Create a Firebase account
```
https://firebase.google.com/
```
### 3) Install the Firebase CLI
```
sudo npm install -g firebase-tools
```
### 4) Login to your Firebase account
```
firebase login
```
### 5) Initialize firebase instance in working directory
```
firebase init
```
### 6) Select Hosting via space and press Enter
```
? Which Firebase CLI features do you want to set up for this folder? Press Space to select features, then Enter to confirm
 your choices. (Press <space> to select, <a> to toggle all, <i> to invert selection)
 ◯ Database: Deploy Firebase Realtime Database Rules
 ◯ Firestore: Deploy rules and create indexes for Firestore
 ◯ Functions: Configure and deploy Cloud Functions
❯◯ Hosting: Configure and deploy Firebase Hosting sites
 ◯ Storage: Deploy Cloud Storage security rules
 ◯ Emulators: Set up local emulators for Firebase features
```
### 7) Select create new project and press Enter
```
? Please select an option: 
  Use an existing project 
❯ Create a new project 
  Add Firebase to an existing Google Cloud Platform project 
  Don't set up a default project 
```
### 8) Enter unique project id and project name
```
i  If you want to create a project in a Google Cloud organization or folder, please use "firebase projects:create" instead
, and return to this command when you've created the project.
? Please specify a unique project id (warning: cannot be modified afterward) [6-30 characters]:
 xyz123
? What would you like to call your project? (defaults to your project ID) xyz
```
### 9) Change public folder to dist/your-app-name when asked (it defaults to public).
### 10) Configure as single page app? Yes
### 11) If firebase asks to overwrite your index.html file, just say NO.
### 12) deploy your production-ready app to Firebase Hosting
```
firebase deploy
```
### 13) Your app is now deployed and you can launch it with
```
firebase open
```
