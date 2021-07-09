# UniversalDemo

This project was generated with [Angular CLI](https://github.com/angular/angular-cli) version 12.1.1.

## Development server

Run `ng serve` for a dev server. Navigate to `http://localhost:4200/`. The app will automatically reload if you change any of the source files.

## Build

Run `ng build` to build the project. The build artifacts will be stored in the `dist/` directory.

## Installation and steps to repro the random loiading delay of approx 15 seconds when deployed to an Azure Windows or Linux App Service as Code 

Same problem is discussed here: https://docs.microsoft.com/en-us/answers/questions/308191/angular-universal-webb-app-with-ssr-randomly-slow.html

1. Have Node 12/14 installed.
2. Have angular cli installed: `npm i @angular/cli`
3. Get this code: `git clone https://github.com/juliansamuel/universal-demo.git`
4. Open the code in VS Code and run `npm --install` from the terminal to install the dependencies.
5. Run `ng start` to start the app in dev mode
6. Run `npm run build:ssr` to build the app deployment artifacts into the Dist folder
7. Deploy the build artifacts to an Azure Windows App Service.
8. Keep on hitting refresh until you randomly get a delay of between 15 & 16 seconds.
