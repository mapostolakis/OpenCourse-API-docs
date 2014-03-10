# Department Information (by department id)

## Description

Returns all available information of a given department for a specific department id.

## Parameters

`GET /departments/id/{department_id}`

Parameter  | Type | Required | Description
------- | ------- | ------ | --------
**key** |  String | yes   | Valid API Key

**Output Format**

- json

## Examples

`GET /departments/id/{department_id}`

- [http://opencourse.me/api/departments/id/6](http://opencourse.me/api/departments/id/6)


## Response

Field Name   |  Type    | Description
------------|   -------- |  --------- |
**id**  | Integer  | The id of the department.
**title** | String | The title of the department.
**abbreviation** | String | A two or three letter abbreviation used in course codes. 
**area**  | String   |  The area a department might belong in. e.g.: "Humanities".
**courses** | Array | An array containing all the courses that belong to the department.


## Output

### JSON example

```json
[
  {
    "id": 6,
    "title": "Art History",
    "abbreviation": "AT",
    "area": "Humanities",
    "courses": [
      {
        "id": 22,
        "title": "History of Art 1",
        "code": "AT 1000",
        "description": "The Stone Age. Mesopotamian, Egyptian, Minoan, Mycenaean, and ancient Greek art. Roman, Early Christian, and Byzantine art.",
        "level": null,
        "credits": 15,
        "prerequisites": null
      },
      {
        "id": 23,
        "title": "History of Art 2",
        "code": "AT 1001",
        "description": "Survey of Western European architecture, sculpture, and painting from the medieval period to the present.",
        "level": null,
        "credits": 15,
        "prerequisites": null
      },
      {
        "id": 24,
        "title": "Writing about Art",
        "code": "AT 2224",
        "description": "Introduction to research methodology and the essential resources of art historical scholarship. Training in critical thinking, evaluation/synthesis of sources and the creation of an argument. Particular emphasis placed on writing a short research paper and the scholarly use of secondary resources.",
        "level": 4,
        "credits": 15,
        "prerequisites": [
          "AT 1000",
          "AT 1001"
        ]
      },
      {
        "id": 25,
        "title": "Art and Architecture of Ancient Greece",
        "code": "AT 2005",
        "description": "The art and architecture of ancient Greece from the Geometric period to the coming of Rome.",
        "level": 4,
        "credits": 15,
        "prerequisites": null
      },
      {
        "id": 26,
        "title": "Roman Art and Architecture",
        "code": "AT 2006",
        "description": "The art of the Republic and the Empire to the time of Constantine the Great. The art of Etruria briefly considered.",
        "level": 4,
        "credits": 15,
        "prerequisites": null
      },
      {
        "id": 27,
        "title": "History of Architecture",
        "code": "AT 1025",
        "description": "Examination of Western architecture from the Early Modern Period to the Present, through a series of key monuments and their context.",
        "level": 4,
        "credits": 15,
        "prerequisites": null
      },
      {
        "id": 28,
        "title": "Modern Art",
        "code": "AT 2113",
        "description": "Survey of the modernist period in visual arts covering the main artistic trends from the beginning to mid-twentieth century. The concept of modernity is examined vis--vis the theoretical, social and political changes characterizing the first half of the 20th century.",
        "level": 5,
        "credits": 15,
        "prerequisites": [
          "AT 1001"
        ]
      },
      {
        "id": 29,
        "title": "Theories of Art",
        "code": "AT 3023",
        "description": "A historical survey of the founding ideas, theories and philosophical systems that have formed the background of artistic production in Western civilization.",
        "level": 5,
        "credits": 15,
        "prerequisites": [
          "AT 1000",
          "AT 1001"
        ]
      },
      {
        "id": 30,
        "title": "Northern European Art 15th-16th c.",
        "code": "AT 2026",
        "description": "Art in Northern Europe during the 15th-16th centuries. Major and minor arts in Germany, France, the Low Countries, Britain and Austria.",
        "level": 5,
        "credits": 15,
        "prerequisites": null
      }
    ]
  }
]
```