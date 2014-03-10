# Course Information (by code)

## Description

Returns all available information of a given course for a specific course _code_.

## Parameters

`GET /courses/code/{code}`

Parameter  | Type | Required | Description
------- | ------- | ------ | --------
**key** |  String | yes   | Valid API Key
**code** | String | yes | The code identifier of the course.

**Output Format**

- json

## Examples

`GET /courses/code/{code}`

- [http://opencourse.me/api/courses/code/AT%201000](http://opencourse.me/api/courses/code/AT%201000)

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

### JSON

```json example
[
  {
    "id": 22,
    "title": "History of Art 1",
    "code": "AT 1000",
    "description": "The Stone Age. Mesopotamian, Egyptian, Minoan, Mycenaean, and ancient Greek art. Roman, Early Christian, and Byzantine art.",
    "level": null,
    "credits": 15,
    "prerequisites": null,
    "department_id": 6
  }
]
```