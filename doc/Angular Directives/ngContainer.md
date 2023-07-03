10. NgContainer:

   Introduction:
   - The NgContainer directive provides a way to group and manage multiple Angular structural directives in a single container element.
   - It is commonly used when you need to apply multiple structural directives to a single element.

   Snippet:
   ```html
   <ng-container *ngIf="condition">
     <!-- Content to be displayed when condition is true -->
   </ng-container>
   ```

   Explanation:
   - The `ng-container` is a logical element provided by Angular that doesn't render any markup in the final DOM.
   - It serves as a container for other elements and directives.
   - By using the `ng-container` along with structural directives like `*ngIf` or `*ngFor`, you can apply these directives to a group of elements without adding an additional wrapper element to the DOM.
   - The NgContainer directive helps to improve code readability and maintainability by grouping directives together.

   Common Mistake:
   - A common mistake with `NgContainer` is using it without any structural directives. The `ng-container` is typically used in conjunction with structural directives to provide functionality and should not be used alone without any directive inside.

  Example:
  
  Here's an example that combines NgContent, NgContainer, and NgTemplateOutlet:

  Parent Component Template:
  ```html
  <app-container-example>
    <ng-container *ngTemplateOutlet="customTemplate; context: { name: 'John' }"></ng-container>
  </app-container-example>

  <ng-template #customTemplate let-name="name">
    <div>
      Welcome, {{ name }}!
      <ng-content></ng-content>
    </div>
  </ng-template>
  ```

  Child Component Template (app-container-example):
  ```html
  <ng-content></ng-content>
  ```

  Explanation:
  - In the parent component template, we have a custom template defined using the `ng-template` element with the reference `#customTemplate`.
  - The template includes a `<div>` element with the greeting message "Welcome, {{ name }}!" where `name` is a context variable.
  - Inside the template, we use the `ng-content` directive to project any content passed from the parent component.
  - In the parent component, we use the `app-container-example` component and provide the custom template using `ng-template-outlet`.
  - We pass the context object `{ name: 'John' }` to the template, where `name` is assigned the value `'John'`.
  - The content within the `ng-container` in the parent component is projected into the `<ng-content>` in the custom template of the child component.
  - This allows for dynamic rendering of content with customized greetings.

  By going through this example, we have covered the usage of NgContent, NgContainer, and NgTemplateOutlet directives.

