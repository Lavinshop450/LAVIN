```mermaid
classDiagram
  class Customer {
    +String name
    +String phone
    +String email
    +register()
    +login()
  }

  class Product {
    +String title
    +String category
    +String size
    +String color
    +float price
    +int stock
    +addProduct()
    +updateStock()
  }

  class Order {
    +int orderId
    +Date date
    +float totalPrice
    +String status
    +createOrder()
    +trackOrder()
  }

  class Cart {
    +addItem(Product)
    +removeItem(Product)
    +calculateTotal()
  }

  Customer "1" --> "*" Order : places
  Customer "1" --> "1" Cart : has
  Cart "1" --> "*" Product : contains
  Order "*" --> "*" Product : includes
