# Nuxt2.js Universal App with SSR via Firebase Functions and Firebase Hosting

Host a Nuxt2 Universal app or site by combining Nuxt2.js with Firebase Cloud Functions and Hosting.

[Live Preview](https://fir-630f1.firebaseapp.com)

---

## Pre-Setup: Before Installing Any Dependencies

1. Obtain a Firebase Project ID to use for this project. [See Overiew Here](#firebase-project-setup)

2. Inside this directory, locate the file `.setup-firebaserc` and replace the text `YOUR_FIREBASE_PROJECT_ID` with your Firebase Project ID.

---

## Setup

We will now get everything setup and deployed in 3 commands:

**Note:** _All of these commands are ran from the root directory_

1. Install Dependencies in all necessary directories and creates `.firebaserc` from `.setup-firebaserc`

```bash
yarn setup
```

### for Dev

```bash
yarn dev
```

### for Serve (Local server)

1. `yarn build`
2. `yarn pre:public`
3. `yarn serve`

### for deploy  (Firebase hosting)

1. `yarn build`
2. `yarn pre:public`
3. `yarn deploy`

---

### Firebase Project Setup

1. Create a Firebase Project using the [Firebase Console](https://console.firebase.google.com).

2. Obtain the Firebase Project ID

### Features

- Server-side rendering with Firebase Hosting combined with Firebase Functions
- Firebase Hosting as our CDN for our publicPath (See nuxt.config.js)

### Things to know...

- You must have the Firebase CLI installed. If you don't have it install it with `npm install -g firebase-tools` and then configure it with `firebase login`.

- If you have errors, make sure `firebase-tools` is up to date. I've experienced many problems that were resolved once I updated.

* The root directory has a package.json file with several scripts that will be used to optimize and ease getting started and the workflow

* ALL commands are ran from the root directory