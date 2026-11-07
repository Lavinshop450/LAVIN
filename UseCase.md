
```mermaid
graph LR
    %% بازیگرها
    Customer((مشتری))
    Admin((مدیر مزون))

    %% موارد استفاده مشتری
    Customer --> UC1(مرور محصولات)
    Customer --> UC2(جستجو و فیلتر)
    Customer --> UC3(مشاهده جزئیات)
    Customer --> UC4(افزودن به سبد خرید)
    Customer --> UC5(پرداخت سفارش)
    Customer --> UC6(پیگیری سفارش)

    %% موارد استفاده مدیر
    Admin --> UC7(مدیریت محصولات)
    Admin --> UC8(گزارش فروش)
    Admin --> UC9(مدیریت سفارش‌ها)
'''
