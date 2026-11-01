```mermaid
sequenceDiagram
  actor Customer as مشتری
  participant UI as سایت لاوین
  participant DB as دیتابیس
  participant Gateway as درگاه پرداخت

  Customer->>UI: انتخاب محصول و افزودن به سبد
  UI->>DB: بررسی موجودی محصول
  DB-->>UI: موجودی تایید شد
  Customer->>UI: درخواست پرداخت
  UI->>Gateway: ارسال اطلاعات پرداخت
  Gateway-->>UI: پرداخت موفق
  UI->>DB: ثبت سفارش جدید
  DB-->>UI: شماره سفارش صادر شد
  UI-->>Customer: نمایش پیام موفقیت و کد رهگیری
