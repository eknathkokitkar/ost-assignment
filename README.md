<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0"/>
  <title>UML Diagram with Mermaid.js</title>
  <script type="module">
    import mermaid from 'https://cdn.jsdelivr.net/npm/mermaid@10/dist/mermaid.esm.min.mjs';
    mermaid.initialize({ startOnLoad: true });
  </script>
</head>
<body>
  <h2>UML Class Diagram Example</h2>
  <div class="mermaid">
    classDiagram
      class Animal {
        +String name
        +void makeSound()
      }

      class Dog {
        +void bark()
      }

      class Cat {
        +void meow()
      }

      Animal <|-- Dog
      Animal <|-- Cat
  </div>
</body>
</html>
