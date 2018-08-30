---
swagger: "2.0"
x-collection-name: DataAtWork
x-complete: 0
info:
  title: Open Skills API Skills Associated with a Job
  description: Retrieves a collection of skills associated with a specified job.
  contact:
    name: Work Data Initiative
    url: http://www.dataatwork.org
  version: "1.0"
host: api.dataatwork.org
basePath: /v1
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /jobs:
    get:
      summary: Job Titles and Descriptions
      description: Retrieves the names, descriptions, and UUIDs of all job titles.
      operationId: retrieves-the-names-descriptions-and-uuids-of-all-job-titles
      x-api-path-slug: jobs-get
      parameters:
      - in: query
        name: limit
        description: Maximum number of items per page
      - in: query
        name: offset
        description: Pagination offset
      responses:
        200:
          description: OK
      tags:
      - Job
      - Titles
      - Descriptions
  /jobs/{id}:
    get:
      summary: Job Title and Description
      description: Retrieves the name, description, and UUID of a job by specifying
        its O*NET SOC Code or UUID.
      operationId: retrieves-the-name-description-and-uuid-of-a-job-by-specifying-its-onet-soc-code-or-uuid
      x-api-path-slug: jobsid-get
      parameters:
      - in: path
        name: id
        description: The O*NET SOC Code or UUID of the job title to retrieve
      responses:
        200:
          description: OK
      tags:
      - Job
      - Title
      - Description
  /jobs/{id}/related_skills:
    get:
      summary: Skills Associated with a Job
      description: Retrieves a collection of skills associated with a specified job.
      operationId: retrieves-a-collection-of-skills-associated-with-a-specified-job
      x-api-path-slug: jobsidrelated-skills-get
      parameters:
      - in: path
        name: id
        description: The UUID of the job to retrieve skills for
      responses:
        200:
          description: OK
      tags:
      - Skills
      - Associated
      - Job
x-streamrank:
  polling_total_time_average: 0
  polling_size_download_average: 0
  streaming_total_time_average: 0
  streaming_size_download_average: 0
  change_yes: 0
  change_no: 0
  time_percentage: 0
  size_percentage: 0
  change_percentage: 0
  last_run: ""
  days_run: 0
  minute_run: 0
---