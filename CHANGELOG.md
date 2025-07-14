# Changelog

## v0.1.31 - 25-07-14
- Обновлены методы Magnit Post

## v0.1.30 - 25-07-09
- Добавлен новый метод Magnit Post для эстимации времени и сроков доставки

## v0.1.29 - 25-07-02
- Добавлена ручка обновления СКУ.
- Внесены правки в документацию

## v0.1.28 - 25-06-24
- Обновление методы Last Mile

## v0.1.27 - 25-06-17
- Улучшения документации по ручкам для работы с характеристиками, словарями и ску;
- Исправлен фильтр в ручке получения списка ску (/api/seller/v1/products/sku/list).
- Исправлен tag у нескольких ручек API Магнит Маркет.
- Для API Магнит Маркет добавлены scope.

## v0.1.25 - 25-05-30
- Ручка загрузки продуктов: добавили возможность создания характеристик.
- Ручки словарей и характеристик: расширен ответ.
- Исправлены описания многих ручек, добавлен перевод.

## v0.1.24 - 25-04-17
- Добавился новый метод POST /api/seller/v1/products/sku/shops/{shop_id}/short/list для получения списка компактной информации по SKU
- Добавились новые поля в SkuRequest (POST /api/seller/v1/products/sku):
  defined_characteristic_list
  product_filters_list

## v0.1.23 - 25-03-18
- Исправлен фильтр для ручки получения данных по остаткам (/api/seller/v1/products/sku/stocks/info).

## v0.1.22 - 25-03-14
- Обновлен SkuFilter;
- Изменены error responses.
- 
## v0.1.21 - 25-03-11
- API Magnit Market Получение статуса заявок загрузки SKU (GET /api/seller/v1/products/sku/tasks/{task_id}/status) - в response (TaskStatusResponse) добавлено поле status.
- Если не удалось найти Продавца в некоторых случаях теперь возвращается 401 Unauthorized (было 404).

## v0.1.20 - 25-03-06
- Исправлено дублирование `/api/` в адресах Magnit Market API.

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

