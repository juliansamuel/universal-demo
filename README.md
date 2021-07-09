# UniversalDemo

This project was generated with [Angular CLI](https://github.com/angular/angular-cli) version 12.1.1.

## Development server

Run `ng serve` for a dev server. Navigate to `http://localhost:4200/`. The app will automatically reload if you change any of the source files.

## Code scaffolding

Run `ng generate component component-name` to generate a new component. You can also use `ng generate directive|pipe|service|class|guard|interface|enum|module`.

## Build

Run `ng build` to build the project. The build artifacts will be stored in the `dist/` directory.

## Running unit tests

Run `ng test` to execute the unit tests via [Karma](https://karma-runner.github.io).

## Running end-to-end tests

Run `ng e2e` to execute the end-to-end tests via a platform of your choice. To use this command, you need to first add a package that implements end-to-end testing capabilities.

## Further help

To get more help on the Angular CLI use `ng help` or go check out the [Angular CLI Overview and Command Reference](https://angular.io/cli) page.

Installation and steps to repro this bug: https://docs.microsoft.com/en-us/answers/questions/308191/angular-universal-webb-app-with-ssr-randomly-slow.html
1. Have Node 12/14 installed.
2. Have angular cli installed: 'npm i @angular/cli'
3. Get this code: 'git clone https://github.com/juliansamuel/universal-demo.git'
4. Open the code in VS Code and run 'npm --install' from the terminal to install the dependencies.
5. Run 'ng start' to start the app in dev mode
6. Run 'npm run build:ssr' to build the app deployment arifacts into the Dist folder
7. Deploy the build artifacts to an Azure Windows App Service.
8. Keep on hitting refresh until you randomly get a delay of between 15 & 16 seconds.

