{
  "info": {
    "name": "Open Skills API Job Titles and Descriptions",
    "_postman_id": "a65c54fa-19ad-4b81-8f1e-171dcc8c2cf4",
    "description": "Retrieves the names, descriptions, and UUIDs of all job titles.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Job",
      "item": [
        {
          "id": "bf7da1d7-1c3e-4fa7-be8f-5b92d18bfd62",
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
              "id": "9208896f-56aa-4721-b6a0-b3d608b91526"
            }
          ]
        }
      ]
    }
  ]
}