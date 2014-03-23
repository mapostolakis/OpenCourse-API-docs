# Major Items Information (by major id)

## Description

Returns all available information of the major items of a major, for a specific major id.

## Parameters

`GET /majors/id/{major_id}/items`

Parameter  | Type | Required | Description
------- | ------- | ------ | --------
**key** |  String | yes   | Valid API Key
**major_id | Integer | yes | The id of the specified major.

**Output Format**

- json

## Examples

`GET /majors/id/{major_id}/items`

- [http://opencourse.me/api/majors/id/2/items](http://opencourse.me/api/majors/id/2/items)


## Response

Field Name   |  Type    | Description
------------|   -------- |  --------- |
- | Array | An array containing all the major items that belong to the major.

### Major Item Response

Field Name | Type | Description
---------- | ------ | ----------|
**id** | Integer | The major item's id.
**description** | String | The description of the major item as it is stated in the Undergraduate Program Course List.
**departments** | Array | An array containing the department ids of any departments that might be involved with the major item. e.g. "Humanities"
**is_course** | Boolean | A boolean flag stating if the major item is a course or a description of more than one courses.

## Output

### JSON example

```json
[
  {
    "id": 312,
    "description": "WP 1010 Introduction to Academic Writing",
    "departments": null,
    "is_course": true
  },
  {
    "id": 313,
    "description": "WP 1111 Academic Writing",
    "departments": null,
    "is_course": true
  },
  {
    "id": 314,
    "description": "WP 1212 Academic Writing and Research",
    "departments": null,
    "is_course": true
  },
  {
    "id": 315,
    "description": "SP 2200 Presentation Skills or EN 2342 Professional Communication",
    "departments": null,
    "is_course": false
  },
  {
    "id": 316,
    "description": "Two courses in natural science with laboratory",
    "departments": [
      "16",
      "17",
      "22",
      "35",
      "39"
    ],
    "is_course": false
  },
  {
    "id": 317,
    "description": "CS 1070 Introduction to Information Systems",
    "departments": null,
    "is_course": true
  },
  {
    "id": 318,
    "description": "PH 2010 Ethics",
    "departments": null,
    "is_course": true
  },
  {
    "id": 319,
    "description": "One course selected from: archaeology, literature, classical literature, music, philosophy, theatre arts",
    "departments": [
      "15",
      "18",
      "34",
      "8"
    ],
    "is_course": false
  },
  {
    "id": 320,
    "description": "HY 1000 Survey of Western Civilization 1",
    "departments": null,
    "is_course": true
  },
  {
    "id": 321,
    "description": "HY 1001 Survey of Western Civilization 2",
    "departments": null,
    "is_course": true
  },
  {
    "id": 322,
    "description": "PH 2014 Aesthetics",
    "departments": null,
    "is_course": true
  },
  {
    "id": 323,
    "description": "AT 1000 History of Art 1",
    "departments": null,
    "is_course": true
  },
  {
    "id": 324,
    "description": "AT 1001 History of Art 2",
    "departments": null,
    "is_course": true
  },
  {
    "id": 325,
    "description": "Four courses in at least two of the following areas: anthropology, economics, political science, psychology, sociology",
    "departments": [
      "12",
      "21",
      "40",
      "4",
      "5"
    ],
    "is_course": false
  }
]
```