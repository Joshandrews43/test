<a name="top"></a>
# carline-backend v1.0.0



 - [Student](#Student)
   - [Check student in/out](#Check-student-in/out)
   - [Create Student](#Create-Student)
   - [Get All Students](#Get-All-Students)
   - [Get Student](#Get-Student)

___


# <a name='Student'></a> Student

## <a name='Check-student-in/out'></a> Check student in/out
[Back to top](#top)

```
GET /api/:schoolId/:studentId/sign
```

### Parameters - `Parameter`

| Name     | Type       | Description                           |
|----------|------------|---------------------------------------|
| schoolId | `String` |  |

### Parameters - `body`

| Name     | Type       | Description                           |
|----------|------------|---------------------------------------|
| guardianId | `String` |  |

### Parameters - `query`

| Name     | Type       | Description                           |
|----------|------------|---------------------------------------|
| signOption | `String` | <p><code>signIn</code> or <code>signOut</code></p> |
| guardianless | `boolean` | <p>Whether the sign was guardianless</p> |

### Success response

#### Success response - `Success 200`

| Name     | Type       | Description                           |
|----------|------------|---------------------------------------|
| student | `Object` | <p>Updated student data with new <code>signedIn</code> status.</p> |

## <a name='Create-Student'></a> Create Student
[Back to top](#top)

```
GET /api/:schoolId/student
```

### Parameters - `Parameter`

| Name     | Type       | Description                           |
|----------|------------|---------------------------------------|
| schoolId | `String` |  |

### Parameters - `body`

| Name     | Type       | Description                           |
|----------|------------|---------------------------------------|
| Student | `String` | <p>An object containing the students information</p> |

### Success response

#### Success response - `Success 200`

| Name     | Type       | Description                           |
|----------|------------|---------------------------------------|
| student | `Object` | <p>Created student data inlcuding default fields.</p> |

## <a name='Get-All-Students'></a> Get All Students
[Back to top](#top)

```
GET /api/:schoolId/students
```

### Parameters - `Parameter`

| Name     | Type       | Description                           |
|----------|------------|---------------------------------------|
| schoolId | `String` |  |

### Success response

#### Success response - `Success 200`

| Name     | Type       | Description                           |
|----------|------------|---------------------------------------|
| students | `Object` | <p>Object of students with studentId's as key.</p> |

## <a name='Get-Student'></a> Get Student
[Back to top](#top)

```
GET /api/:schoolId/:studentId
```

### Parameters - `Parameter`

| Name     | Type       | Description                           |
|----------|------------|---------------------------------------|
| schoolId | `String` |  |
| studentId | `String` |  |

### Success response

#### Success response - `Success 200`

| Name     | Type       | Description                           |
|----------|------------|---------------------------------------|
| student | `Object` | <p>Student data.</p> |
