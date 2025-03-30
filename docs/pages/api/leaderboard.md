# Leaderboard

## Get Leaderboard

### GET /leaderboard

Retrieve current game rankings

**Query Parameters**
| Name   | Default | Description          |
|--------|---------|----------------------|
| limit  | 50      | Number of results    |
| offset | 0       | Pagination offset    |

**Success Response**
```json
{
  "total": 1000,
  "results": [
    {
      "rank": 1,
      "username": "top_player",
      "score": 9850,
      "avatar": "https://..."
    },
    {
      "rank": 2,
      "username": "second_best",
      "score": 9800,
      "avatar": "https://..."
    }
  ]
}
```

| Error Code | Description       |
|------------|-------------------|
| 400        | Invalid parameters|