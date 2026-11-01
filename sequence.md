```mermaid
graph LR
  %% بازیگرها
  Customer((مشتری))
  Admin((مدیر مزون))

  %% موارد استفاده مشتری
  UC1(مرور محصولات)
  UC2(جستجو و فیلتر)
  UC3(مشاهده جزئیات محصول)
  UC4(افزودن به سبد خرید)
  UC5(ثبت و پرداخت سفارش)
  UC6(پیگیری سفارش)

  %% موارد استفاده مدیر
  UC7(مدیریت محصولات)
  UC8(مشاهده گزارش فروش)
  UC9(مدیریت سفارش‌ها)

  %% ارتباطات مشتری
  Customer --> UC1
  Customer --> UC2
  Customer --> UC3
  Customer --> UC4
  Customer --> UC5
  Customer --> UC6

  %% ارتباطات مدیر
  Admin --> UC7
  Admin --> UC8
  Admin --> UC9
