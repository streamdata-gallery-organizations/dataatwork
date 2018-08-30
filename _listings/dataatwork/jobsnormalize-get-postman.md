{
  "info": {
    "name": "Open Skills API Job Title Normalization",
    "_postman_id": "c79af895-6cc3-40cf-928b-33323285ea49",
    "description": "Retrieves the canonical job title for a synonymous job title",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Job",
      "item": [
        {
          "id": "e154afe5-33a9-43ae-805f-b6b04f26d2f0",
          "name": "retrieves-the-names-descriptions-and-uuids-of-all-job-titles",
          "request": {
            "url": "http://api.dataatwork.org/v1/jobs?limit=%7B%7D&offset=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Retrieves the names, descriptions, and UUIDs of all job titles."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "761e5f92-91cf-490c-819d-3579962d23a4"
            }
          ]
        },
        {
          "id": "57412c5b-1fb7-4ef6-92b1-6677fe154a59",
          "name": "retrieves-the-name-description-and-uuid-of-a-job-by-specifying-its-onet-soc-code-or-uuid",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.dataatwork.org",
              "path": [
                "v1",
                "jobs/:id"
              ],
              "variable": [
                {
                  "id": "id",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Retrieves the name, description, and UUID of a job by specifying its O*NET SOC Code or UUID."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "3fd52942-bd4b-4de0-a5f5-97578f6f4cf4"
            }
          ]
        },
        {
          "id": "d7f7dd44-1c05-4020-87c8-7a4ac2e9c8d2",
          "name": "retrieves-the-names-descriptions-and-uuids-of-all-job-titles-matching-a-given-search-criteria",
          "request": {
            "url": "http://api.dataatwork.org/v1/jobs/autocomplete?begins_with=%7B%7D&contains=%7B%7D&ends_with=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Retrieves the names, descriptions, and UUIDs of all job titles matching a given search criteria."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "67bf36fc-7e99-4e1f-9c33-e254afd30d39"
            }
          ]
        },
        {
          "id": "abf17b35-aa90-4f13-b0af-25dd4fc86a41",
          "name": "retrieves-the-canonical-job-title-for-a-synonymous-job-title",
          "request": {
            "url": "http://api.dataatwork.org/v1/jobs/normalize?job_title=%7B%7D&limit=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Retrieves the canonical job title for a synonymous job title"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "105f68d0-8203-40b2-8d85-898ed4490f31"
            }
          ]
        }
      ]
    },
    {
      "name": "Skills",
      "item": [
        {
          "id": "e06289e7-7f5f-466b-b56c-139a22c13049",
          "name": "retrieves-a-collection-of-skills-associated-with-a-specified-job",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.dataatwork.org",
              "path": [
                "v1",
                "jobs/:id/related_skills"
              ],
              "variable": [
                {
                  "id": "id",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Retrieves a collection of skills associated with a specified job."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "ee0d52d2-825b-42d6-a198-3364b8fac584"
            }
          ]
        }
      ]
    },
    {
      "name": "Jobs",
      "item": [
        {
          "id": "12c7fc7b-913a-4b32-9755-c05813721bd5",
          "name": "retrieves-a-collection-of-jobs-associated-with-a-specified-job",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.dataatwork.org",
              "path": [
                "v1",
                "jobs/:id/related_jobs"
              ],
              "variable": [
                {
                  "id": "id",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Retrieves a collection of jobs associated with a specified job."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "523d3190-da85-4026-a2d3-ebd087f1cb36"
            }
          ]
        }
      ]
    }
  ]
}