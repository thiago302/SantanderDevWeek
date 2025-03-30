#Santander Dev Week
Java RESTfull API criada para a Santander dev week.


## diagrama de classes

'''mermaid
classDiagram
    class User {
        +String name
        +Account account
        +Feature[] features
        +Card card
        +News[] news
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
        +String Number
        +double Limit
    }

    class News {
        +String icon
        +String description
    }

    User *--> Account
    User *--> Feature : has
    User *--> Card
    User *--> News : has

'''
