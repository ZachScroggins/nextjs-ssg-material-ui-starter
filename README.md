# Next.js SSG Material-UI Firebase Starter

Starter kit for [Next.js](https://nextjs.org/) SSG app with [Material-UI](https://material-ui.com/) and [Firebase Hosting](https://firebase.google.com/products/hosting)

## How to use

Download the starter [or clone the repo](https://github.com/mui-org/material-ui)

```sh
curl https://codeload.github.com/mui-org/material-ui/tar.gz/master | tar -xz --strip=2  material-ui-master/examples/nextjs
cd nextjs
```

Install dependencies

```sh
npm install
```

### Configuration

#### Material-UI

1. [Customize the Material-UI theme](https://material-ui.com/customization/theming/) in `src/theme.js`

   Theme and Palette Generators

   - [create-mui-theme](https://react-theming.github.io/create-mui-theme/): Is an online tool for creating Material-UI themes via Material Design Color Tool

   - [material-ui-theme-editor](https://in-your-saas.github.io/material-ui-theme-editor/): Is an online tool for creating Material-UI themes via Material Design Color Tool

   * [Material palette generator](https://material.io/inline-tools/color/): Is an online tool for creating Material-UI themes via Material Design Color Tool

#### Firebase

2. [Create a Firebase project](https://console.firebase.google.com/u/0/) and add a new app

   Set up Firebase Hosting for your web app during Registration

3. Initialize Firebase in `firebase/initFirebase.js` by importing the necessary Firebase modules and replacing the clientCredentials with your Firebase Configuration (found in "Project settings")... To use you just have to import it anywhere in the app

### Deploy

1. Install the Firebase CLI

   ```sh
   npm install -g firebase-tools
   ```

2. Login to Firebase with CLI

   ```sh
   firebase login
   ```

3. Configure Hosting with CLI

   ```sh
   firebase init
   ```

   Specify "out" as your public root directory

4. Deploy with CLI
   ```sh
   firebase deploy
   ```
   Your app is now available at
   - projectID.web.app
   - projectID.firebaseapp.com
