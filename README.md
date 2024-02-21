# learning-mermaid
Learning mermaid

[Including diagrams in your Markdown files with Mermaid](https://github.blog/2022-02-14-include-diagrams-markdown-files-mermaid/)

# Mermaid in markdown github

## Graph
```mermaid
    graph TD;
        A-->B;
        A-->C;
        B-->D;
        C-->D;
```

## Sequence Diagrams
```mermaid
sequenceDiagram
    Alice->>John: Hello John, how are you?
    John-->>Alice: Great!
    Alice-)John: see you later!
```

## Class Diagram
```mermaid
---
title: Animal example
---
classDiagram
    note "From Duck till Zebra"
    Animal <|-- Duck
    note for Duck"can fly\ncan swim\n can dive\ncan help in debugging"
    Animal <|-- Fish
    Animal <|-- Zebra
    Animal : +int age
    Animal : +String gender
    Animal: +isMammal()
    Animal: +mate()
    class Duck {
        +String beakColor
        +swim()
        +quack()
    }

    class Fish{
        -int sizeInFeet
        -canEat()
    }

    class Zebra{
        +bool is_wild
        +run()
    }
```
