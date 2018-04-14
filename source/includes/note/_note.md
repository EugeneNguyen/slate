## Note (Medium) (New)

This query allow to get notes

```graphql
notes {
  id
  title
  content
  date
}
```

> The above command returns JSON structured like this:

```json
{
  "data": [
    {
      "id": "1",
      "title": "Hello",
      "content": "- Added Popover component, so you can use it in whole app if need.",
      "date": "06/Apr/2018"
    }
  ]
}
```

### Request

`messages(conversation_id: Int): [Message]`

### Query Parameters

Parameter | Type   | Required | Default | Description
--------- | ------ | -------- | ------- | -----------

