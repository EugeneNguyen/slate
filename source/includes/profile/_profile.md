## Profile (High) (New)

This query allow to get profile

```graphql
profile {
  user_profile {
    profile_photo
    fullname
  }
  progress {
    glucose1 {
      day
      glucose
    }
    glucose2 {
      day
      glucose
    }
    activity {
      day
      steps
    }
    diet {
      day
      calories
    }
    weeks {
      id
      week
      finished
    }
  }
  goals {
    long_term_goals {
      id
      goal
    }
    short_term_goals: {
      id
      title
      detail
      target
    }
  }
  reports {
    id
    title
    time
  }
}
```

> The above command returns JSON structured like this:

```json
{
  "data": {
    "user_profile": {
      "profile_photo": "https://png.icons8.com/color/1600/avatar.png",
      "fullname": "Joe Doe"
    },
    "progress": {
      "glucose1": [
        { "day": "Mo", "glucose": 100 }
      ],
      "glucose2": [
        { "day": "Mo", "glucose": 110 }
      ],
      "activity": [
        { "day": "Mo", "steps": 5000 }
      ],
      "diet": [
        { "day": "Mo", "calories": 1000 }
      ],
      "weeks": [
        {
          "id": 1,
          "week": 1,
          "finished": true
        }
      ]
    },
    "goals": {
      "long_term_goals": {
        "id": 1,
        "goal": "Maecenas auctor arcu ac convallis suscipit. Nulla fermentum mattis justo, id finibus augue fermentum nec. Sed nec lacus vel turpis dictum porttitor sed vel ipsum."
      },
      "short_term_goals": [
        {
          "id": 1,
          "title": "Stress",
          "detail": "Visit stress coach",
          "target": "2 sessions/week"
        }
      ]
    },
    "reports": [
      {
        "id": "1",
        "title": "Weekly Report",
        "time": "08 Jan 2018 - 14 Jan 2018"
      }
    ]
  }
}

```

### Request

`profile: Profile`

### Query Parameters

Parameter | Type   | Required | Default | Description
--------- | ------ | -------- | ------- | -----------

