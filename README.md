# DummyAPI

В процесс прохождения практики на курсе "Тестирование REST API. Postman" мной тестировался сервис DummyAPI, а именно объект **Post**, для тестирования данного оъекта была создана MindMap по который были созданы тест-кейсы, которые в свою очередь были заведены в коллецию далее для более удобной работы было создано необходимое окружение, после этого были добавленны простые автотесты! Полная информация с ссылками и примерами ниже.

## Оглавление

1. [Описание проекта](#introduction)
2. [POST](#paragraph1)
 
    2.1. [GET /post](#subparagraph1)
    
    2.2. [POST /post/create](#subparagraph2)
3. [Майнд-карта](#paragraph2)





## Описание проекта <a name="introduction"></a>


https://dummyapi.io/ Данный сайт представляет собой сервис для тестирования API. Для выполнения запросов необходим app-id, который можно получить автоматически после регистрации на сайте. В качестве тестирования взят объект **Post**.

## POST <a name="paragraph1"></a>

#### GET /post (Get List) <a name="subparagraph1"></a>
Возвращает список постов. 
- доступен query params для вывода определенной страницы.
- доступен query params для отображения числа постов на странице.
  
List (пример)
```javascript

{
  "data":
  "total": 995,
  "page": 0
  "limit": 5
}

```
Post Preview (пример)
```javascript
 {
 "id": "63fe100e59f47dff96c66bc9",
 "image": "https://img.dummyapi.io/photo-1564694202779-bc908c327862.jpg",
 "likes": 43,
 "tags": [
 "animal",
 "dog",
 "golden retriever"],
 "text": "qwerty",
 "publishDate": "2023-02-28T14:30:38.354Z",
 "updatedDate": "2023-02-28T14:30:38.354Z",
 "owner": {
 "id": "60d0fe4f5311236168a109ca",
 "title": "ms",
 "firstName": "Sara",
 "lastName": "Andersen",
 "picture": "https://randomuser.me/api/portraits/women/58.jpg"
            }
        }
```
        
#### POST /post/create (Create Post) <a name="subparagraph2"></a>

Создает новsq пост. Возвращает данные о посте.

Request Body (Пример)

```javascript
{
 "text": "qwert",
 "image": "https://img.dummyapi.io/photo-1564694202779-bc908c327862.jpg",
 "likes": 43,
 "tags": [
 "animal",
 "dog",
 "golden retriever"],
 "owner": "60d0fe4f5311236168a109ca"
    }
```

Response Body (Пример)


```javascript
{
 "id": "63ff46bb6d62c40516e776b6",
 "image": "https://img.dummyapi.io/photo-1564694202779-bc908c327862.jpg",
 "likes": 43,
 "link": "",
 "tags": [
 "animal",
 "dog",
 "golden retriever"],
 "text": "qwert",
 "publishDate": "2023-03-01T12:36:11.413Z",
 "updatedDate": "2023-03-01T12:36:11.413Z",
 "owner": {
 "id": "60d0fe4f5311236168a109ca",
 "title": "ms",
 "firstName": "Sara",
 "lastName": "Andersen",
 "picture": "https://randomuser.me/api/portraits/women/58.jpg"
    }
}
```



## Майнд-карта <a name="paragraph2"></a>

![Alt-текст](https://i.imgur.com/ivbGpbG.png)

Также майнд-карту можно скачать [здесь](https://github.com/VladimirB17/DummyAPI/blob/main/Dummy_API%20(2).xmind)

## Тест-кейсы
Также были оформлены тест-кейсы в соответствии с майнд-картой.
Тест-кейсы можно посмотреть тут

## Баг-репорты

## Коллекции POSTMAN

## Автотесты

{
    "data":
    "total": 995,
    "page": 0,
    "limit": 5
}


