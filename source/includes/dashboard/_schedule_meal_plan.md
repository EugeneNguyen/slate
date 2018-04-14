## Schedule Meal Plan (High) (New)

This query allow to get schedule of Meal Plan

```graphql
scheduleMealPlans {
  meal_options {
    id
    name
    food {
      id
      name
      category
      time
    }
  }
  guidance {
    do {
      id
      description
    }
    avoid {
      id
      description
    }
  }
}
```

> The above command returns JSON structured like this:

```json
{
  "data": {
    "meal_options": [
      {
        "id": 1,
        "name": "Option 1",
        "foods": [
          {
            "id": 1,
            "name": "Suspendisse commodo in..",
            "category": "SERVES 2",
            "time": "30M",
            "image": "http://asset1.marksandspencer.com/is/image/mands/MS_FD_F04C_00398503_NC_X_EC_0?$PDP_MAXI_ZOOM_NEW$"
          }
        ]
      }
    ],
    "guidance": {
      "do": [
        {
          "id": 1,
          "description": "Phasellus tristique porta justo vel"
        }
      ],
      "avoid": [
        {
          "id": 1,
          "description": "Phasellus tristique porta justo vel"
        }
      ]
    }
  }
}
```

### Request

`scheduleMealPlans: MealPlan`

### Query Parameters

Parameter | Type   | Required | Default | Description
--------- | ------ | -------- | ------- | -----------

