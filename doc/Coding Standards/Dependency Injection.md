5. Dependency Injection:
   - Dependency injection (DI) is a fundamental concept in Angular that promotes loose coupling and reusability by allowing components, services, and other dependencies to be injected rather than explicitly instantiated.

   - Use dependency injection for services and other dependencies instead of creating instances manually.

   - To inject a service into a component, you can specify it as a constructor parameter and Angular will handle the injection for you. For example:

     ```typescript
     import { Component } from '@angular/core';
     import { UserService } from './user.service';

     @Component({
       selector: 'app-user',
       templateUrl: './user.component.html',
       styleUrls: ['./user.component.css']
     })
     export class UserComponent {
       constructor(private userService: UserService) { }

       // ...
     }
     ```

     In this example, the `UserService` is injected into the `UserComponent` via the constructor.

   - Provide dependencies at the component level whenever possible to limit their scope. This improves encapsulation and allows for easier testing and maintenance.

     ```typescript
     import { Component, OnInit } from '@angular/core';
     import { DataService } from './data.service';

     @Component({
       selector: 'app-my-component',
       templateUrl: './my-component.component.html',
       styleUrls: ['./my-component.component.css'],
       providers: [DataService]
     })
     export class MyComponent implements OnInit {
       constructor(private dataService: DataService) { }

       ngOnInit(): void {
         // Use the dataService
       }

       // ...
     }
     ```

     In this example, the `DataService` is provided at the component level by including it in the `providers` array of the component's metadata. This ensures that each instance of the `MyComponent` component has its own instance of the `DataService`.

By leveraging dependency injection, you can achieve decoupling, maintainability, and testability in your Angular code.
