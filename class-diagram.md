```mermaid
  classDiagram
  class Customer {
    +String name
    +login()
  }
  class Product {
    +String title
    +float price
  }
  class Order {
    +int orderId
    +createOrder()
  }
  Customer --> Order
  Order --> Product
