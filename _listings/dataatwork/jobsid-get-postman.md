{
  "info": {
    "name": "Open Skills API Job Title and Description",
    "_postman_id": "8b6d8a13-6c4f-4480-b199-162c3e72b096",
    "description": "Retrieves the name, description, and UUID of a job by specifying its O*NET SOC Code or UUID.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Job",
      "item": [
        {
          "id": "de820e5b-fb34-435f-9f83-806d78d825ba",
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
              "id": "3c190de6-ee5e-479a-9914-dd19554b3e45"
            }
          ]
        },
        {
          "id": "0259bf26-9b78-4865-935a-9d3dc82661e4",
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
              "id": "04723257-cfd7-43e9-a903-7d21e302f247"
            }
          ]
        }
      ]
    }
  ]
}