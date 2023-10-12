# Santander Dev Week - 2023
Java RESTful API criada para a Santander Dev Week 2023

## Diagrama de classes

```mermaid

classDiagram
  class User {
    - String name
    - Account account
    - Feature[] features
    - Card card
    - News[] news
  }

  class Account {
    - String number
    - String agency
    - float balance
    - float limit
  }

  class Feature {
    - String icon
    - String description
  }

  class Card {
    - String number
    - float limit
  }

  class News {
    - String icon
    - String description
  }

  User "1" *-- "1" Account : has
  User "1" *-- "*" Feature : has
  User "1" *-- "1" Card : has
  User "1" *-- "*" News : has




```
