<p align="center">
  <img src="http://open.course.s3.amazonaws.com/web.png" alt="OpenCourse" width="200"/>
</p>

## Overview
The OpenCourse project was made as part of the capstone project of ITC 4918. It provides a lightweight API for data relevant to the majors and courses the college provides. This is a student project and is not affiliated in any way with the college.

Another part of this project is the OpenCourse iOS client, called **Courses**. **Courses** utilizes in full extend the OpenCourse API and provides a catalogue with all majors and courses, as calculation of suggested courses based on passed courses, course bookmarking, note keeping and many more features.

## Disclaimer

Review the _"Restrictions"_ section of the docs before using the OpenCourse API data. In case you build a service upon this data, please inform your users of the potentials risks.

## Accessing the API

All calls are made to the following URL with the required parameters for a given service.

`http://opencourse.me/api/`

To make an API call, you must have a valid **API Key**. The response format is currently in `json` (other formats like `xml` are intended to be added in the near future).

## Endpoints

### Courses

- [/courses/id/{course_id}](/api/courses/courses_id.md)
- [/courses/code/{code}](/api/courses/courses_code.md)

### Departments

- [/departments/all](/api/departments/departments_all.md)
- [/department/id/{department_id}](/api/departments/departments_id.md)

### Majors

- [/majors/all](/api/majors/majors_all.md)
- [/majors/school/{school_id}](/api/majors/majors_school.md)
- [/majors/id/{major_id}/items](/api/majors/majors_id_items.md)

## Restrictions

### API Key
Currently, an API Key is required to make any API calls. Please request a key by contacting [m.apostolakis@acg.edu](mailto:m.apostolakis@acg.edu).

### Data

All data offered by the API are public. This project does not store nor provide any private data such as student data. 

**Warning** the accuracy of the data is by any means guaranteed.  This means anything can change at any point in the future and the API **could** become outdated.

This project was built as part of a course requirement and is not intended to be used as a commercial product.

## Contributing

If you would like to offer your suggestions or report any errors  or updates for the courses and majors, please create a [new issue](https://github.com/mapostolakis/OpenCourse-API-docs/issues/new) of the OpenCourse Documentation [repository](https://github.com/mapostolakis/OpenCourse-API-docs/) and label it appropriately.

## Contact

If you have any suggestions or just want to get in touch with me, please feel free to contact me at [m.apostolakis@acg.edu](mailto:m.apostolakis@acg.edu) or at my [GitHub](https://github.com/mapostolakis) page.
