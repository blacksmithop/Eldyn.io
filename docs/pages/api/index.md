# API Overview

Welcome to the API documentation. This API provides user management and game features.

## Base URL
`https://api.example.com/v1`

## Common Headers
```json
{
  "Content-Type": "application/json",
  "Authorization": "Bearer <token>"
}
```

## Error Responses
```json
{
  "error": {
    "code": "STATUS_CODE",
    "message": "Human-readable description"
  }
}
```

| Status Code | Description          |
|-------------|----------------------|
| 400         | Bad Request          |
| 401         | Unauthorized         |
| 404         | Not Found            |
| 500         | Internal Server Error|