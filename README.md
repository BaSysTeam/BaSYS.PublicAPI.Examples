# BaSYS.PublicAPI.Examples

Example Bruno collection for BaSYS Public API.

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
