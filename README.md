# Santander Dev Week 
Java RESTful API criada para a Santander dev week 

## Diagrama de classes 

 ```mermaid
classDiagram
  class User {
    +String name
    +Account account
    +Features[] features
    +Card card
    +News[] news
  }

  class Account {
    +String Number
    +String Agency
    +float Balance
    +float Limit
  }

  class Features {
    +String icon
    +String description
  }

  class Card {
    +String Number
    +float Limit
  }

  class News {
    +String icon
    +String description
  }

  User "1" *-- "1" Account
  User "1" *-- "1...N" Features
  User "1"  *-- "1" Card
  User "1" *-- "1...N" News
```
