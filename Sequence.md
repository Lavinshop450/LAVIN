```mermaid
sequenceDiagram
  actor Customer as مشتری
  participant Site as سایت لاوین
  Customer->>Site: انتخاب محصول
  Customer->>Site: ثبت سفارش
  Site-->>Customer: پرداخت موفق
