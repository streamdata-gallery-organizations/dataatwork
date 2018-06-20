---
name: DataAtWork
x-slug: dataatwork
description: ""
image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Screen
  Shot 2016-10-12 at 11.19.25 PM.png
x-kinRank: "8"
x-alexaRank: "0"
tags: DataAtWork
created: "2018-06-20"
modified: "2018-06-20"
url: https://raw.githubusercontent.com/streamdata-gallery-organizations/dataatwork/master/_listings/dataatwork/apis.md
specificationVersion: "0.14"
apis:
- name: Open Skills API Job Titles and Descriptions
  x-api-slug: open-skills-api
  description: Retrieves the names, descriptions, and UUIDs of all job titles.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Screen
    Shot 2016-10-12 at 11.19.25 PM.png
  humanURL: http://www.dataatwork.org/
  baseURL: ://api.dataatwork.org//v1//jobs
  tags: Job, Titles, Descriptions
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/dataatwork/master/_listings/dataatwork/jobs-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/dataatwork/master/_listings/dataatwork/jobs-get-openapi.md
- name: Open Skills API Job Title and Description
  x-api-slug: open-skills-api
  description: Retrieves the name, description, and UUID of a job by specifying its
    O*NET SOC Code or UUID.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Screen
    Shot 2016-10-12 at 11.19.25 PM.png
  humanURL: http://www.dataatwork.org/
  baseURL: ://api.dataatwork.org//v1//jobs/{id}
  tags: Job, Title, Description
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/dataatwork/master/_listings/dataatwork/jobsid-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/dataatwork/master/_listings/dataatwork/jobsid-get-openapi.md
- name: Open Skills API Skills Associated with a Job
  x-api-slug: open-skills-api
  description: Retrieves a collection of skills associated with a specified job.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Screen
    Shot 2016-10-12 at 11.19.25 PM.png
  humanURL: http://www.dataatwork.org/
  baseURL: ://api.dataatwork.org//v1//jobs/{id}/related_skills
  tags: Skills, Associated, Job
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/dataatwork/master/_listings/dataatwork/jobsidrelated-skills-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/dataatwork/master/_listings/dataatwork/jobsidrelated-skills-get-openapi.md
- name: Open Skills API Jobs Associated with a Job
  x-api-slug: open-skills-api
  description: Retrieves a collection of jobs associated with a specified job.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Screen
    Shot 2016-10-12 at 11.19.25 PM.png
  humanURL: http://www.dataatwork.org/
  baseURL: ://api.dataatwork.org//v1//jobs/{id}/related_jobs
  tags: Jobs, Associated, Job
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/dataatwork/master/_listings/dataatwork/jobsidrelated-jobs-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/dataatwork/master/_listings/dataatwork/jobsidrelated-jobs-get-openapi.md
- name: Open Skills API Job Title Autocomplete
  x-api-slug: open-skills-api
  description: Retrieves the names, descriptions, and UUIDs of all job titles matching
    a given search criteria.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Screen
    Shot 2016-10-12 at 11.19.25 PM.png
  humanURL: http://www.dataatwork.org/
  baseURL: ://api.dataatwork.org//v1//jobs/autocomplete
  tags: Job, Title, Autocomplete
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/dataatwork/master/_listings/dataatwork/jobsautocomplete-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/dataatwork/master/_listings/dataatwork/jobsautocomplete-get-openapi.md
- name: Open Skills API Job Title Normalization
  x-api-slug: open-skills-api
  description: Retrieves the canonical job title for a synonymous job title
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Screen
    Shot 2016-10-12 at 11.19.25 PM.png
  humanURL: http://www.dataatwork.org/
  baseURL: ://api.dataatwork.org//v1//jobs/normalize
  tags: Job, Title, Normalization
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/dataatwork/master/_listings/dataatwork/jobsnormalize-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/dataatwork/master/_listings/dataatwork/jobsnormalize-get-openapi.md
- name: Open Skills API Unusual Job Titles
  x-api-slug: open-skills-api
  description: Retrieves a list of unusual job titles and the UUIDs of their canonical
    jobs.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Screen
    Shot 2016-10-12 at 11.19.25 PM.png
  humanURL: http://www.dataatwork.org/
  baseURL: ://api.dataatwork.org//v1//jobs/unusual_titles
  tags: Unusual, Job, Titles
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/dataatwork/master/_listings/dataatwork/jobsunusual-titles-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/dataatwork/master/_listings/dataatwork/jobsunusual-titles-get-openapi.md
- name: Open Skills API Skill Names and Descriptions
  x-api-slug: open-skills-api
  description: Retrieve the names, descriptions, and UUIDs of all skills.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Screen
    Shot 2016-10-12 at 11.19.25 PM.png
  humanURL: http://www.dataatwork.org/
  baseURL: ://api.dataatwork.org//v1//skills
  tags: Skill, Names, Descriptions
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/dataatwork/master/_listings/dataatwork/skills-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/dataatwork/master/_listings/dataatwork/skills-get-openapi.md
- name: Open Skills API Skill Name and Description
  x-api-slug: open-skills-api
  description: Retrieves the name, description, and UUID of a job by specifying its
    UUID.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Screen
    Shot 2016-10-12 at 11.19.25 PM.png
  humanURL: http://www.dataatwork.org/
  baseURL: ://api.dataatwork.org//v1//skills/{id}
  tags: Skill, Name, Description
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/dataatwork/master/_listings/dataatwork/skillsid-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/dataatwork/master/_listings/dataatwork/skillsid-get-openapi.md
- name: Open Skills API Jobs Associated with a Skill
  x-api-slug: open-skills-api
  description: Retrieves a collection of jobs associated with a specified skill.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Screen
    Shot 2016-10-12 at 11.19.25 PM.png
  humanURL: http://www.dataatwork.org/
  baseURL: ://api.dataatwork.org//v1//skills/{id}/related_jobs
  tags: Jobs, Associated, Skill
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/dataatwork/master/_listings/dataatwork/skillsidrelated-jobs-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/dataatwork/master/_listings/dataatwork/skillsidrelated-jobs-get-openapi.md
- name: Open Skills API Skills Associated with a Skill
  x-api-slug: open-skills-api
  description: Retrieves a collection of skills associated with a specified skill.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Screen
    Shot 2016-10-12 at 11.19.25 PM.png
  humanURL: http://www.dataatwork.org/
  baseURL: ://api.dataatwork.org//v1//skills/{id}/related_skills
  tags: Skills, Associated, Skill
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/dataatwork/master/_listings/dataatwork/skillsidrelated-skills-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/dataatwork/master/_listings/dataatwork/skillsidrelated-skills-get-openapi.md
- name: Open Skills API Skill Name Autocomplete
  x-api-slug: open-skills-api
  description: Retrieves the names, descriptions, and UUIDs of all skills matching
    a given search criteria.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Screen
    Shot 2016-10-12 at 11.19.25 PM.png
  humanURL: http://www.dataatwork.org/
  baseURL: ://api.dataatwork.org//v1//skills/autocomplete
  tags: Skill, Name, Autocomplete
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/dataatwork/master/_listings/dataatwork/skillsautocomplete-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/dataatwork/master/_listings/dataatwork/skillsautocomplete-get-openapi.md
- name: Open Skills API Skill Name Normalization
  x-api-slug: open-skills-api
  description: Retrieves the canonical skill name for a synonymous skill name
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Screen
    Shot 2016-10-12 at 11.19.25 PM.png
  humanURL: http://www.dataatwork.org/
  baseURL: ://api.dataatwork.org//v1//skills/normalize
  tags: Skill, Name, Normalization
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/dataatwork/master/_listings/dataatwork/skillsnormalize-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/dataatwork/master/_listings/dataatwork/skillsnormalize-get-openapi.md
- name: Open Skills API
  x-api-slug: open-skills-api
  description: ""
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Screen
    Shot 2016-10-12 at 11.19.25 PM.png
  humanURL: http://www.dataatwork.org/
  baseURL: ://api.dataatwork.org//v1
  tags: DataAtWork
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/dataatwork/master/_listings/dataatwork/openapi.md
x-common:
- type: x-developer
  url: http://api.dataatwork.org/v1/spec/
- type: x-website
  url: http://www.dataatwork.org/
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---