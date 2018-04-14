## Lesson info (Medium) (New)

This query allow to get Lesson info

```graphql
lesson(id: Int) {
  title
  subtitle
  articles {
    title
  }
  videos {
    title
  }
  quiz {
    title
  }
}
```

> The above command returns JSON structured like this:

```json
{
  "data": {
    "title": "Lesson 6",
    "subtitle": "Understanding Nutrition Labels",
    "articles": [
      {
        "title": "Article 1"
      }
    ],
    "videos": [
      {
        "title": "Video 1"
      }
    ],
    "quiz": [
      {
        "title": "Quiz 1"
      }
    ]
  }
}
```

### Request

`lesson(id: Int): Lesson`

### Query Parameters

Parameter | Type   | Required | Default | Description
--------- | ------ | -------- | ------- | -----------
id        | Int    | Yes      | null    |

