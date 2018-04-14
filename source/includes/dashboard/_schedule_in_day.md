## Schedule In Day (High) (New)

This query allow to get schedule in a day

```graphql
scheduleInDay($date: String) {
  date
  summary {
    nutrition
    exercise
  }
  activities {
    type
    data
  }
}
```

> The above command returns JSON structured like this:

```json
{
  "data": {
    "date": "2018-04-11",
    "summary": {
      "nutrition": [
        {
          "id": "fiber",
          "name": "Fiber",
          "completed": 4,
          "total": 10
        }
      ],
      "exercise": {
        "steps": 1200,
        "activity": "45m"
      }
    },
    "activities": [
      {
        "id": 8,
        "type": "medication",
        "data": {
          "medicines": [
            {
              "id": 1,
              "name": "Metformin",
              "qty": "2 Pills"
            }
          ],
          "completed": false
        }
      },
      {
        "id": 9,
        "type": "weight",
        "data": {
          "completed": false
        }
      },
    ]
  }
}
```

### Request

`scheduleInDay($date: String): Schedule`

### Query Parameters

Parameter | Type   | Required | Default | Description
--------- | ------ | -------- | ------- | -----------
date      | String | No       | today   | if param date is missing, return today result

