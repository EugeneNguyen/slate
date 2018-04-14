## Contact (High) (New)

This query allow to get contacts

```graphql
contacts {
  _id
  name
  avatar
}
```

> The above command returns JSON structured like this:

```json
{
  "data": {
    "contacts": [
      {
        "_id": 1,
        "name": "Diet Coach",
        "avatar": "http://i.dailymail.co.uk/i/pix/2013/07/01/article-2352727-0EE42FA200000578-317_634x533.jpg"
      }
    ]
  }
}
```

### Request

`contacts: [Contact]`

### Query Parameters

Parameter | Type   | Required | Default | Description
--------- | ------ | -------- | ------- | -----------

