## Search Medication (High) (New)

This query allow to get medication with brand and/or name

```graphql
medications(brand: String, name: String) {
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

`medications(brand: String, name: String): [Medication]`

### Query Parameters

Parameter | Type   | Required | Default | Description
--------- | ------ | -------- | ------- | -----------
brand     | String | No       | null    | when no brand defined, return all other medication
name      | String | No       | null    | when no name defined, return all other medication
