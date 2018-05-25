{
  "info": {
    "name": "Europeana get information about a specific Europeana provider",
    "_postman_id": "4f18da4f-bb36-4ea5-9d8b-27139254f216",
    "description": "Get information about a specific europeana provider.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Dataset",
      "item": [
        {
          "id": "98fcf7a5-64a5-463e-be4a-bfdcde763523",
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
              "id": "9ba828e0-03b6-437b-97fd-1b8814ca8b6f"
            }
          ]
        }
      ]
    },
    {
      "name": "Datasets",
      "item": [
        {
          "id": "895cfb36-e5f9-48ca-ba21-7d47827a2e38",
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
              "id": "8b96400d-e5e2-4463-8e0a-d643899c58b1"
            }
          ]
        }
      ]
    },
    {
      "name": "Search",
      "item": [
        {
          "id": "0f27a400-67fe-49b1-b337-f68728518a6a",
          "name": "openSearch",
          "request": {
            "url": "http://www.europeana.eu/v2/opensearch.rss?count=%7B%7D&searchTerms=%7B%7D&startIndex=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Basic search function following the opensearch specification."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "8488189c-b492-43b4-acaf-7f17de74d36a"
            }
          ]
        }
      ]
    },
    {
      "name": "Provider",
      "item": [
        {
          "id": "4faf2976-8b6b-4cf6-b5b9-108cdfecd0ff",
          "name": "getProvider",
          "request": {
            "url": {
              "protocol": "http",
              "host": "www.europeana.eu",
              "path": [
                "v2",
                "provider/:id.json"
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
            "description": "Get information about a specific europeana provider."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "175d3603-6aa8-4992-8333-72da42f2bf00"
            }
          ]
        }
      ]
    }
  ]
}