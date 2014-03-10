# Department Information

## Description

Returns all available information for any departments stored in the database.

## Parameters

`GET /departments/all`

Parameter  | Type | Required | Description
------- | ------- | ------ | --------
**key** |  String | yes   | Valid API Key

**Output Format**

- json

## Examples

`GET /departments/all`

- [http://opencourse.me/api/departments/all](http://opencourse.me/api/departments/all)


## Response

Field Name   |  Type    | Description
------------|   -------- |  --------- |
**id**  | Integer  | The id of the department.
**title** | String | The title of the department.
**abbreviation** | String | A two or three letter abbreviation used in course codes. 
**area**  | String   |  The area a department might belong in. e.g.: "Humanities".


## Output

### JSON example

```json
[
  {
    "id": 1,
    "title": "Writing Program",
    "abbreviation": "WP",
    "area": null
  },
  {
    "id": 2,
    "title": "Information Technology",
    "abbreviation": "IT",
    "area": null
  },
  {
    "id": 3,
    "title": "Mathematics",
    "abbreviation": "MA",
    "area": null
  },
  {
    "id": 4,
    "title": "Sociology",
    "abbreviation": "SO",
    "area": "Social Sciences"
  },
  {
    "id": 5,
    "title": "Psychology",
    "abbreviation": "PS",
    "area": null
  },
  {
    "id": 6,
    "title": "Art History",
    "abbreviation": "AT",
    "area": "Humanities"
  },
  {
    "id": 7,
    "title": "History",
    "abbreviation": "HY",
    "area": "Humanities"
  },
  {
    "id": 8,
    "title": "Philosophy",
    "abbreviation": "PH",
    "area": null
  },
  {
    "id": 9,
    "title": "CIS",
    "abbreviation": "CS",
    "area": null
  },
  {
    "id": 10,
    "title": "English",
    "abbreviation": "EN",
    "area": "Humanities"
  },
  {
    "id": 11,
    "title": "Accounting & Finance",
    "abbreviation": "AF",
    "area": null
  },
  {
    "id": 12,
    "title": "Anthropology",
    "abbreviation": "AN",
    "area": "Social Sciences"
  },
  {
    "id": 13,
    "title": "Applied Psychology",
    "abbreviation": "AP",
    "area": null
  },
  {
    "id": 14,
    "title": "Archaeology Special Topics",
    "abbreviation": "AHX",
    "area": "Humanities"
  },
  {
    "id": 15,
    "title": "Archaeology",
    "abbreviation": "AH",
    "area": null
  }
]
```