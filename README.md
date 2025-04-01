Sandander Dev Week 2025
Java RESTful criada para a Sandander Dev Week 2025. este projeto é de 2023, mas trouxemos para o bootcamp da avanade. o Decola Tech 2025


## Diagrama de Classes

```mermaid
classDiagram
    class User {
        +string name
        +Account account
        +Feature[] features
        +Card card
        +News news
    }

    class Account {
        +string number
        +string agency
        +float balance
        +float limit
    }

    class Feature {
        +string icon
        +string description
    }

    class Card {
        +string number
        +float limit
    }

    class News {
        +string icon
        +string description
    }

    User "1" -- "1" Account : has
    User "1" -- "0..*" Feature : has
    User "1" -- "1" Card : has
    User "1" -- "1" News : has
```
