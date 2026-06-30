# BaSYS.PublicAPI.Examples

Example Bruno collection for BaSYS Public API.

Bruno: <https://www.usebruno.com/>

## Usage

1. Open this repository as a Bruno collection.
2. Select the `local` environment.
3. Set environment variables:
   - `baseUrl` - BaSYS backend URL, for example `https://api.example.com`
   - `dbName` - tenant database name
   - `login` and `password` - user credentials
   - `accessToken` - token returned by `public-api-auth`
   - `refreshToken` - refresh token returned by `public-api-auth`
   - `kind` - meta object kind name
   - `metaObjectKindUid` and `metaObjectUid` - object identifiers to query
4. Run `public-api-auth`, copy the returned token values into the environment, then run the metadata requests.

The committed environment contains only placeholder values. Do not commit real credentials or JWT tokens.

## Инструкция на русском

Это пример коллекции запросов [Bruno](https://www.usebruno.com/) для публичного API BaSYS.

### Как открыть коллекцию

1. Установите Bruno с сайта <https://www.usebruno.com/>.
2. Запустите Bruno.
3. Нажмите `Open Collection`.
4. Выберите папку этого репозитория.
5. В списке environments выберите окружение `local`.

### Как установить переменные environment в Bruno

1. Откройте коллекцию в Bruno.
2. В верхней панели выберите environment `local`.
3. Нажмите на меню environments рядом с названием окружения и откройте редактирование переменных.
4. Заполните значения:
   - `baseUrl` - адрес backend BaSYS, например `https://api.example.com`
   - `dbName` - имя базы данных tenant
   - `login` и `password` - учетные данные пользователя
   - `accessToken` - access token, полученный из запроса `public-api-auth`
   - `refreshToken` - refresh token, полученный из запроса `public-api-auth`
   - `kind` - имя вида метаобъекта
   - `metaObjectKindUid` - идентификатор вида метаобъекта
   - `metaObjectUid` - идентификатор метаобъекта
5. Сохраните изменения environment.

### Порядок работы с запросами

1. Заполните `baseUrl`, `dbName`, `login` и `password`.
2. Выполните запрос `public-api-auth`.
3. Скопируйте из ответа значения token и refresh token в переменные `accessToken` и `refreshToken`.
4. Выполняйте остальные запросы коллекции.

В репозитории сохранены только placeholder-значения. Не коммитьте реальные логины, пароли и JWT-токены.
