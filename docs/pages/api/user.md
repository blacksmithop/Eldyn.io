# User Operations

## Get User Details

### GET /users/{id}

Retrieve user profile information

**Path Parameters**
| Name | Description  |
|------|--------------|
| id   | User ID      |

**Success Response**
```json
{
  "id": "USER_ID",
  "username": "example_user",
  "email": "user@example.com",
  "joined_at": "2023-01-01T00:00:00Z",
  "stats": {
    "score": 1500,
    "rank": 42
  }
}
```

| Error Code | Description       |
|------------|-------------------|
| 401        | Unauthorized access |
| 404        | User not found    |