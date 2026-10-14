## Git Demo 1

Hello world demo. This is a simple demonstration of how to use Git for version control. In this demo, we will cover the basics of creating a repository, making commits, and pushing changes to a remote repository.

classDiagram
    class Animal
    Vehicle <|-- Car

classDiagram
  class Customer {
    +String name
    +String email
  }
  class Order {
    +String id
    +Date placedAt
    +total() Money
  }
  class LineItem {
    +int quantity
  }
  class Payment {
    <<interface>>
    +authorise() bool
  }
  Customer "1" --> "*" Order : places
  Order "1" *-- "*" LineItem : contains
  Order --> Payment : settled by