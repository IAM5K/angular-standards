8. NgContent:

   Introduction:
   - The NgContent directive is used to project and pass content from a parent component to a child component's template.
   - It allows for flexible content insertion and composition within Angular components.

   Snippet:
   Parent Component Template:
   ```html
   <app-child>
     <h1>Content to be projected</h1>
   </app-child>
   ```

   Child Component Template:
   ```html
   <ng-content></ng-content>
   ```

   Explanation:
   - The `ng-content` directive is used within the child component's template to define the insertion point for projected content from the parent component.
   - Any content placed between the opening and closing tags of the child component in the parent template will be projected into the `ng-content` element in the child component.
   - The NgContent directive enables flexible composition and reusability of components, allowing for customizable content injection.

   Common Mistake:
   - A common mistake with `NgContent` is misunderstanding how it works and expecting the projected content to be automatically styled or modified within the child component. The child component is responsible for handling and rendering the projected content.
