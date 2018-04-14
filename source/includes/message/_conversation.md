## Contact (High) (New)

This query allow to get conversations

```graphql
conversations {
  id
  last_message
  user {
    id
    name
    photo
  }
}
```

> The above command returns JSON structured like this:

```json
{
  "data": [
    {
      "id": 1,
      "last_message": "Last message content...",
      "user": {
        "id": 4,
        "name": "Diet Coach",
        "photo": ""
      }
    }
  ]
}

```

### Request

`conversations: [Conversation]`

### Query Parameters

Parameter | Type   | Required | Default | Description
--------- | ------ | -------- | ------- | -----------

