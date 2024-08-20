1. Register a User:

Method: POST
URL: http://localhost:8000/api/register
Body: JSON
{
    "username": "newuser",
    "email": "newuser@example.com",
    "first_name": "New",
    "last_name": "User",
    "password": "newpassword"
}
--------------------------------------------------------

2. List Users:

Method: GET
URL: http://localhost:8000/api/users
Headers:
Authorization: Bearer <access_token>
--------------------------------------------------------
3. Retrieve User Details:

Method: GET
URL: http://localhost:8000/api/users/<user_id>
Headers:
Authorization: Bearer <access_token>
--------------------------------------------------------

4. Update User Details:

Method: PATCH
URL: http://localhost:8000/api/users/<user_id>
Headers:
Authorization: Bearer <access_token>
Body: JSON
{
    "first_name": "UpdatedName"
}
-------------------------------------------------------
5. Delete User:

Method: DELETE
URL: http://localhost:8000/api/users/<user_id>
Headers:
Authorization: Bearer <access_token>
-------------------------------------------------------
