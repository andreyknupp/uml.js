# UML.js

Convert JSON to UML using Graphviz Dot.

## Why?

A programmatic way to generate *Class Diagrams*

## TODO

- More diagrams (like use case)
- A "*language*"
- Support for default values on properties
- Option to export *pretty* dot files

### How I think this language would be

**CoffeeScript way** (my favorite)

```nohl
class Animal
  - name : string

  + Animal()
  + setName(name : string) : void
  + getName() : string

class Mammal < Animal

class Fish < Animal

class Dolphin < Mammal, Fish
```

**Ruby way**

```nohl
class Animal
  - name : string

  + Animal()
  + setName(name : string) : void
  + getName() : string
end

class Mammal < Animal
end

class Fish < Animal
end

class Dolphin < Mammal, Fish
end
```
