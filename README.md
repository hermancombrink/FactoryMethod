-- Use the Factory Method when you don’t know beforehand the exact types and dependencies of the objects your code should work with.
-- The Factory Method separates product construction code from the code that actually uses the product. Therefore it’s easier to extend the product construction code independently from the rest of the code.
-- Use the Factory Method when you want to provide users of your library or framework with a way to extend its internal components.

## Pros

- You avoid tight coupling between the creator and the concrete products.
- **Single Responsibility Principle:** You can move the product creation code into one place in the program, making the code easier to support.
- **Open/Closed Principle:** You can introduce new types of products into the program without breaking existing client code.

## Cons

- The code may become more complicated since you need to introduce a lot of new subclasses to implement the pattern.
- The best case scenario is when you’re introducing the pattern into an existing hierarchy of creator classes.
