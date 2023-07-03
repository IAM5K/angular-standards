9. NgNonBindable:

   Introduction:
   - The NgNonBindable directive prevents Angular from parsing and interpolating the content within its element, treating it as static text.
   - It is useful when you want to display content that contains Angular-specific syntax without it being evaluated.

   Snippet:
   ```html
   <div ngNonBindable>
     {{ expression }}
   </div>
   ```

   Explanation:
   - The `ngNonBindable` directive is used as an attribute on an element (e.g., `<div>`) to indicate that the content within the element should be treated as static text and not parsed by Angular.
   - Angular will ignore any Angular-specific syntax, such as double curly braces `{{}}` or directives, within the element with `ngNonBindable`.
   - This directive is helpful when you need to display code snippets, Angular template examples, or content that should not be evaluated by Angular.

   Common Mistake:
   - A common mistake with `NgNonBindable` is using it unnecessarily. It's important to use this directive sparingly and only when needed, as it can impact performance by preventing Angular from optimizing and evaluating the content.
