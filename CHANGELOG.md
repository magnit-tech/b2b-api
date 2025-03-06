# Changelog

## v0.1.19 - 25-03-06
- Добавлен эндпоинт получения списка активных магазинов (GET /seller/v1/shops).
- В эндпоинте POST /seller/v1/products/sku/list в response у поля vat сменился тип на string.
- В эндпоинте удаления SKU (POST /seller/v1/products/sku/shops/{shop_id}/sku/delete)  изменились требования в request параметрам.
- В эндпоинте создания/обновления списка SKU (POST /seller/v1/products/sku) в request из обязательных убрано поле okpd2 и добавлено short_description.
- В эндпоинтах работы с заказами и посылками небольшие правки.

## v0.1.18 - 25-03-05
- Создание/обновление списка СКУ (POST /seller/v1/products/sku): в request для поля barcode поднята разрядность типа до int64

## v0.1.17 - 25-02-26
- POST /api/seller/v1/products/sku/price: добавлено описание response
- POST /api/seller/v1/products/sku/list: исправлено описание request

## v0.1.16 - 25-02-25
- В /api/seller/v1/products/sku/shops/{shop_id}/sku/unarchive параметры запроса перенесены из Query String в Request Body
- В /api/seller/v1/products/sku/shops/{shop_id}/sku/delete параметры запроса перенесены из Query String в Request Body

## v0.1.15 - 25-02-21
* Обновлена сущность Sku в API Magnit Market FBS
* Изменена пагинация для запроса словарей в API Magnit Market FBS

## v0.1.14 - 25-02-12
* Изменено описание метода /api/seller/v1/products/dictionary в API Magnit Market FBS
* Имена некоторых параметров переименованы согласно общему код-стайлу из camelCase в snake_case в API Magnit Market FBS
* Добавлены новые методы в API Magnit Market FBS
* Расширено описание методов API Magnit Market FBS

## v0.1.13 - 25-02-11
* Изменен адрес демо-стенда для проведения тестирования
* Исправлены методы API Magnit Market FBS

## v0.1.12 - 25-02-06
* Внесены изменения в методы API Magnit Market FBS

## v0.1.11 - 25-02-05
* Добавлены методы API Magnit Market FBS

## v0.1.10 - 24-07-12
* Добавлены методы API Magnit Post

## v0.1.9 - 24-07-01
* Добавлены методы API Last Mile

## v0.1.8 - 24-05-23
* Добавлен новый метод аутентификации v2.
* Метод аутентификации v1 объявлен как deprecated. Его поддержка прекратится 31 января 2025 года.

## v0.1.7 - 24-04-26
* В метод состава заказа добавлен идентификатор запроса и время проверки марки из-за вступления в силу изменения правил работы с маркированным товаром согласно ППРФ № 1944.

## v0.1.6 - 23-12-27
* Добавлены возможные причины отмен заказов.

