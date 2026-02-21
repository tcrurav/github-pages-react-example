# Upload React Project to Github pages

This project is there as an example on how to upload a dist project to Github pages.

This is the result in https://

Here are the instructions I have followed: https://gist.github.com/sc1f/12ad9c209a87678b49f4507abf458138

## Getting Started

Read the links in the acknowlegements section bellow to get an idea about Firebase.

The final result looks like this, i.e. a simple CRUD without update.

![Screenshot](/screenshots/screenshot-1.png)

## Prerequisites

You need a working environment with:
* [Git](https://git-scm.com) - You can install it from https://git-scm.com/downloads.
* [Node.js](https://nodejs.org) - Install node.js from https://nodejs.org/es/download/. It's advisable to install the LTS version.

## General Installation instructions

Create a Firebase project and create a Real-time database in that project.

Import some fake data in your database to start up. Here you have some:
[Some data to import to Firebase](/docs/reactbikes-default-rtdb-export.json)

Clone this project:

```
git clone https://github.com/tcrurav/ReactFirebaseSimpleExample.git
```

Now install all dependencies.

```
cd ReactFirebaseSimpleExample
npm install
```

Modify the constant firebaseConfig in file src/firebase.js so that it contains the corresponding configuration data of your project. Here you have an example:

```
const firebaseConfig = {
  apiKey: "AIzaSyBL83k7hQlfWWYFsjV4qIqAwFyTNV3Csds",
  authDomain: "reactbikes.firebaseapp.com",
  databaseURL: "https://reactbikes-default-rtdb.europe-west1.firebasedatabase.app",
  projectId: "reactbikes",
  storageBucket: "reactbikes.appspot.com",
  messagingSenderId: "120470000752",
  appId: "1:120470000752:web:e3ce490552fcc96fe750b5"
};
```

And finally run the project.

```
cd ReactFirebaseSimpleExample
npm start
```

Enjoy!!!


## Built With

* [Visual Studio Code](https://code.visualstudio.com/) - The Editor used in this project
* [Node.js](https://nodejs.org/) - Node.js® is a JavaScript runtime built on Chrome's V8 JavaScript engine.
* [firebase real-time database](https://firebase.google.com/docs/database/web/read-and-write?hl=es-419) - Read and Write data in the web.
* [Create React App](https://create-react-app.dev/) - Set up a modern web app by running one command

## Acknowledgments

* https://gist.github.com/sc1f/12ad9c209a87678b49f4507abf458138. Pushing the contents of your dist folder to gh-pages.
* https://gist.github.com/PurpleBooth/109311bb0361f32d87a2. A very complete template for README.md files.