{
  "info": {
    "name": "Open Skills API Jobs Associated with a Job",
    "_postman_id": "f7a06912-a485-4ed3-8eef-f03d8b3aa725",
    "description": "Retrieves a collection of jobs associated with a specified job.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "jobs",
      "item": [
        {
          "id": "f400f996-1237-4954-8be4-bcd4d73fe5a3",
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
            "description": "Retrieves a collection of jobs associated with a specified job"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "67f5080f-62e8-449e-9a2c-76dafa9cf359"
            }
          ]
        }
      ]
    }
  ]
}