4. NgClass:

   Introduction:
   - The NgClass directive dynamically adds or removes CSS classes based on provided conditions or expressions.
   - It allows you to conditionally apply CSS classes to elements based on certain conditions in your Angular templates.

   Snippet:
   ```html
   <div [ngClass]="{ 'class-name': condition }">
     <!-- Content with dynamically applied CSS class -->
   </div>
   ```

   Explanation:
   - The `ngClass` directive is used as an attribute on an element to define the conditions for applying CSS classes.
   - Inside the `[ngClass]` attribute, you provide an object where the keys represent the class names, and the values represent the conditions for applying those classes.
   - When the `condition` evaluates to `true`, the associated CSS class (`class-name` in this example) is added to the element. If the condition is `false`, the class is removed.
   - Multiple classes and conditions can be provided within the object.
   - The NgClass directive allows for dynamic styling and class manipulation based on changing application state.

   Common Mistake:
   - A common mistake with `NgClass` is not using the object syntax correctly. It's important to ensure that the object structure is properly defined with class names as keys and condition expressions as values. Additionally, missing the single quotes around class names can cause errors.
