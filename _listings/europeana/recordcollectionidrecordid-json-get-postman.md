{
  "info": {
    "name": "Europeana get a single record in JSON format",
    "_postman_id": "35c2bfa7-0e06-4e0d-8af0-0d0ce7eae548",
    "description": "Get a single record in json format.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Collections",
      "item": [
        {
          "id": "06289f69-ae83-4752-a936-f4162c66722f",
          "name": "getSingleRecordJson",
          "request": {
            "url": {
              "protocol": "http",
              "host": "www.europeana.eu",
              "path": [
                "v2",
                "record/:collectionId/:recordId.json"
              ],
              "query": [
                {
                  "key": "callback",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "hierarchytimeout",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "profile",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "wskey",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "collectionId",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "recordId",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Get a single record in json format."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "e2bad7de-4bd9-4ab2-a4ea-2aaf9355bf9c"
            }
          ]
        }
      ]
    }
  ]
}