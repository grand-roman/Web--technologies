# Административный интерфейс в Django

### Материалы

[The Django admin site](https://docs.djangoproject.com/en/4.1/ref/contrib/admin/)

[The Django admin site](https://docs.djangoproject.com/en/4.1/ref/contrib/admin/#modeladmin-objects)

[ModelAdmin List Filters | Django documentation](https://docs.djangoproject.com/en/4.1/ref/contrib/admin/filters/)

[The Django admin site](https://docs.djangoproject.com/en/4.1/ref/contrib/admin/#inlinemodeladmin-objects)

[The Django admin site](https://docs.djangoproject.com/en/4.1/ref/contrib/admin/#django.contrib.admin.ModelAdmin.fieldsets) 

[Admin actions | Django documentation](https://docs.djangoproject.com/en/4.1/ref/contrib/admin/actions/)

## Цели практической работы 

-   Создать модели и подключить их к админке.
    
-   Вывести поля модели на страницу в админке.
    
-   Реализовать поиск по полям в модели.
    
-   Отобразить связь «ко многим».
    
-   Разделить поля по группам (на странице деталей).
    
-   Добавить групповое действие для моделей в таблице.
    

## Что нужно сделать

Для выполнения работы используйте проект mysite, приложение ShopApp и модели Product и Order (всё это можно взять из предыдущей практической работы).

1.  Подключите модели Product и Order к админке.
    
2.  Выведите поля модели на страницу в админке.
    
3.  Добавьте поиск по двум полям в модели (можно больше). Одно поле должно быть строковым, другое — числовым.
    
4.  Отобразите связь «ко многим» на странице модели, на которой по умолчанию связь не отображается (в данном случае это Product, к модели которого нужно добавить Order).
    
5.  Разделите поля по группам (на странице деталей объекта): базовая группа без названия с полями «Имя» и «Описание», группа по цене с полями «Цена» и «Скидка», а также группа с дополнительными опциями, где будет поле по архивации (эта секция должна быть свёрнута).
    
6.  Добавьте групповое действие для архивации записей в таблице.
    

## Рекомендации
Практическая работа подразумевает использование следующих атрибутов.

-   [TabularInline](https://docs.djangoproject.com/en/4.1/ref/contrib/admin/#django.contrib.admin.TabularInline)
    
-   [fieldsets](https://docs.djangoproject.com/en/4.1/ref/contrib/admin/#django.contrib.admin.ModelAdmin.fieldsets)
    
-   [Admin actions](https://docs.djangoproject.com/en/4.1/ref/contrib/admin/actions/)
    

## Что оценивается

-   Приложение установлено и настроено, модели описаны, миграции сгенерированы.
    
-   Admin-модели созданы и зарегистрированы (отображаются в админке).
    
-   Реализован поиск по полям в модели: минимум одно строковое поле («Имя», «Описание») и минимум одно числовое поле («Цена», «Скидка»).
    
-   На одной из моделей отображена связь «ко многим» (где по умолчанию отображения нет). Сделайте отображение заказов на странице деталей продукта.
    
-   Для моделей в таблице реализовано групповое действие (групповая архивация продуктов).
