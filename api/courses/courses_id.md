# Course Information (by course id)

## Description

Returns all available information of a given course for a specific course _id_.

## Parameters

`GET /courses/id/{course_id}`

Parameter  | Type | Required | Description
------- | ------- | ------ | --------
**key** |  String | yes   | Valid API Key
**course_id** | Integer | yes | The id of the course.

**Output Format**

- json

## Examples

`GET /courses/id/{course_id}`

- [http://opencourse.me/api/courses/id/40](http://opencourse.me/api/courses/id/40)


## Response

Field Name   |  Type    | Description
------------|   -------- |  --------- |
**id**  | Integer  | The id of the course.
**title** | String | The title of the course.
**code** | String | The code identifier of the course. 
**description**  | String   |  A brief description of the course.
**level** | Integer | The level of the course.
**credits** | Integer | The number of credits of the course.
**prerequisites** | Array  |  An array containing all the course codes of the prerequisite courses of the course.
**department_id** |  Integer   | The id of the department that the course belongs to.


## Output

### JSON example

```json 
[
  {
    "id": 40,
    "title": "The Italian Renaissance",
    "code": "AT 3109",
    "description": "The phenomenon of the Italian Renaissance and its relation to political, social and economic circumstances. The emergence and function of the arts in shaping the physical and ideological appearance of the Italian cities/centers of power.",
    "level": 6,
    "credits": 15,
    "prerequisites": [
      "AT 1001"
    ],
    "department_id": 6
  }
]
```