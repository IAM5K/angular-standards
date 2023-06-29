# AngularStandards

This project was generated with [Angular CLI](https://github.com/angular/angular-cli) version 16.1.2.

## Development server

Run `ng serve` for a dev server. Navigate to `http://localhost:4200/`. The application will automatically reload if you change any of the source files.

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

## Response⁠
Provided resource have some inappropriate rule sets and must be modified.

### Warnings should not be
1. Default log for failure of 
```console
  /home/macaw/mwd/Angular/angular-standards/src/main.ts
    7:17  warning  Unexpected console statement  no-console
```
2. 
```console
/home/macaw/mwd/Angular/angular-standards/src/app/app-routing.module.ts
   8:28  error  Missing trailing comma                              comma-dangle
   9:4   error  Missing trailing comma                              comma-dangle
  14:26  error  Missing trailing comma                              comma-dangle
  16:1   error  Prefer default export on a file with single export  import/prefer-default-export
```
3. 
```console
/home/macaw/mwd/Angular/angular-standards/src/app/app.component.spec.ts
  19:6  error  Strings must use singlequote  quotes
```
4. 
