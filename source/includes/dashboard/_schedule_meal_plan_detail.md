## Schedule Meal Plan Detail (High) (New)

This query allow to get schedule of Meal Plan Detail

```graphql
scheduleMealPlan(id: Int) {
  id
  name
  category
  time
  image
  nutrition {
    summary {
      fiber
      carb
      protein
      fat
    }
    details {
      id
      name
      value
      items {
        id
        name
        value
      }
    }
  }
  ingredients
  directions
}
```

> The above command returns JSON structured like this:

```json
{
  "data": {
    "id": 1,
    "name": "Fettuccine with Brown Butter and Sage",
    "category": "SERVES 2",
    "time": "30M",
    "image": "https://nerdist.com/wp-content/uploads/2016/11/pokemon-cookbook-feature-11282016.jpg",
    "nutrition": {
      "summary": {
        "fiber": 5,
        "carb": 1,
        "protein": 1,
        "fat": 0
      },
      "details": [
        {
          "id": 2,
          "name": "Fat",
          "value": "6g",
          "items": [
            {
              "id": 1,
              "name": "Saturated Fat",
              "value": "1g"
            }
          ]
        }
      ]
    },
    "ingredients": [
      "200 g (7 oz) dried Fettuccine",
    ],
    "directions": [
      "Cook the pasta according to the instructions on the package."
    ]
  }
}
```

### Request

`scheduleMealPlan(id: Int): MealPlan`

### Query Parameters

Parameter | Type   | Required | Default | Description
--------- | ------ | -------- | ------- | -----------
id        | Int    | Yes      | null    |