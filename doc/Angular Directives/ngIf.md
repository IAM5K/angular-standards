1. NgIf:

   Introduction:
   - The NgIf directive conditionally adds or removes elements from the DOM based on the provided expression.
   - It is commonly used to conditionally display or hide elements based on certain conditions in your Angular templates.

   Snippet:
   ```html
   <div *ngIf="condition">
     <!-- Content to be displayed when the condition is true -->
   </div>
   ```

   Explanation:
   - The `*ngIf` directive is used as an attribute on a container element (e.g., `<div>`) to define the condition for rendering the enclosed content.
   - When the `condition` expression evaluates to `true`, the content within the element is added to the DOM. If the condition is `false`, the content is removed from the DOM.
   - This directive has a significant impact on the DOM as elements are dynamically added or removed, affecting the layout and rendering of the page.
  
   Common Mistake:
   - A common mistake with `NgIf` is forgetting to add a container element. It is important to wrap the elements with a container element (e.g., a `<div>`) to avoid errors and maintain the correct DOM structure.
