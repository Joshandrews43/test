<a name="top"></a>
# carline-backend v1.0.0



 - [Student](#Student)
   - [Get All Students](#Get-All-Students)
 - [User](#User)
   - [Request User information](#Request-User-information)

___


# <a name='Student'></a> Student

## <a name='Get-All-Students'></a> Get All Students
[Back to top](#top)

```
GET /api/:schoolId/students
```

### Success response

#### Success response - `Success 200`

| Name     | Type       | Description                           |
|----------|------------|---------------------------------------|
| students | `Object` | <p>Object of students with studentId's as key.</p> |

# <a name='User'></a> User

## <a name='Request-User-information'></a> Request User information
[Back to top](#top)

```
GET /user/:id
```

### Parameters - `Parameter`

| Name     | Type       | Description                           |
|----------|------------|---------------------------------------|
| id | `Number` | <p>Users unique ID.</p> |

### Success response

#### Success response - `Success 200`

| Name     | Type       | Description                           |
|----------|------------|---------------------------------------|
| firstname | `String` | <p>Firstname of the User.</p> |
| lastname | `String` | <p>Lastname of the User.</p> |
