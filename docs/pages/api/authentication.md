# Authentication

## Login

### POST /auth/login

Authenticate user with credentials

**Request Body**
```json
{
  "email_or_username": "user@example.com",
  "password": "securepassword123"
}
```

**Success Response**
```json
{
  "token": "eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9...",
  "expires_in": 3600
}
```

## Sign-Up

### POST /auth/signup

Create new user account

**Request Body (Email/Password)**
```json
{
  "username": "new_user",
  "email": "new@example.com",
  "password": "SecurePassword123!"
}
```

**Request Body (OAuth)**
```json
{
  "provider": "google",
  "access_token": "ya29.a0AfH6SMB..."
}
```

**Success Response**
```json
{
  "id": "USER_ID",
  "username": "new_user",
  "email": "new@example.com",
  "created_at": "2023-07-15T12:34:56Z"
}
```

| Error Code | Description                  |
|------------|------------------------------|
| 400        | Invalid credentials format  |
| 409        | Email/username already exists|