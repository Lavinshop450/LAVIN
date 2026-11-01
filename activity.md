
```text
```mermaid
flowchart TD
  Start([ورود به سایت]) --> Browse[مرور محصولات]
  Browse --> Select[انتخاب محصول]
  Select --> CheckSize{راهنمای سایز نیاز داری؟}
  CheckSize -- بله --> ViewSize[دیدن جدول سایز]
  ViewSize --> AddCart[افزودن به سبد خرید]
  CheckSize -- خیر --> AddCart
  AddCart --> Login{وارد شده‌ای؟}
  Login -- خیر --> Register[ثبت‌نام / ورود]
  Register --> Checkout[تایید سبد خرید]
  Login -- بله --> Checkout
  Checkout --> Payment[پرداخت آنلاین]
  Payment --> Success{پرداخت موفق بود؟}
  Success -- بله --> OrderConfirm[ثبت سفارش و کد رهگیری]
  Success -- خیر --> Payment
  OrderConfirm --> End([پایان])
