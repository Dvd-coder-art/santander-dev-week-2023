## SANTANDER DEV WEEK
Java RESTful API criada para a Santander Dev Week

## Diagrama de Classes

```mermaid
classDiagram
    class User {
        +String name
        +Account account
        +List~Feature~ features
        +Card card
        +List~News~ news
    }

    class Account {
        +String number
        +String agency
        +double balance
        +double limit
    }

    class Feature {
        +String icon
        +String description
    }

    class Card {
        +String number
        +double limit
    }

    class News {
        +String icon
        +String description
    }

    User --> Account
    User --> "0..*" Feature
    User --> Card
    User --> "0..*" News
```


 Esse Projeto esta com falha na conexão com o Railwai/Postgree usando intelij, funcinou usando eclipse.

