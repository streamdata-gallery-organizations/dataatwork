{
  "info": {
    "name": "Open Skills API Job Title Autocomplete",
    "_postman_id": "14f3f2ab-c27a-4c45-92a8-c954efd4d4c1",
    "description": "Retrieves the names, descriptions, and UUIDs of all job titles matching a given search criteria.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "job",
      "item": [
        {
          "id": "219a953b-c9cf-4e06-87ee-c8dd30e723db",
          "name": "retrieves-the-names-descriptions-and-uuids-of-all-job-titles-matching-a-given-search-criteria",
          "request": {
            "url": "http://api.dataatwork.org/v1/jobs/autocomplete?begins_with=%7B%7D&contains=%7B%7D&ends_with=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Retrieves the names, descriptions, and UUIDs of all job titles matching a given search criteria"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "94fa6f3f-ab5f-483d-9f6d-4cd972830d02"
            }
          ]
        }
      ]
    }
  ]
}