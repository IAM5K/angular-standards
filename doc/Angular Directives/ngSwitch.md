3. NgSwitch:

   Introduction:
   - The NgSwitch directive conditionally renders content based on multiple expressions using a switch-case-like syntax.
   - It allows you to define different templates based on the value of a specific expression.

   Snippet:
   ```html
   <div [ngSwitch]="condition">
     <div *ngSwitchCase="'value1'">
       <!-- Content to be displayed when condition is 'value1' -->
     </div>
     <div *ngSwitchCase="'value2'">
       <!-- Content to be displayed when condition is 'value2' -->
     </div>
     <div *ngSwitchDefault>
       <!-- Default content when condition does not match any case -->
     </div>
   </div>
   ```

   Explanation:
   - The `ngSwitch` directive is used as an attribute on a container element (e.g., `<div>`) to define the expression to be evaluated.
   - Inside the container, you can use `*ngSwitchCase` to define templates for specific cases and `*ngSwitchDefault` for the default case.
   - When the `condition` matches a case expression, the corresponding template is rendered. If none of the cases match, the default template is rendered.
   - The NgSwitch directive simplifies the conditional rendering of different templates based on values, providing a more concise syntax compared to multiple `*ngIf` conditions.

   Common Mistake:
   - A common mistake with `NgSwitch` is forgetting to use the single quotes (`'`) around case values. It is important to enclose the values in quotes to ensure proper comparison and matching.
