{
  "info": {
    "name": "Open Skills API Unusual Job Titles",
    "_postman_id": "767bb4ee-3f53-449d-9bda-30ea9441e4d4",
    "description": "Retrieves a list of unusual job titles and the UUIDs of their canonical jobs.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Job",
      "item": [
        {
          "id": "e9200bee-b5cb-45c1-be49-7f95e09c857a",
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
              "id": "04177af9-dfe2-42ff-99c0-7da1e5511eed"
            }
          ]
        },
        {
          "id": "968c1bc9-9543-4a28-a428-275019456cf8",
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
              "id": "53b36bd8-9042-4485-92e3-851afd10f669"
            }
          ]
        },
        {
          "id": "b0aaa88d-e219-48fb-936d-2606f1fccc6f",
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
              "id": "5dd5a7f3-371b-47a0-bf73-3835e57bb721"
            }
          ]
        },
        {
          "id": "129894a4-a06d-4fda-aba5-c9e7fde25eae",
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
              "id": "88374fad-5c02-4315-8ce1-5c43a87d24eb"
            }
          ]
        }
      ]
    },
    {
      "name": "Skills",
      "item": [
        {
          "id": "d0caf677-ca58-47d5-bcb9-e3ceef698064",
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
              "id": "92c9d15a-1639-4752-acd0-7786a148f487"
            }
          ]
        }
      ]
    },
    {
      "name": "Jobs",
      "item": [
        {
          "id": "9fd5f28c-30be-4a15-a252-4d1cd520a70e",
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
              "id": "c49bc468-ef55-40f8-852d-244bc5e207be"
            }
          ]
        }
      ]
    },
    {
      "name": "Unusual",
      "item": [
        {
          "id": "94a1ed27-4542-42b4-98b2-120d6d26dbd9",
          "name": "retrieves-a-list-of-unusual-job-titles-and-the-uuids-of-their-canonical-jobs",
          "request": {
            "url": "http://api.dataatwork.org/v1/jobs/unusual_titles",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Retrieves a list of unusual job titles and the UUIDs of their canonical jobs."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "ebda65a8-caac-48b2-a2dc-a522f725b784"
            }
          ]
        }
      ]
    }
  ]
}