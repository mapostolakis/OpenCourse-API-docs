# Majors Information

## Description

Returns all available information for any majors stored in the database.

## Parameters

`GET /majors/all`

Parameter  | Type | Required | Description
------- | ------- | ------ | --------
**key** |  String | yes   | Valid API Key

**Output Format**

- json

## Examples

`GET /majors/all`

- [http://opencourse.me/api/majors/all](http://opencourse.me/api/majors/all)


## Response

Field Name   |  Type    | Description
------------|   -------- |  --------- |
**id**  | Integer  | The id of the major.
**title** | String | The title of the major.
**school** | Integer | The code of the specified school. See **_School Codes_** below for more information.


### School Codes

School | Code |
------| ------- |
**School of Business** | 0 
**School of Liberal Arts & Sciences** | 1
**Frances Rich School of Fine & Performing Arts** | 2

## Output

### JSON example

```json
[
  {
    "id": 1,
    "title": "Information Technology",
    "school": 1
  },
  {
    "id": 2,
    "title": "Art History",
    "school": 1
  },
  {
    "id": 3,
    "title": "Communication",
    "school": 1
  },
  {
    "id": 4,
    "title": "Economics",
    "school": 1
  },
  {
    "id": 5,
    "title": "English & American Literature",
    "school": 1
  },
  {
    "id": 6,
    "title": "Environmental Studies",
    "school": 1
  },
  {
    "id": 8,
    "title": "Philosophy",
    "school": null
  },
  {
    "id": 9,
    "title": "Psychology",
    "school": null
  },
  {
    "id": 10,
    "title": "Sociology",
    "school": 1
  },
  {
    "id": 11,
    "title": "Liberal Studies",
    "school": 1
  },
  {
    "id": 12,
    "title": "History",
    "school": 1
  },
  {
    "id": 13,
    "title": "English Literature with Linguistics",
    "school": 1
  }
]
```