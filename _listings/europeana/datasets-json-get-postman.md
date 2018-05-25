{
  "info": {
    "name": "Europeana get the list of Europeana datasets",
    "_postman_id": "28b6a3db-aae5-43bd-884e-9ecc9e631e0e",
    "description": "Get the list of europeana datasets.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Dataset",
      "item": [
        {
          "id": "283d6814-ba6b-4df7-9462-675cd571a8cd",
          "name": "getDataset",
          "request": {
            "url": {
              "protocol": "http",
              "host": "www.europeana.eu",
              "path": [
                "v2",
                "dataset/:id.json"
              ],
              "query": [
                {
                  "key": "callback",
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
            "description": "Get information about a specific dataset."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "ecee442e-d421-405c-abb2-85ae6ae29601"
            }
          ]
        }
      ]
    },
    {
      "name": "Datasets",
      "item": [
        {
          "id": "5d9157c4-f18d-4df0-96ea-17a98698fac5",
          "name": "listDatasets",
          "request": {
            "url": "http://www.europeana.eu/v2/datasets.json?callback=%7B%7D&countryCode=%7B%7D&edmDatasetName=%7B%7D&offset=%7B%7D&pagesize=%7B%7D&status=%7B%7D&wskey=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Get the list of europeana datasets."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "397e0e7c-02ce-4690-9643-07ab595e5d0e"
            }
          ]
        }
      ]
    }
  ]
}