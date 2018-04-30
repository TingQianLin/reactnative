# Auth

A very basic authentication demo app use [Firebase](https://firebase.google.com).

## Firebase Setup

1. Go to [Firebase](https://firebase.google.com), if you don't have an account, create one.
2. Click **GO TO CONSOLE** and create new project.
3. Click **DEVELOP** on the left side then select **Authentication**.
4. Click **SIGN-IN METHOD** and enable **Email/Password**.
5. Run `npm install --save firebase` to install firebase library.
6. Click **WEB SETUP** on the top-right corner to get the config.
7. `firebase.initialzeApp()` to initialize the firebase with the config.

The firebase config looks like below shows:

```JavaScript
const firebaseConfig = {
  apiKey: 'Automantically_-Generated7Random_ApiKey',
  authDomain: 'yourproject.firebaseapp.com',
  databaseURL: 'https://yourproject.firebaseio.com',
  projectId: 'yourproject',
  storageBucket: 'yourproject.appspot.com',
  messagingSenderId: '0123456789ID'
}
```