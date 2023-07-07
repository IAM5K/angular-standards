# Angular Standards
## Purpose
The purpose of this repository is to provide a set of standards and best practices for developing angular applications that should be followed to write quality and safe code. 

It is still under progess so things will keep on adding.
We have `doc` folder that contain collection of concepts and questions & answers that can help you to prepare for interview, exam or expanding knowledge. You can add it to watch list and give it a star if it helps. Contents are refrenced from multiple sources (primarily Angular Documentation).

***Note:** There are known duplicates in `docs/security` that needs to be sanitized. It will be cleaned soon.

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
1. Default log for failure of Angular packages, we should not remove this.
```console
  /home/macaw/mwd/Angular/angular-standards/src/main.ts
    7:17  warning  Unexpected console statement  no-console
```
2. Trailing comma should not be recomended, in strict lintings/ json. Trailing comman throws an error as it is not required but still there.
```console
/home/macaw/mwd/Angular/angular-standards/src/app/app-routing.module.ts
   8:28  error  Missing trailing comma                     comma-dangle
   9:4   error  Missing trailing comma                     comma-dangle
  14:26  error  Missing trailing comma                     comma-dangle
```
3. In case of dynamic string value allication angular generated files use **` `` `**. 
```console
/home/macaw/mwd/Angular/angular-standards/src/app/app.component.spec.ts
  19:6  error  Strings must use singlequote  quotes
```
4. This error is raising error on base architecture template of angular.
```console
/home/macaw/mwd/Angular/angular-standards/src/app/app.module.ts
  14:1  error  Prefer default export on a file with single export  import/prefer-default-export
```

## Supportive Links
1. https://github.com/OsmosysSoftware/dev-standards/blob/main/coding-standards/angular.md
2. https://angular.io/guide/styleguide
3. https://github.com/airbnb/javascript/tree/master/packages/eslint-config-airbnb-base
4. https://osmosysasia-my.sharepoint.com/:x:/g/personal/rajkumar_p_osmosys_co/EcSnDteKjvhGr-6jgmdIRDEBVsW7hjqfXs7o8NwUTea7oQ?e=QQAVfR
5. https://eslint.org/docs/latest/rules/spaced-comment#rule-details
6. https://angular.io/guide/security
7. 
