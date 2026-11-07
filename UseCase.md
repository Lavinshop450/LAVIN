
```mermaid
graph L
@startuml
left to right direction

actor "مشتری" as Customer
actor "مدیر فروشگاه" as Admin
actor "درگاه پرداخت" as Payment

rectangle "سامانه فروشگاه آنلاین LAVIN" {

  usecase "ثبت‌نام" as UC1
  usecase "ورود به حساب کاربری" as UC2

  usecase "مشاهده محصولات" as UC3
  usecase "جست‌وجو و فیلتر محصولات" as UC4
  usecase "مشاهده جزئیات محصول" as UC5
  usecase "مشاهده راهنمای سایز" as UC6
  usecase "مشاهده نظرات و امتیازها" as UC7
  usecase "ثبت نظر و امتیاز" as UC8

  usecase "مدیریت سبد خرید" as UC9
  usecase "محاسبه مبلغ سفارش" as UC10
  usecase "ثبت سفارش" as UC11
  usecase "پرداخت آنلاین" as UC12
  usecase "مشاهده و پیگیری سفارش" as UC13

  usecase "درخواست مرجوعی" as UC14
  usecase "درخواست تعویض سایز" as UC15

  usecase "مشاهده پیشنهادهای هدیه" as UC16
  usecase "خرید کارت هدیه" as UC17
  usecase "درخواست بسته‌بندی ویژه" as UC18

  usecase "ثبت سفارش دوخت اختصاصی" as UC19

  usecase "مدیریت محصولات" as UC20
  usecase "مدیریت سفارش‌ها" as UC21
}

Customer -- UC1
Customer -- UC2
Customer -- UC3
Customer -- UC4
Customer -- UC5
Customer -- UC6
Customer -- UC7
Customer -- UC8
Customer -- UC9
Customer -- UC11
Customer -- UC13
Customer -- UC14
Customer -- UC15
Customer -- UC16
Customer -- UC17
Customer -- UC18
Customer -- UC19

Admin -- UC20
Admin -- UC21

Payment -- UC12

UC5 ..> UC6 : <<extend>>
UC8 ..> UC7 : <<extend>>
UC11 ..> UC10 : <<include>>
UC11 ..> UC12 : <<include>>
UC14 ..> UC13 : <<extend>>
UC15 ..> UC13 : <<extend>>
UC18 ..> UC11 : <<extend>>
