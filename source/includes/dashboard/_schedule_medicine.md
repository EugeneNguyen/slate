## Schedule Medicine (High) (New)

This query allow to get schedule of medicine

```graphql
scheduleMedicine(tag: String) {
  medicines {
    id
    name
    qty
  }
  tag
}
```

> The above command returns JSON structured like this:

```json
{
  "data": {
    "medicines": [
      {
        "id": 1,
        "name": "Metformin",
        "qty": "2 Pills"
      },
      {
        "id": 2,
        "name": "Metformin",
        "qty": "2 Pills"
      }
    ],
    "tag": "Lunch"
  }
}

```

### Request

`scheduleMedicine(tag: String): MedicineWithTag`

### Query Parameters

Parameter | Type   | Required | Default | Description
--------- | ------ | -------- | ------- | -----------
tag       | String | Yes      | null    | 

