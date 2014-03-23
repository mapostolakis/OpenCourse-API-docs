# Majors Information (by school)

## Description

Returns all available information for any majors stored in the database, for a specified school.

## Parameters

`GET /majors/school/{school_id}`

Parameter  | Type | Required | Description
------- | ------- | ------ | --------
**key** |  String | yes   | Valid API Key
**school** | Integer | yes | The specified school.

**Output Format**

- json

## Examples

`GET /majors/school/{school_id}`

- [http://opencourse.me/api/majors/school/1](http://opencourse.me/api/majors/school/1)


## Response

Field Name   |  Type    | Description
------------|   -------- |  --------- |
- | Array | An array containing all majors where their school code matches the school code parameter.


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