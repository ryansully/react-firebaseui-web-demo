# FirebaseUI for web - React Auth demo

This project was bootstrapped with [Create React App](https://github.com/facebookincubator/create-react-app)
and modified to match the [Firebase UI for web - Auth demo](https://github.com/firebase/firebaseui-web/tree/master/demo).

## Prerequisite

You need to have created a Firebase Project in the
[Firebase Console](https://firebase.google.com/console/) as well as configured a web app.

## Installation

Install the firebase command line tool with `npm install -g firebase-tools` (See
[docs](https://firebase.google.com/docs/cli/#setup)).

Enable the Auth providers you would like to offer your users in the console, under
Auth > Sign-in methods.

Run:

```bash
git clone https://github.com/ryansully/react-firebaseui-web-demo.git
cd react-firebaseui-web-demo
```

This will clone the repository in the current directory.

If you want to be able to deploy the demo app to one of your own Firebase Hosting instance,
configure it using the following command:

```bash
firebase use --add
```

Select the project you have created in the prerequisite, and type in `default` or
any other name as the alias to use for this project.

Copy `.env` to `.env.local`:

```bash
cp .env .env.local
```

Modify `.env.local` with the configuration values from the Web snippet code found in the console (either by clicking
"Add Firebase to your web app" button in your Project overview, or clicking the "Web setup" button in the Auth page).

Copy `.env.local` to `.env.test.local`:

```bash
cp .env.local .env.test.local
```

## Deploy

To deploy the demo app, run the following command in the root directory:

```bash
npm start
```

This will compile all the files needed to run FirebaseUI, and start a server locally at http://localhost:3000.