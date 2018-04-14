## Schedule Food (High) (New)

This query allow to get schedule of Food

```graphql
scheduleFood(tag: String, time: String) {
  foods {
    id
    name
  }
  options {
    tag
    time
  }
}
```

> The above command returns JSON structured like this:

```json
{
  "data": {
    "foods": [
      {
        "id": 1,
        "name": "Tomatoe & Cheese Toast"
      },
      {
        "id": 2,
        "name": "Tomatoe & Cheese Toast"
      }
    ],
    "options": {
      "tag": "Lunch",
      "time": "13:56"
    }
  }
}

```

### Request

`scheduleFood(tag: String, time: String): Food`

### Query Parameters

Parameter | Type   | Required | Default | Description
--------- | ------ | -------- | ------- | -----------
tag       | String | Yes      | null    | 
time      | String | Yes      | null    | 

