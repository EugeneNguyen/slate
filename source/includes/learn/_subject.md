## Subject (Medium) (New)

This query allow to get Subject

```graphql
learnSubjects {
  estimation
  subjects: {
    id
    completed
    total
    title
    lesson_groups
  }
}
```

> The above command returns JSON structured like this:

```json
{
  "data": {
    "estimation": "5 days streak",
    "subjects": [
      {
        "id": 1,
        "completed": 15,
        "total": 15,
        "title": "Basics",
        "lesson_groups": 3
      }
    ]
  }
}

```

### Request

`learnSubjects: Subject`

### Query Parameters

Parameter | Type   | Required | Default | Description
--------- | ------ | -------- | ------- | -----------

