# Обработка запросов в Django, Middlewares

### Материалы

-   [Концепция MVC и MTV](https://habr.com/ru/company/vivid_money/blog/544856/) 

-   [Postman](https://www.postman.com/)
    
-   [Insomnia REST](https://insomnia.rest/)

-   [HTTPBin](https://httpbin.org/) 

-   [Request and response objects | Django documentation](https://docs.djangoproject.com/en/4.1/ref/request-response/#django.http.HttpRequest.POST) 
    
-   [File storage API | Django documentation](https://docs.djangoproject.com/en/4.1/ref/files/storage/) 

-   [Middleware | Django documentation](https://docs.djangoproject.com/en/4.1/topics/http/middleware/) 
    
-   [Порядок вызова обработчиков в Middleware](https://miro.medium.com/max/640/1*CrgbKz0w7yio7i4LaykOJg.png)
    

  
  

## Цели практической работы

-   Сделать view-функцию для загрузки файлов с ограничением по размеру.
    
-   Написать throttling middleware (лимит по запросам от пользователя).
    

  

### Что нужно сделать

#### Задача 1

Создайте view-функцию для загрузки файлов с ограничением по размеру.

Рекомендация: проверьте размер файла перед сохранением и верните пользователю ошибку, если файл превышает заданный размер.

  

#### Задача 2

Напишите throttling middleware, который будет ограничивать обработку запросов пользователя, если он делает обращения слишком часто.

Рекомендация: возьмите IP-адрес пользователя из request.meta. Проверьте, как давно пользователь с этим IP выполнял запрос. Если недавно, то верните ошибку и не обрабатывайте дальше запрос.

  

### Что оценивается

-   Приложение установлено и настроено.
    
-   Функция для загрузки файла не позволяет загрузить файл размером более 1 Мб.
    
-   При частом посещении пользователем страниц сайта ему возвращается ошибка о превышении лимита на количество запросов. 
