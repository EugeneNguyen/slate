## Login (High) (New)

This mutation allow to login and get access token to work with other queries and mutations

```graphql
mutation login($username: String, $password: String) {
  jwtToken 
}
```

> The above command returns JSON structured like this:

```json
{
  "data": {
    "authenticate": {
      "jwtToken": "<Access token>"
    }
  }
}
```

### Request

`mutation login($username: String, $password: String): AccessToken`

### Query Parameters

Parameter | Type   | Required | Default | Description
--------- | ------ | -------- | ------- | -----------
username  | String | Yes      | null    | 
password  | String | Yes      | null    | [TBD] Encrypted or not
