# AngularPractice

This project was generated with [Angular CLI](https://github.com/angular/angular-cli) version 13.2.2.

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

# Angular_Practice-

# To get Started in the CLI(terminal) install:
npm install -g @angular/cli 

# Create your new Angular project, add flags you will need: 
ng new (name of project) --style=scss --routing=true --skipTest (skipTest only if your not doing any testing)

# We are Using Bulma CSS Framework so in the CLI install Bulma:
npm install bulma --save 

# Go to styles.css and import Bulma:
@import '../node_modules/bulma/bilma.sass';

# In src folder create a new file for main styles:
touch main-styles.scss

# Go to bulma documentation :
visit site bulma.io go to Documentatiom->Customize->With Sass CLI go down to #6(Add your Own Bulma Style) and copy all the code except for the imports into main-styles.scss

# We will also need to import main-styles.scss into styles.scss :
@imports'./main-styles.scss';

# Serve application to the browser by typing in the CLI:
ng serve 

# Check to see if it is up and running on:
http://localhost:4200/

# Change Styling to your liking in main-styles.scss:

# Go to app->app.componenet.html:
delete all the placeholder content except for the routing (<router-outlet></router-outlet>)

# In a new CLI create pages:
ng generate component pages/NotesList 

# Go to the app->app.routing.module.ts to create path for NotesList:
const routes: Routes = [
    { path '', component: NotesListComponenet }
];

# Create a layout componenet:
ng generate component pages/MainLayout

# In order to get the @ViewChild and @ Input to work you have to go to tsconfig.json and add:
"noPropertyAccessFromIndexSignature": true,
    "noImplicitReturns": false,











