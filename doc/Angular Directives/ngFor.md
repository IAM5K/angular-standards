2. NgFor:

   Introduction:
   - The NgFor directive repeats a template for each item in an iterable collection, allowing dynamic rendering of lists or tables.
   - It is commonly used to iterate over arrays or objects in your Angular templates and generate multiple instances of a template.

   Snippet:
   ```html
   <ul>
     <li *ngFor="let item of items; let i = index">{{ item }}</li>
   </ul>
   ```

   Explanation:
   - The `*ngFor` directive is used as an attribute on an element (e.g., `<li>`) to define the iteration over a collection.
   - The `items` is the iterable collection (array or object) you want to iterate over.
   - Inside the `*ngFor` directive, you can access each item using the `let item` syntax, and optionally, you can also get the index using `let i = index`.
   - The content within the element with `*ngFor` is duplicated for each item in the collection, resulting in multiple elements in the DOM.
   - Angular's change detection mechanism tracks changes in the collection, updating the DOM accordingly when items are added, removed, or modified.

   Common Mistake:
   - A common mistake with `NgFor` is forgetting to provide a unique key for each item when iterating over arrays. It is important to use a unique identifier (e.g., an ID) as the key to optimize performance and enable proper tracking of elements.


