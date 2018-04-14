## Recent Medication (High) (New)

This query allow to get contacts

```graphql
medicationRecent {
  id
  medBrand
  medName
  medDosage
}
```

> The above command returns JSON structured like this:

```json
{
  "data": [
    {
      "id": "1",
      "medBrand": "Metaglip",
      "medName": "Glipizide & Metformin",
      "medDosage": "500 mg per pill"
    }
  ]
}
```

### Request

`medicationRecent: [Medication]`

### Query Parameters

Parameter | Type   | Required | Default | Description
--------- | ------ | -------- | ------- | -----------

