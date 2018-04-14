## Message (High) (New)

This query allow to get messages of a conversation

```graphql
messages(conversation_id: Int) {
  messages {
    _id
    createdAt
    appointment {
      _id
      title
      by
      at
      start
      end
      to
      status
      our_own_data
    }
    user: {
      _id
      name
      avatar
    }
  }
  users {
    _id
    name
    avatar
  }
}
```

> The above command returns JSON structured like this:

```json
{
  "data": {
    "messages": [
      {
        "_id": 4,
        "createdAt": "2018-04-05T23:58:46.265Z",
        "appointment": {
          "_id": 1,
          "title": "Appointment Request",
          "by": "Phonecall",
          "at": "2018-04-05T23:58:46.265Z",
          "start": "9:30",
          "end": "10:00",
          "to": "Dr. Rakesh Yadav",
          "status": "waiting",
          "our_own_data": "Our own data"
        },
        "user": {
          "_id": 2,
          "name": "React Native",
          "avatar": "http://i.dailymail.co.uk/i/pix/2013/07/01/article-2352727-0EE42FA200000578-317_634x533.jpg"
        }
      }
    ],
    "users": [
      {
        "_id": 2,
        "name": "React Native",
        "avatar": "http://i.dailymail.co.uk/i/pix/2013/07/01/article-2352727-0EE42FA200000578-317_634x533.jpg"
      }
    ]
  }
}
```

### Request

`messages(conversation_id: Int): [Message]`

### Query Parameters

Parameter | Type   | Required | Default | Description
--------- | ------ | -------- | ------- | -----------
conversation_id | Int | Yes   | null    |

