
```text
```mermaid
graph LR
  Customer((مشتری))
  Admin((مدیر مزون))

  UC1(مرور محصولات)
  UC2(جستجو و فیلتر)
  UC3(مشاهده جزئیات محصول)
  UC4(افزودن به سبد خرید)
  UC5(ثبت و پرداخت سفارش)
  UC6(پیگیری سفارش)

  UC7(مدیریت محصولات)
  UC8(مشاهده گزارش فروش)
  UC9(مدیریت سفارش‌ها)

  Customer --> UC1
  Customer --> UC2
  Customer --> UC3
  Customer --> UC4
  Customer --> UC5
  Customer --> UC6

  Admin --> UC7
  Admin --> UC8
  Admin --> UC9
