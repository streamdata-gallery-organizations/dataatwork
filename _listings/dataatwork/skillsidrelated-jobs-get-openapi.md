---
swagger: "2.0"
x-collection-name: DataAtWork
x-complete: 0
info:
  title: Open Skills API Jobs Associated with a Skill
  description: Retrieves a collection of jobs associated with a specified skill.
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
  /jobs/{id}/related_jobs:
    get:
      summary: Jobs Associated with a Job
      description: Retrieves a collection of jobs associated with a specified job.
      operationId: retrieves-a-collection-of-jobs-associated-with-a-specified-job
      x-api-path-slug: jobsidrelated-jobs-get
      parameters:
      - in: path
        name: id
        description: The UUID of the job to retrieve related jobs for
      responses:
        200:
          description: OK
      tags:
      - Jobs
      - Associated
      - Job
  /jobs/autocomplete:
    get:
      summary: Job Title Autocomplete
      description: Retrieves the names, descriptions, and UUIDs of all job titles
        matching a given search criteria.
      operationId: retrieves-the-names-descriptions-and-uuids-of-all-job-titles-matching-a-given-search-criteria
      x-api-path-slug: jobsautocomplete-get
      parameters:
      - in: query
        name: begins_with
        description: Find job titles beginning with the given text fragment
      - in: query
        name: contains
        description: Find job titles containing the given text fragment
      - in: query
        name: ends_with
        description: Find job titles ending with the given text fragment
      responses:
        200:
          description: OK
      tags:
      - Job
      - Title
      - Autocomplete
  /jobs/normalize:
    get:
      summary: Job Title Normalization
      description: Retrieves the canonical job title for a synonymous job title
      operationId: retrieves-the-canonical-job-title-for-a-synonymous-job-title
      x-api-path-slug: jobsnormalize-get
      parameters:
      - in: query
        name: job_title
        description: Find the canonical job title(s) for jobs matching the given text
          fragment
      - in: query
        name: limit
        description: Maximumn number of job title synonyms to return
      responses:
        200:
          description: OK
      tags:
      - Job
      - Title
      - Normalization
  /jobs/unusual_titles:
    get:
      summary: Unusual Job Titles
      description: Retrieves a list of unusual job titles and the UUIDs of their canonical
        jobs.
      operationId: retrieves-a-list-of-unusual-job-titles-and-the-uuids-of-their-canonical-jobs
      x-api-path-slug: jobsunusual-titles-get
      responses:
        200:
          description: OK
      tags:
      - Unusual
      - Job
      - Titles
  /skills:
    get:
      summary: Skill Names and Descriptions
      description: Retrieve the names, descriptions, and UUIDs of all skills.
      operationId: retrieve-the-names-descriptions-and-uuids-of-all-skills
      x-api-path-slug: skills-get
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
      - Skill
      - Names
      - Descriptions
  /skills/{id}:
    get:
      summary: Skill Name and Description
      description: Retrieves the name, description, and UUID of a job by specifying
        its UUID.
      operationId: retrieves-the-name-description-and-uuid-of-a-job-by-specifying-its-uuid
      x-api-path-slug: skillsid-get
      parameters:
      - in: path
        name: id
        description: The UUID of the skill name to retrieve
      responses:
        200:
          description: OK
      tags:
      - Skill
      - Name
      - Description
  /skills/{id}/related_jobs:
    get:
      summary: Jobs Associated with a Skill
      description: Retrieves a collection of jobs associated with a specified skill.
      operationId: retrieves-a-collection-of-jobs-associated-with-a-specified-skill
      x-api-path-slug: skillsidrelated-jobs-get
      parameters:
      - in: path
        name: id
        description: The UUID of the skill to retrieve jobs for
      responses:
        200:
          description: OK
      tags:
      - Jobs
      - Associated
      - Skill
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