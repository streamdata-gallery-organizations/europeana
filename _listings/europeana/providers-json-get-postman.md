{
  "info": {
    "name": "Europeana get the list of Europeana data providers",
    "_postman_id": "2ad9067c-1bb8-47d1-9078-c10ab109af5e",
    "description": "Get the list of europeana data providers.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Dataset",
      "item": [
        {
          "id": "d1208036-50e3-464e-bb9a-06c1091d0974",
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
              "id": "ab697fda-f1a1-4fe8-bb59-131d2a351e3c"
            }
          ]
        }
      ]
    },
    {
      "name": "Datasets",
      "item": [
        {
          "id": "9be9a143-88f2-42ce-b150-d956bbab8f09",
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
              "id": "f298515a-ddb2-486f-a9a3-49c53ef5360c"
            }
          ]
        }
      ]
    },
    {
      "name": "Search",
      "item": [
        {
          "id": "b3583752-e3b1-40d9-b9cd-c99380d7439a",
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
              "id": "86af6bd0-4e19-4fe8-bae7-5719a42d3b41"
            }
          ]
        }
      ]
    },
    {
      "name": "Provider",
      "item": [
        {
          "id": "f5dbe38a-c26f-4b47-b547-c1eb2c041e88",
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
              "id": "cda553c4-febb-483e-b164-fe226ec55693"
            }
          ]
        }
      ]
    },
    {
      "name": "Providers",
      "item": [
        {
          "id": "24cb9efd-1e23-471d-baad-cb7e2ffc5514",
          "name": "listProviderDatasets",
          "request": {
            "url": {
              "protocol": "http",
              "host": "www.europeana.eu",
              "path": [
                "v2",
                "provider/:id/datasets.json"
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
            "description": "Get the list of datasets provided by a specific provider."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "73d7e7a6-deee-4267-9875-0eaa73cf4826"
            }
          ]
        },
        {
          "id": "7b30977e-c6b2-4956-b19b-5fb746127efd",
          "name": "listProviders",
          "request": {
            "url": "http://www.europeana.eu/v2/providers.json?callback=%7B%7D&countryCode=%7B%7D&offset=%7B%7D&pagesize=%7B%7D&wskey=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Get the list of europeana data providers."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "b1ea46ad-accb-493b-ac67-71a0c27ee20d"
            }
          ]
        }
      ]
    }
  ]
}